# Projeto Split — Documento Mestre do Produto

**Marketplace de grupos e gestão inteligente de assinaturas**

| Campo | Valor |
|---|---|
| Versão | 1.0 |
| Data | 19 de setembro de 2026 |
| Responsável | Felipe Júdice |
| Status | Concepção e validação |

> Nome interno provisório. Nome comercial, cores, tipografia e símbolo serão definidos após a validação do posicionamento e do modelo.

## Como usar este documento

Este documento organiza as decisões já tomadas, as hipóteses ainda não comprovadas e os pontos que exigem validação antes do desenvolvimento. Ele serve como base para conversas com produto, design, tecnologia, jurídico, parceiros de pagamento e possíveis investidores.

| Categoria | Significado | Tratamento |
|---|---|---|
| Decisão aprovada | Direção definida para o projeto | Preservar no MVP ou justificar alteração |
| Hipótese | Suposição que precisa de evidência | Testar com usuários e números |
| Validação obrigatória | Tema jurídico, financeiro ou técnico | Não lançar antes de confirmar |

## Resumo executivo

O Projeto Split será uma plataforma digital que reúne marketplace de grupos, organização de assinaturas e pagamentos protegidos. A proposta é ajudar usuários a visualizar seus gastos recorrentes, encontrar oportunidades permitidas de compartilhamento, administrar cobranças e reduzir riscos entre participantes e administradores.

> **Proposta de valor provisória:** Todas as suas assinaturas em um só lugar. Compartilhe quando puder. Economize quando quiser.

O produto não deve ser apresentado apenas como um site para dividir serviços de streaming. A visão mais forte é a de uma plataforma de gestão inteligente de assinaturas. O marketplace atrai usuários, o gestor financeiro aumenta a recorrência de uso, o fluxo protegido cria confiança e a reputação melhora a qualidade da oferta.

## 1. Visão estratégica

### 1.1 Problema

As pessoas acumulam assinaturas de entretenimento, armazenamento, produtividade, educação e software sem uma visão clara do gasto total. Quando dividem uma assinatura, a administração costuma acontecer por mensagens, Pix e planilhas, gerando atrasos, falta de transparência, cancelamentos inesperados e conflitos.

- Dificuldade para enxergar o gasto mensal e anual consolidado.
- Inadimplência e cobranças manuais em grupos compartilhados.
- Falta de reputação e histórico verificável entre desconhecidos.
- Risco de perda de acesso, troca de senha ou encerramento do grupo.
- Pouca clareza sobre quais planos podem ser compartilhados e em quais condições.

### 1.2 Oportunidade

Existe espaço para reunir descoberta, organização, cobrança e acompanhamento financeiro em uma única experiência. A oportunidade é maior quando o produto continua útil mesmo depois que o usuário encontra um grupo, pois o painel de gastos e economia cria motivo para retornar.

### 1.3 Visão

Ser uma referência brasileira em gestão e compartilhamento responsável de assinaturas, transformando gastos recorrentes dispersos em decisões financeiras mais claras.

### 1.4 Missão

Ajudar pessoas e pequenos grupos a organizar assinaturas, economizar quando o compartilhamento for permitido e realizar pagamentos recorrentes com mais previsibilidade e proteção.

## 2. Públicos prioritários

| Público | Necessidade principal |
|---|---|
| Participante | Busca uma vaga em serviço elegível e valoriza economia, simplicidade e segurança. |
| Administrador de grupo | Possui uma assinatura com vagas e precisa receber, organizar participantes e demonstrar confiabilidade. |
| Organizador privado | Já divide despesas com pessoas conhecidas e quer centralizar cobrança e controle. |
| Usuário do gestor | Deseja acompanhar todas as assinaturas, mesmo sem participar do marketplace. |
| Pequenas equipes | Público futuro para licenças empresariais ou de equipe formalmente permitidas. |

## 3. Pilares do produto

### 3.1 Marketplace de grupos

Ambiente de descoberta de grupos públicos com vagas disponíveis. O usuário poderá comparar serviço, preço, quantidade de vagas, reputação do administrador, tempo de atividade e condições de entrada.

### 3.2 Grupos privados

Grupos acessíveis somente por convite para famílias, amigos, colegas ou equipes que já se conhecem. A modalidade usa a estrutura de cobrança e organização da plataforma, sem aparecer no marketplace.

### 3.3 Gestor de assinaturas

Painel para registrar serviços pessoais e compartilhados, acompanhar vencimentos e visualizar o impacto financeiro.

