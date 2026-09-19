# Wireframes das jornadas críticas (rascunho de baixa fidelidade)

> **Status: rascunho para discussão, não layout final.** Wireframes em ASCII para validar fluxo e informação por tela antes de qualquer decisão visual (cores, tipografia e identidade ficam para a Etapa 6, conforme o [Documento Mestre](documento-mestre.md)). Cobre as 4 jornadas da seção 5 e usa as telas do mapa da seção 11.

## Convenções

- `[Botão]` = ação principal
- `( )` `(•)` = campo de seleção
- `[____]` = campo de texto
- `⚠` = aviso/regra de negócio que precisa aparecer nessa tela
- `?` = decisão pendente que afeta o wireframe (ver `decisoes-pendentes.md`)

---

## Jornada 1 — Entrada de participante (seção 5.1)

`Criar conta → confirmar contatos → verificar identidade → buscar serviço → analisar grupo → aceitar regras → pagar entrada → receber instruções → confirmar funcionamento → acompanhar cobrança → avaliar experiência`

### Tela 1.1 — Criar conta (área Pública)
```
┌─────────────────────────────────────────┐
│  Projeto Split                    Entrar │
├─────────────────────────────────────────┤
│         Criar conta                      │
│  Nome completo   [___________________]   │
│  E-mail          [___________________]   │
│  Celular         [___________________]   │
│  Senha           [___________________]   │
│  ( ) Aceito os Termos e a Política       │
│  [Criar conta]                           │
└─────────────────────────────────────────┘
```

### Tela 1.2 — Confirmar contatos
```
┌─────────────────────────────────────────┐
│  Confirme seu e-mail e celular           │
│  Código enviado para j***@email.com      │
│  Código  [______]      [Reenviar]        │
│  [Confirmar]                             │
└─────────────────────────────────────────┘
```

### Tela 1.3 — Verificar identidade (participante)
> ⚠ Exigência de verificação para participante é uma decisão pendente — pode variar por valor/serviço. Este wireframe assume o caminho "verificação exigida".
```
┌─────────────────────────────────────────┐
│  Verificar identidade                    │
│  CPF          [___________________]      │
│  Selfie       [Tirar foto]               │
│  ⚠ Usamos isso só para reduzir fraude,   │
│    não é garantia de comportamento       │
│    futuro do administrador.              │
│  [Enviar]                                │
└─────────────────────────────────────────┘
```

### Tela 1.4 — Marketplace (busca)
```
┌─────────────────────────────────────────┐
│  Buscar: [streaming de video____] [Filtrar▾]│
│  Filtros: Categoria  Preço  Vagas  Reputação│
├─────────────────────────────────────────┤
│  [Netflix Família]  R$20/mês  3 vagas    │
│    Admin: ★★★★☆ Identidade verificada    │
│  [Spotify Duo]      R$12/mês  1 vaga     │
│    Admin: ★★★★★ Administrador Pro        │
│  [Google One 2TB]   R$8/mês   4 vagas    │
└─────────────────────────────────────────┘
```

### Tela 1.5 — Página do grupo
```
┌─────────────────────────────────────────┐
│  Netflix Família — Grupo #1234           │
│  Admin: Maria S. ✔ Identidade verificada │
│         ⭐ Administrador de confiança     │
│  Preço: R$20/mês | Vagas: 3 de 4         │
│  Regras: sem revenda, uso pessoal        │
│  Tempo de atividade: 8 meses             │
│  Condições de saída: aviso de 7 dias     │
│  [Ver regras completas]                  │
│  [Solicitar entrada]                     │
└─────────────────────────────────────────┘
```

### Tela 1.6 — Aceitar regras + checkout
```
┌─────────────────────────────────────────┐
│  Entrar no grupo Netflix Família         │
│  Você vai pagar agora:                   │
│    2 mensalidades          R$ 40,00      │
│    Taxa da plataforma      R$  X,XX      │
│    Total                   R$ XX,XX      │
│  ⚠ Por que 2 mensalidades? [Saiba mais]  │
│  ( ) Li e aceito as regras do grupo      │
│  ( ) Li e aceito Termos e Política       │
│  Forma de pagamento  [Cartão ▾]          │
│  [Pagar e entrar]                        │
└─────────────────────────────────────────┘
```

