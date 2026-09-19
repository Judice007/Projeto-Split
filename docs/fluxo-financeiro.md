# Fluxo financeiro completo (rascunho)

> **Status: rascunho técnico para validação jurídica, contábil e com o parceiro de pagamentos.** Este documento traduz a seção 6 do [Documento Mestre](documento-mestre.md) em estados e transições. Nada aqui deve ser implementado em código antes de confirmação com um parceiro de pagamentos real e parecer jurídico (ver seção 6.4 — condicionante obrigatória: split de pagamento, agenda de repasse e retenção não são a mesma coisa, e custódia/escrow só pode ser prometida se suportada pelo provedor).

## 1. Visão geral dos estados de uma cota (vaga em grupo público)

```
[Solicitação] → [Entrada paga] → [Ativa] → [Renovação mensal] ⇄ [Ativa]
                                     ↓
                          [Disputa aberta] → [Resolvida] → [Ativa | Encerrada]
                                     ↓
                              [Encerrada] → [Substituição assistida | Estorno | Realocação]
```

## 2. Entrada (primeira cobrança)

**Gatilho:** participante aceita as regras do grupo e confirma pagamento.

**Cobrança:** 2 mensalidades + taxa da plataforma (regra da seção 6.1).

| Parcela | Destino imediato | Quando fica disponível ao administrador |
|---|---|---|
| 1ª mensalidade | Reserva/custódia da plataforma | Após defasagem de 1 ciclo, se não houver disputa qualificada aberta e o acesso permanecer válido |
| 2ª mensalidade | Reserva/custódia da plataforma | Cobre o ciclo seguinte OU funciona como reserva operacional — **decisão pendente** (ver `decisoes-pendentes.md`), depende de estrutura final acordada com o parceiro de pagamentos |
| Taxa da plataforma | Receita da plataforma | Imediato (ou conforme regra fiscal aplicável) |

**Pré-condições para aceitar a entrada:**
- Grupo público com identidade do administrador verificada (seção 4.1).
- Serviço com ficha de elegibilidade aprovada (seção 4.3 / `matriz-servicos.md`).
- Vaga disponível no grupo.
- Preço e taxa exibidos antes da confirmação de pagamento (regra do marketplace, seção 12).

**Efeito colateral:** administrador é notificado para fornecer acesso; contagem do prazo de segurança (seção 6.3) é iniciada.

## 3. Durante o ciclo

- Participante usa o serviço e pode reportar problemas a qualquer momento.
- Plataforma monitora: prazo de segurança antes do primeiro saque ainda correndo, existência de disputas abertas, comportamento de risco.
- Administrador deve manter o acesso válido durante todo o período pago (regra do marketplace).

## 4. Transição para o ciclo seguinte (renovação)

**Gatilho:** fim do ciclo pago, sem disputa qualificada em aberto.

1. Participante passa à cobrança mensal recorrente (não paga mais "2 mensalidades", apenas 1 + taxa, salvo decisão em contrário).
2. Plataforma libera o valor referente ao ciclo anterior ao administrador, respeitando:
   - Prazo de segurança já cumprido.
   - Ausência de bloqueio de repasse por disputa.
   - Conta de recebimento vinculada ao titular verificado (mesmo CPF/CNPJ do cadastro do grupo).
3. Administrador recebe o repasse do **ciclo anterior**, nunca do ciclo corrente — a defasagem de 1 ciclo é estrutural, não um atraso operacional.

**Ponto em aberto:** a política exata de o que acontece com a "segunda mensalidade" original quando o participante permanece no grupo por múltiplos ciclos (ela se torna reserva permanente? é devolvida em algum momento? cobre o último ciclo na saída?) é uma decisão pendente e deve ser definida com o parceiro de pagamentos antes de qualquer implementação.

## 5. Disputa (bloqueio de repasse)

**Gatilho:** participante ou administrador abre chamado (motivos na seção 13.1: acesso não fornecido, acesso removido antes do fim do período, serviço cancelado, plano diferente do anunciado, cobrança incorreta, comportamento abusivo, uso incompatível pelo participante).