- Gasto total mensal e projeção anual.
- Separação entre assinaturas pessoais e compartilhadas.
- Economia estimada e acumulada.
- Datas de cobrança e histórico de reajustes.
- Possíveis sobreposições ou serviços pouco utilizados.
- Grupos que participa, grupos que administra e saldo a receber.

### 3.4 Pagamento protegido

A plataforma controla cobrança, agenda de repasse, bloqueios e estornos dentro das capacidades do parceiro de pagamentos. O dinheiro não deve ser repassado imediatamente ao administrador quando isso reduzir a proteção do participante.

### 3.5 Reputação e confiança

A confiança será construída por identidade validada, histórico, avaliações e indicadores de risco. Um plano pago poderá comprar recursos e visibilidade, mas nunca deverá ser comunicado como garantia de honestidade.

## 4. Modelo de grupos

### 4.1 Grupo público

- Aparece no marketplace.
- Exige identidade verificada do administrador.
- Exibe preço, vagas, regras e condições de saída.
- Fica sujeito a moderação, reputação e limites operacionais.

### 4.2 Grupo privado

- É acessível por convite ou link.
- Não aparece na busca pública.
- Continua sujeito às regras de pagamento e uso aceitável.
- Não autoriza compartilhamento que contrarie regras do fornecedor.

### 4.3 Elegibilidade de serviços

Cada serviço deverá possuir uma ficha interna atualizada antes de aparecer na plataforma.

- Tipo de plano e quantidade de membros.
- Requisitos de residência, família, equipe ou organização.
- Possibilidade ou proibição de revenda.
- Regras territoriais e forma de convite.
- Riscos de bloqueio.
- Fonte oficial consultada e data da última revisão.

> **Regra de lançamento:** Nenhum serviço entra no marketplace apenas por ser popular. A modalidade precisa ser analisada e aprovada.

## 5. Jornadas principais

### 5.1 Entrada de participante

Criar conta → confirmar contatos → verificar identidade quando exigido → buscar serviço → analisar grupo → aceitar regras → pagar entrada → receber instruções → confirmar funcionamento → acompanhar cobrança → avaliar experiência.

### 5.2 Criação de grupo

Criar conta → verificar identidade → cadastrar recebimento no mesmo CPF ou CNPJ → selecionar serviço elegível → informar plano, preço, vagas e regras → comprovar assinatura quando necessário → passar por análise → publicar → receber participantes → manter acesso → receber repasses.

### 5.3 Gestão financeira

Cadastrar assinatura → informar preço, periodicidade e vencimento → classificar como pessoal ou compartilhada → acompanhar totais → receber alertas → revisar gastos e oportunidades de economia.

### 5.4 Falha ou encerramento

Problema reportado → possível bloqueio de repasse → administrador notificado → coleta de evidências → solução, estorno ou realocação → registro no histórico → eventual sanção.

## 6. Sistema de pagamento e proteção

### 6.1 Regra conceitual aprovada

Na entrada em um grupo público, o participante paga duas mensalidades antecipadas, além da taxa da plataforma. A primeira cobre o período inicial. A segunda funciona como cobertura do ciclo seguinte ou reserva operacional, conforme a estrutura final. O administrador recebe com defasagem de um ciclo, desde que o acesso permaneça válido e não exista disputa relevante aberta.

| Momento | Participante | Plataforma | Administrador |
|---|---|---|---|
| Entrada | Paga 2 mensalidades + taxa | Registra e separa valores | Fornece acesso |
| Durante o ciclo | Usa e reporta problemas | Monitora e recebe disputas | Mantém serviço ativo |
| Ciclo seguinte | Passa à cobrança mensal | Libera conforme regras | Recebe o ciclo anterior |
| Se houver falha | Solicita solução | Pode bloquear repasse | Responde e comprova |

### 6.2 Exemplo ilustrativo

> **Exemplo:** Cota mensal de R$ 20,00. Entrada de R$ 40,00 mais a taxa. O repasse ao administrador ocorre posteriormente, conforme calendário e ausência de bloqueios.

### 6.3 Controles mínimos

- Prazo de segurança antes do primeiro saque.
- Bloqueio de repasse durante disputa qualificada.
- Conta de recebimento vinculada ao titular verificado.
- Histórico de cobranças, estornos e repasses.
- Política clara para a segunda mensalidade em cada cenário.
- Tratamento de chargeback e saldo negativo.
- Limites progressivos para contas novas.
- Proibição de cobrança externa em grupos públicos.
- Conciliação financeira e trilha de auditoria.

### 6.4 Condicionante obrigatória