### Tela 1.7 — Instruções de acesso (pós-pagamento)
```
┌─────────────────────────────────────────┐
│  ✔ Pagamento confirmado                  │
│  O administrador foi notificado e tem    │
│  até 24h para liberar seu acesso.        │
│  [Ver instruções quando disponíveis]     │
│  [Reportar problema]                     │
└─────────────────────────────────────────┘
```

### Tela 1.8 — Minhas assinaturas / Cobranças (área Participante)
```
┌─────────────────────────────────────────┐
│  Dashboard        Minhas assinaturas     │
├─────────────────────────────────────────┤
│  Netflix Família   Ativo   próx. 12/10   │
│  Spotify (pessoal) Ativo   próx. 05/10   │
│  Gasto mensal total: R$ XX,XX            │
│  [Confirmar que está funcionando]        │
│  [Avaliar experiência]                   │
└─────────────────────────────────────────┘
```

---

## Jornada 2 — Criação de grupo (seção 5.2)

`Criar conta → verificar identidade → cadastrar recebimento → selecionar serviço elegível → informar plano/preço/vagas/regras → comprovar assinatura → análise → publicar → receber participantes → manter acesso → receber repasses`

### Tela 2.1 — Cadastrar recebimento
```
┌─────────────────────────────────────────┐
│  Dados de recebimento                    │
│  ⚠ Deve ser o mesmo CPF/CNPJ verificado  │
│  CPF/CNPJ   [___________________]        │
│  Chave Pix / conta [_______________]     │
│  [Salvar e continuar]                    │
└─────────────────────────────────────────┘
```

### Tela 2.2 — Selecionar serviço elegível
```
┌─────────────────────────────────────────┐
│  Que serviço você quer compartilhar?     │
│  [Buscar serviço_______________]         │
│  ✔ Netflix — elegível                    │
│  ✔ Spotify — elegível                    │
│  ✖ Serviço X — não elegível ainda        │
│     [Sugerir este serviço]               │
└─────────────────────────────────────────┘
```

### Tela 2.3 — Configurar grupo
```
┌─────────────────────────────────────────┐
│  Novo grupo — Netflix                    │
│  Tipo         (•) Público  ( ) Privado   │
│  Plano        [Família 4 telas ▾]        │
│  Preço/vaga   [R$ ____]                  │
│  Vagas totais [____]                     │
│  Regras       [____________________]     │
│  Condição de saída [aviso de __ dias]    │
│  [Continuar]                             │
└─────────────────────────────────────────┘
```

### Tela 2.4 — Comprovar assinatura + enviar para análise
```
┌─────────────────────────────────────────┐
│  Comprovar assinatura ativa              │
│  [Anexar comprovante/print]              │
│  ⚠ Seu grupo só aparece no marketplace   │
│    após análise (pode levar até X dias)  │
│  [Enviar para análise]                   │
└─────────────────────────────────────────┘
```

### Tela 2.5 — Meus grupos (área Administrador)
```
┌─────────────────────────────────────────┐
│  Meus grupos                             │
│  Netflix Família   Em análise            │
│  Spotify Duo       Publicado  1/2 vagas  │
├─────────────────────────────────────────┤
│  Cobranças e repasses                    │
│  Próximo repasse: R$ XX,XX em 12/10      │
│  Ciclo atual retido até: 12/10           │
│  ⚠ 1 disputa aberta pode atrasar repasse │
└─────────────────────────────────────────┘
```

---

## Jornada 3 — Gestão financeira / Gestor de assinaturas (seção 5.3)

`Cadastrar assinatura → informar preço/periodicidade/vencimento → classificar pessoal ou compartilhada → acompanhar totais → receber alertas → revisar economia`

