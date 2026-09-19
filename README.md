# Projeto Split

Marketplace de grupos e gestão inteligente de assinaturas.

> Nome interno provisório. Nome comercial, identidade visual e domínio serão definidos após a validação do posicionamento e do modelo (ver [Etapa 6 do roadmap](docs/documento-mestre.md#19-roadmap-proposto)).

## Status atual: Concepção e validação (Etapa 1 — Fundamentos)

Este repositório ainda não contém código de produto. Antes de desenvolver, o próprio [Documento Mestre](docs/documento-mestre.md) recomenda validar hipóteses de demanda, viabilidade jurídica e viabilidade financeira. Ver a conclusão do documento:

> "O principal risco seria começar pelo código antes de validar as regras."

## Protótipo navegável

Um protótipo clicável de baixa/média fidelidade das 4 jornadas críticas (entrada de participante, criação de grupo, gestão financeira, disputa/encerramento) está disponível em [`prototipo/index.html`](prototipo/index.html) — abra o arquivo em qualquer navegador. Sem identidade visual definitiva de propósito.

Versão hospedada para visualização rápida: https://claude.ai/artifact/LC1q3JBd4qveHEcwf3DYDf

## Estrutura do repositório

```
docs/
  documento-mestre.md        Documento mestre completo do produto (v1.0)
  decisoes-pendentes.md      Lista de decisões que ainda faltam ser tomadas
  proximos-passos.md         Checklist acionável da Etapa 1 (Fundamentos)
  roadmap.md                 As 6 etapas do roadmap, com critérios de avanço
  matriz-servicos.md         Rascunho de serviços candidatos ao piloto
  fluxo-financeiro.md        Rascunho do fluxo financeiro completo (entrada, repasse, disputa, estorno)
  wireframes.md              Wireframes de baixa fidelidade das jornadas críticas
prototipo/
  index.html                 Protótipo navegável (HTML/CSS/JS puro, sem build)
```

## Como contribuir com este momento do projeto

1. Leia o [Documento Mestre](docs/documento-mestre.md) por completo — ele é a fonte da verdade sobre visão, público, modelo financeiro, riscos e escopo do MVP.
2. Trate toda "decisão aprovada" nele como ponto de partida, não como imutável: mudanças exigem justificativa registrada.
3. Trate toda "hipótese" como algo a testar com usuários e números antes de virar decisão.
4. Não implemente nada rotulado como "validação obrigatória" (jurídico, financeiro, técnico) sem confirmação formal.
5. Acompanhe [decisoes-pendentes.md](docs/decisoes-pendentes.md) e [proximos-passos.md](docs/proximos-passos.md) para saber o que falta antes de avançar de etapa.

## Próxima etapa

Ver [docs/proximos-passos.md](docs/proximos-passos.md) para as ações prioritárias da Etapa 1 (Fundamentos): matriz de serviços elegíveis, fluxo financeiro completo, consulta jurídica, conversa com parceiros de pagamento, entrevistas com usuários — a maior parte já iniciada, o restante depende de conversas humanas reais (jurídico, parceiro de pagamento, usuários).