A plataforma não deve prometer custódia ou escrow sem que o arranjo seja suportado pelo provedor de pagamentos e validado juridicamente. Split de pagamento, agenda de repasse e retenção não são automaticamente a mesma coisa.

### 6.5 Substituição assistida

Quando um grupo for encerrado, a plataforma poderá oferecer opções compatíveis antes do reembolso. A migração depende de consentimento claro do usuário e compatibilidade de preço, serviço e regras.

## 7. Identidade, plano pago e reputação

### 7.1 Identidade verificada

Indica que dados como CPF ou CNPJ, documento, telefone, selfie quando aplicável e titularidade do recebimento foram validados. Não representa garantia de comportamento futuro.

### 7.2 Administrador Pro

Plano mensal pago voltado a visibilidade e ferramentas. Pode usar uma estrela, desde que a comunicação deixe claro que se trata de um benefício comercial.

- Destaque visual no perfil e nos grupos.
- Maior exposição no marketplace, identificada como destaque.
- Mais grupos simultâneos.
- Dados de visualizações e conversão.
- Suporte prioritário.
- Ferramentas adicionais de gestão.
- Acesso antecipado a funcionalidades.
- Possível redução de taxa, condicionada à simulação financeira.

> Hipótese inicial de preço: R$ 19,90 a R$ 29,90 por mês. O valor não está aprovado e deverá ser testado.

### 7.3 Administrador de confiança

Reconhecimento conquistado por histórico, não comprado. Os critérios poderão considerar tempo de atividade, ciclos concluídos, avaliação, taxa de cancelamento, disputas procedentes e tempo de resposta.

> **Leitura dos selos:** Identidade verificada significa que sabemos quem é. Administrador Pro significa que paga por recursos. Administrador de confiança significa que possui histórico positivo comprovado.

## 8. Modelo de receita

| Fonte | Descrição |
|---|---|
| Taxa de serviço | Aplicada às transações; pode combinar valor fixo mínimo e percentual. |
| Administrador Pro | Assinatura recorrente para exposição e ferramentas de gestão. |
| Gestor Premium | Plano futuro com relatórios, alertas e recomendações avançadas. |
| B2B e parceiros | Possibilidades futuras para equipes e ofertas oficiais autorizadas. |

A taxa final depende de custos de pagamento, impostos, chargebacks, prevenção a fraude, atendimento e margem. Destaque pago nunca poderá se passar por avaliação de confiança.

## 9. Escopo do MVP 1.0

### 9.1 Funcionalidades essenciais

- Cadastro, login e confirmação de contatos.
- Perfil e verificação de identidade do administrador.
- Marketplace com busca e filtros básicos.
- Página detalhada do grupo.
- Criação de grupos públicos e privados.
- Solicitação ou entrada no grupo.
- Checkout e cobrança recorrente.
- Calendário e status de repasses.
- Grupos que participo e grupos que administro.
- Cadastro manual de assinaturas.
- Dashboard de gasto mensal, anual e economia.
- Notificações essenciais.
- Avaliações e disputas.
- Painel administrativo interno.
- Termos, políticas e consentimentos.

### 9.2 Fora do primeiro lançamento

- Aplicativos nativos Android e iOS.
- Dezenas de categorias.
- Inteligência artificial complexa.
- Conexão automática com todas as contas bancárias.
- Marketplace internacional.
- Plano B2B completo.
- Migração automática sem confirmação.
- Automações sofisticadas antes de existir volume real.

> **Formato do MVP:** Site responsivo, com arquitetura preparada para evoluir posteriormente para PWA ou aplicativo.

## 10. Funcionalidades futuras

- Alertas de aumento de preço.
- Detecção de assinaturas sobrepostas.
- Recurso "Otimizar minhas assinaturas".
- Importação por Open Finance, se viável e autorizada.
- Previsão anual de despesas.
- Migração assistida entre grupos.
- Lista de espera por serviço.
- Programa de indicação.
- Plano Premium do gestor.
- Contas empresariais e relatórios exportáveis.
- Aplicativo móvel.
- Integração com ofertas oficiais de fornecedores.

## 11. Mapa de telas

| Área | Telas principais |
|---|---|
| Pública | Home; Como funciona; Marketplace; Categoria; Grupo; Segurança; Preços; Dúvidas; Entrar; Criar conta; Termos. |
| Participante | Dashboard; Minhas assinaturas; Grupos; Cobranças; Economia; Notificações; Avaliações; Disputas; Perfil. |
| Administrador | Criar grupo; Meus grupos; Vagas; Participantes; Cobranças e repasses; Estatísticas; Pro; Reputação; Suporte. |
| Operação interna | Usuários; Verificações; Catálogo; Grupos; Transações; Disputas; Fraudes; Atendimento; Métricas; Auditoria. |