### Tela 3.1 — Cadastrar assinatura manual
```
┌─────────────────────────────────────────┐
│  Nova assinatura                         │
│  Serviço     [___________________]       │
│  Preço       [R$ ____]                   │
│  Periodicidade (•) Mensal ( ) Anual      │
│  Vencimento  [dia __]                    │
│  Tipo        (•) Pessoal ( ) Compartilhada│
│  [Salvar]                                │
└─────────────────────────────────────────┘
```

### Tela 3.2 — Dashboard do gestor
```
┌─────────────────────────────────────────┐
│  Gasto mensal: R$ 187,40                 │
│  Projeção anual: R$ 2.248,80             │
│  Economia acumulada: R$ 340,00           │
├─────────────────────────────────────────┤
│  Pessoais (4)        Compartilhadas (3)  │
│  Netflix   R$55,90    Spotify  R$12,00   │
│  iCloud+   R$10,00    Google One R$8,00  │
├─────────────────────────────────────────┤
│  ⚠ Possível sobreposição: 2 serviços de  │
│    streaming de música ativos            │
│  [Ver oportunidades de economia]         │
└─────────────────────────────────────────┘
```

### Tela 3.3 — Grupos que participo / administro
```
┌─────────────────────────────────────────┐
│  Grupos que participo (2)                │
│    Netflix Família — Ativo               │
│  Grupos que administro (1)                │
│    Spotify Duo — Saldo a receber: R$12,00│
└─────────────────────────────────────────┘
```

---

## Jornada 4 — Falha ou encerramento (seção 5.4)

`Problema reportado → bloqueio de repasse → administrador notificado → coleta de evidências → solução/estorno/realocação → registro no histórico → eventual sanção`

### Tela 4.1 — Reportar problema
```
┌─────────────────────────────────────────┐
│  Reportar problema — Netflix Família     │
│  Motivo (•) Acesso não fornecido         │
│         ( ) Acesso removido              │
│         ( ) Serviço cancelado            │
│         ( ) Plano diferente do anunciado │
│         ( ) Cobrança incorreta           │
│         ( ) Outro                        │
│  Descrição [___________________________] │
│  Evidências [Anexar arquivo]             │
│  [Abrir disputa]                         │
└─────────────────────────────────────────┘
```

### Tela 4.2 — Acompanhar disputa (participante e administrador)
```
┌─────────────────────────────────────────┐
│  Disputa #567 — Aberta há 2 dias         │
│  Status: aguardando resposta do admin    │
│  ⚠ Repasse deste ciclo está bloqueado    │
│  Linha do tempo:                         │
│   • 10/10 — Chamado aberto               │
│   • 10/10 — Administrador notificado     │
│   • Aguardando evidências (prazo: 3 dias)│
│  [Enviar evidência]  [Ver política]      │
└─────────────────────────────────────────┘
```

### Tela 4.3 — Resultado da disputa
```
┌─────────────────────────────────────────┐
│  Disputa #567 — Encerrada                │
│  Resultado: Estorno parcial + realocação │
│  ⚠ Este caso foi registrado no histórico │
│    de reputação das partes envolvidas    │
│  [Ver grupos compatíveis]                │
└─────────────────────────────────────────┘
```

---

## Notas de consistência entre jornadas

- Toda tela de checkout/pagamento precisa exibir preço + taxa **antes** da confirmação (regra do marketplace, seção 12) — telas 1.6 já refletem isso.
- Toda tela de disputa precisa deixar claro que o repasse pode ser bloqueado — reforça a seção 6 do fluxo financeiro.
- Selos (Identidade verificada / Pro / Confiança) devem aparecer sempre com o mesmo padrão visual e nunca misturados, para não sugerir que "Pro" é garantia de confiança (seção 7, "leitura dos selos").
- Nenhuma tela aqui assume arquitetura técnica — isso é decisão pendente e não deve ser inferido do wireframe.

## Próxima ação

Usar estes wireframes como roteiro do protótipo clicável da Etapa 2 (Fase 3 do plano de validação — "Protótipo: testar jornadas, pagamento antecipado, repasse, selos e disputa antes do desenvolvimento").