```
1. Chamado aberto com motivo e evidências iniciais.
2. Sistema registra e avalia bloqueio preventivo do próximo repasse relacionado.
3. Parte contrária é notificada e tem prazo para responder com evidências.
4. Atendimento decide conforme política publicada.
5. Resultado possível: correção, crédito, realocação, estorno, liberação do repasse retido, ou sanção ao administrador/participante.
6. Caso é registrado no histórico de risco e reputação de ambas as partes.
```

**Regra crítica:** o bloqueio de repasse é uma ferramenta de proteção, não uma retenção automática de todo o saldo do administrador — precisa ser desenhado para não penalizar arbitrariamente grupos sem relação com a disputa.

## 6. Estorno / cancelamento

**Cenários possíveis (a mapear em detalhe com jurídico):**
- Estorno total antes de qualquer uso do acesso (ex.: acesso nunca fornecido).
- Estorno parcial proporcional ao tempo não utilizado.
- Substituição assistida em vez de estorno, se o participante consentir e houver grupo compatível (seção 6.5).
- Recusa de estorno quando o motivo é uso incompatível com as regras pelo próprio participante.

**Todos os cenários dependem de:** política de estorno publicada e compreensível antes do pagamento (seção 13.2), e compatibilidade com regras de proteção ao consumidor (seção 15).

## 7. Chargeback

**Gatilho:** participante contesta a cobrança diretamente com a operadora/banco, fora do fluxo de disputa da plataforma.

1. Plataforma é notificada pelo parceiro de pagamentos.
2. Valor relacionado deve ser identificado e, se ainda não repassado, retido.
3. Se já repassado ao administrador, tratar como saldo negativo a recuperar (ver seção 6.3 — "tratamento de chargeback e saldo negativo").
4. Caso alimenta o histórico de risco do participante (chargebacks recorrentes podem indicar abuso).

**Ponto em aberto:** mecanismo de cobrança do saldo negativo do administrador quando o valor já foi repassado (desconto de repasses futuros? cobrança direta? limite de exposição da plataforma?) — decisão pendente, depende do parceiro de pagamentos.

## 8. Encerramento do grupo

**Gatilhos possíveis:** administrador encerra voluntariamente, serviço é cancelado, administrador perde elegibilidade (fraude, reincidência de disputas), ou o fornecedor do serviço muda regras que tornam o grupo inelegível.

```
1. Grupo marcado como encerrado; novas entradas bloqueadas.
2. Participantes ativos notificados.
3. Plataforma avalia substituição assistida (grupo compatível em preço/serviço/regras) — só ocorre com consentimento claro do participante.
4. Se não houver substituição aceita, segue para estorno conforme política vigente.
5. Saldo retido do administrador é liquidado conforme regras de disputas em aberto e prazos de segurança.
```

## 9. Controles que este fluxo pressupõe (seção 6.3, para referência)

- Prazo de segurança antes do primeiro saque.
- Bloqueio de repasse durante disputa qualificada.
- Conta de recebimento vinculada ao titular verificado.
- Histórico de cobranças, estornos e repasses acessível para auditoria.
- Limites progressivos para contas novas (administradores recentes têm exposição menor).
- Proibição de cobrança externa em grupos públicos.
- Conciliação financeira periódica com trilha de auditoria.

## 10. O que falta para este fluxo sair do papel

- [ ] Confirmar com o parceiro de pagamentos quais desses estados (retenção, split, agenda de repasse) ele suporta nativamente e quais exigiriam lógica própria da plataforma.
- [ ] Definir juridicamente se o modelo de retenção configura ou não custódia/escrow, e o que isso implica em termos regulatórios.
- [ ] Fechar a política da "segunda mensalidade" em cada cenário (permanência longa, saída antecipada, encerramento do grupo).
- [ ] Definir limites numéricos: prazo de segurança (dias), limites progressivos por conta nova, teto de exposição a chargeback.
- [ ] Redigir a política de estorno/cancelamento em linguagem compreensível para o usuário final, a ser exibida antes do pagamento.