## 12. Regras iniciais do marketplace

- Somente serviços previamente aprovados poderão ser cadastrados.
- O administrador deverá declarar corretamente a modalidade do plano.
- Credenciais pessoais não serão expostas publicamente.
- Grupos públicos exigirão identidade validada.
- Preço e taxa serão apresentados antes do pagamento.
- O administrador deverá manter o acesso durante o período pago.
- O participante deverá respeitar os limites e regras do grupo.
- Cobrança fora da plataforma poderá gerar bloqueio.
- Avaliações estarão vinculadas a experiências reais.
- Contas novas terão limites menores.
- Fraude ou falsificação poderá resultar em suspensão.
- Regras de estorno informarão prazos, elegibilidade e destino da reserva.

## 13. Disputas, cancelamentos e reembolsos

### 13.1 Motivos de disputa

- Acesso não fornecido.
- Acesso removido antes do fim do período.
- Serviço cancelado.
- Plano diferente do anunciado.
- Cobrança incorreta.
- Comportamento abusivo.
- Uso incompatível com as regras pelo participante.

### 13.2 Fluxo inicial

1. Usuário abre chamado e informa o motivo.
2. O sistema preserva registros e avalia o bloqueio do repasse.
3. A outra parte é notificada.
4. As partes enviam respostas e evidências dentro do prazo.
5. O atendimento decide conforme política publicada.
6. O resultado pode incluir correção, crédito, realocação, estorno, liberação ou sanção.
7. O caso alimenta o histórico de risco e reputação.

A política final deverá ser compreensível antes do pagamento e detalhada o suficiente para sustentar decisões consistentes.

## 14. Segurança, privacidade e prevenção a fraudes

- Autenticação segura e confirmação de contatos.
- Verificação de identidade proporcional ao risco.
- Criptografia em trânsito e em repouso.
- Segregação de permissões e logs de ações sensíveis.
- Limitação de tentativas e detecção de múltiplas contas.
- Monitoramento de comportamento suspeito respeitando a privacidade.
- Política de retenção e descarte de dados.
- Plano de resposta a incidentes.
- Backups, recuperação e revisão de acessos internos.

A plataforma deverá seguir o princípio da minimização: coletar somente os dados necessários para operação, segurança e obrigações legais.

## 15. Riscos críticos

| Risco | Impacto e cuidado |
|---|---|
| Termos dos fornecedores | Planos de família, residência, equipe e organização possuem regras diferentes e podem mudar. |
| Estrutura financeira | Reter valores, formar reservas e controlar repasses exige desenho jurídico, contábil e técnico adequado. |
| Chargeback e fraude | Dois meses antecipados reduzem alguns riscos, mas não eliminam contestações tardias e saldo negativo. |
| Proteção ao consumidor | Preço, renovação, taxa, cancelamento e responsabilidades precisam ser transparentes. |
| LGPD | CPF, documento, selfie e dados financeiros exigem base legal, segurança e governança. |
| Concentração | Mudanças de regra em poucas marcas podem afetar grande parte do negócio. |
| Liquidez | Muitas categorias com poucos usuários criam um marketplace vazio. |

## 16. Hipóteses a validar

- Usuários aceitam pagar duas mensalidades na entrada.
- A percepção de proteção compensa o desembolso inicial maior.
- Administradores aceitam receber com um ciclo de atraso.
- Existe disposição para pagar o Administrador Pro.
- O gestor é usado mesmo por quem não participa de grupos.
- O cálculo de economia aumenta a retenção.
- Cinco a oito categorias criam liquidez inicial suficiente.
- A substituição assistida reduz cancelamentos.
- A taxa cobre custos sem tornar a oferta pouco atraente.
- O negócio pode operar com modalidades compatíveis com as regras dos fornecedores.

## 17. Métricas do negócio

### 17.1 Aquisição
Visitantes, cadastros, origem, custo por cadastro e conversão da landing page.

### 17.2 Marketplace
Grupos, vagas, tempo para preencher, conversão em entrada, categorias mais demandadas e solicitações sem oferta.

### 17.3 Operação e confiança
Sucesso de pagamento, inadimplência, chargebacks, disputas por cem transações, tempo de resolução, cancelamentos e grupos encerrados.

### 17.4 Retenção e receita
Usuários ativos, retenção por coorte, volume transacionado, receita líquida, receita média, adesão e cancelamento do Pro e economia percebida.

## 18. Plano de validação

