---
name: Project Bootstrap
about: Promover uma RFC aprovada para um repositório dedicado
title: "Project Bootstrap"
labels: ""
assignees: ""
type: Chore
---

<!--
Criar no project-hub como subissue da RFC somente após sua priorização na Discussion.
Definir blocked by pelo ADR e pela priorização quando aplicável.
Transferir esta CHORE antes de abrir o PR de bootstrap.
Desvincular a Epic da RFC antes de transferi-la; ela permanecerá aberta no produto.
-->

## Objetivo

Promover a RFC aprovada para um repositório dedicado usando o template técnico aplicável.

## Lista de tarefas (reaproveitar no PR)

- [ ] **Pré-condições:** Confirmar priorização (Discussion), ADR concluído e `DESIGN.md` atualizado.
- [ ] **Repositório:** Criar pelo template aplicável. Definir nome, visibilidade, descrição e tópicos.
- [ ] **Transferências:** Mover esta CHORE e a Epic para o produto. Conferir Project, Type, Status e dependências.
- [ ] **Conteúdo:** Adaptar placeholders. Incorporar `DESIGN.md`, protótipo, fixtures e artefatos pertinentes.
- [ ] **Governança:** Aplicar ruleset, CI, merges, auto-merge, exclusão de branches e permissões do Actions.
