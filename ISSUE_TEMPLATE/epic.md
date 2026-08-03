---
name: Epic — Evolução planejada pós-v1.0
about: Preservar capacidades planejadas e desdobrá-las sob demanda
title: ""
labels: ""
assignees: ""
type: Epic
---

<!--
Durante a descoberta:
- Criar no project-hub como subissue da RFC.
- Definir blocked by pelo ADR quando aplicável.

Durante o Bootstrap:
- Remover o vínculo Parent com a RFC.
- Transferir a Epic aberta para o repositório do produto.
- Conferir Project, Type, Status e dependências após a transferência.
- Vincular Milestones somente às subissues quando entrarem no planejamento; manter a Epic sem Milestone.

Para cada capacidade:
- Usar uma tarefa principal com objetivo ou resultado esperado.
- Manter as tarefas internas sem recuo dentro de <details> para preservar Convert to issue.
- Tratar itens sem prefixo como entregas previstas; ao criar a Issue, atribuir o Type FEAT.
- Identificar POC e Spike somente quando houver pesquisa real.
- Preservar a descrição completa até criar a Issue.
- Converter em Issue, vincular como subissue e substituir a linha por #ID — título.
- Referenciar no RADAR somente quando existir uma Discussion aplicável.
-->

## Objetivo

Preservar as capacidades planejadas após a arquitetura inicial e convertê-las em subissues (FEAT, POC ou Spike) conforme avancem. Encerrar quando todas forem entregues, encerradas como não planejadas ou movidas ao [Discussion](<URL_DA_DISCUSSION>) .
## Capacidades

- [ ] **[capacidade]** — [objetivo ou resultado esperado].

<details>
<summary>&nbsp;&nbsp;&nbsp;&nbsp;<i>Desdobramentos</i></summary>

- [ ] **[entrega]** — [ação e resultado esperado].
- [ ] **POC · [hipótese]** — [viabilidade a demonstrar].
- [ ] **SPIKE · [decisão]** — [alternativas e critérios a comparar].

</details>