| Fase | Objetivo |
|---|---|
| 1. Descoberta | Entrevistar participantes e administradores sobre hábitos, receios, gastos e aceitação das regras. |
| 2. Landing page | Captar interessados e medir quais assinaturas desejam organizar ou compartilhar. |
| 3. Protótipo | Testar jornadas, pagamento antecipado, repasse, selos e disputa antes do desenvolvimento. |
| 4. Piloto controlado | Operar com poucas categorias aprovadas, limites conservadores e suporte próximo. |
| 5. Decisão | Investir em desenvolvimento robusto somente após evidências de demanda e viabilidade. |

> **Meta inicial sugerida:** Conseguir 100 interessados qualificados em duas a três semanas. A meta orienta aprendizado; sozinha, não prova viabilidade.

## 19. Roadmap proposto

1. **Fundamentos** — Documento mestre, pesquisa, entrevistas, análise jurídica, parceiro financeiro e matriz de serviços.
2. **Produto** — Arquitetura de informação, wireframes, protótipo, testes e revisão das regras.
3. **Validação comercial** — Landing page, lista de espera, conteúdo, pesquisa de demanda e comunidade inicial.
4. **MVP** — Desenvolvimento web, integrações, painel interno, segurança e piloto fechado.
5. **Lançamento controlado** — Poucas categorias, limites, suporte manual e acompanhamento diário.
6. **Marca definitiva** — Nome, domínio, identidade, cores, tipografia, símbolo e linguagem, com pesquisa de disponibilidade.

## 20. Decisões consolidadas

- Nome interno: Projeto Split.
- Produto combina marketplace e gestor de assinaturas.
- Haverá grupos públicos e privados.
- O usuário verá gasto mensal, anual e economia.
- A entrada no grupo público parte de duas mensalidades antecipadas.
- O administrador recebe com defasagem e sujeito a regras de segurança.
- Haverá Identidade Verificada.
- Haverá plano pago Administrador Pro, identificado de forma comercial.
- Haverá reputação conquistada por desempenho.
- O MVP será web responsivo.
- A marca definitiva será criada depois da estruturação e validação inicial.

## 21. Decisões pendentes

- Serviços e categorias do piloto.
- Taxa transacional.
- Preço e benefícios finais do Pro.
- Parceiro de pagamento.
- Prazos exatos de liberação.
- Destino da segunda mensalidade em cada cenário.
- Critérios de reembolso e cancelamento.
- Exigências de verificação para participantes.
- Critérios de publicação e documentos aceitos.
- Responsabilidade por reajustes.
- Critérios do reconhecimento de confiança.
- Política de avaliações e suporte.
- Arquitetura técnica.
- Nome comercial e identidade visual.

## 22. Próximos passos prioritários

1. Criar a matriz de serviços e verificar modalidades aptas ao piloto.
2. Desenhar o fluxo financeiro completo: entrada, renovação, repasse, estorno, chargeback e encerramento.
3. Consultar especialista jurídico em marketplace, pagamentos, consumidor, contratos e LGPD.
4. Conversar com provedores de pagamento sobre recebedores, split, agenda de repasses e reservas.
5. Entrevistar potenciais usuários e administradores.
6. Definir a landing page e o formulário de interesse.
7. Criar wireframes das jornadas críticas.
8. Simular a economia unitária antes de definir preços.
9. Planejar um piloto fechado.
10. Desenvolver a marca definitiva depois dessas validações.

## 23. Critérios para avançar ao desenvolvimento

- Demanda concentrada em categorias elegíveis.
- Participantes compreendem e aceitam o pagamento inicial.
- Administradores aceitam as regras de repasse.
- O parceiro financeiro suporta o fluxo.
- O risco jurídico é administrável.
- A taxa projetada cobre os custos.
- O protótipo é compreendido sem explicação excessiva.
- Existe plano operacional para suporte, fraude e disputas.

## Conclusão

O Projeto Split tem potencial para ocupar uma posição mais ampla do que um marketplace de vagas. A combinação de gestão financeira, grupos públicos e privados, pagamentos protegidos e reputação cria uma proposta recorrente e defensável.

O principal risco seria começar pelo código antes de validar as regras. O valor do projeto dependerá da compatibilidade com os serviços oferecidos, da segurança do fluxo financeiro e da capacidade de criar confiança. O próximo investimento deve ser a validação com usuários, jurídico e parceiros de pagamento.

> **Aviso:** Este documento é estratégico e não substitui parecer jurídico, contábil, tributário, regulatório ou de segurança da informação. Valores, serviços citados e regras operacionais permanecem hipóteses até validação formal.
