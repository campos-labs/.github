# Governança e Fluxo de Trabalho

Engenharia orientada à simplicidade, rastreabilidade e entregas demonstráveis. Processos assíncronos proporcionais ao risco técnico.

## 1. Fase de Descoberta e Arquitetura (`project-hub`)

Fase dedicada à ideação (início opcional em *Discussions*), validações e decisões pré-implementação, estruturada por tipos de issue:

- **`RFC`:** Issue coordenadora que amadurece a proposta, seus limites e a arquitetura inicial registrada no `DESIGN.md`.
- **`POC`:** Valida a hipótese técnica focada; `research/` concentra o código necessário e evidências explicadas.
- **`Spike`:** Compara alternativas, investiga trade-offs e reduz incertezas antes da decisão.
- **`ADR`:** Registra a decisão baseada em evidências, define o recorte adotado e atualiza o `DESIGN.md` quando a arquitetura muda.
- **`Epic`:** Mapeia e coordena capacidades amplas; pode ser subissue temporária da RFC para registrar escopos adiados.

Aprovada a RFC (via *poll*), o produto ganha repositório dedicado, `DESIGN.md` e Epics podem ser transferidos, e a RFC é encerrada.

## 2. Fase de Execução e Releases (Repositório Dedicado)

No novo repositório, o `DESIGN.md` representa a arquitetura vigente e os milestones agrupam o trabalho planejado para cada release.

**Tipos de Issue de Execução:**

- **`FEAT`:** Entrega capacidade funcional; **`FIX`:** corrige defeito ou regressão; **`DOC`:** cria ou atualiza documentação.
- **`CHORE`:** Cobre configuração, infraestrutura e automação; **`REFACTOR`:** melhora a estrutura sem alterar o comportamento esperado.
- **`TEST`:** Trabalho exclusivo de testes; **`PERF`:** otimizações mensuráveis de desempenho. Complementares, adotados sob demanda.

**Regras da Release:**

- **Hierarquia:** `Epic` coordena subissues da versão; Issues de execução dispensam pai quando o milestone já fornece o contexto.
- **Integração:** A `main` é protegida; cada Issue folha gera, em regra, um PR principal, que usa `Closes #ID` e passa por revisão.
- **Qualidade:** `CODEOWNERS` apoia a revisão; CI verde é recomendada quando houver checks configurados (ex.: `pytest` e `ruff`).
- **Release:** Milestones são atribuídos às Issues. Após a validação do escopo, a versão recebe uma tag e uma GitHub Release.

```mermaid
flowchart LR
    D[Discussion] --> R[RFC]
    R --> P[POC e Spike]
    P --> A[ADR]
    A --> G[DESIGN]
    A -. escopo adiado .-> E[Epic]
    A -. futuro/incerto .-> D
    G --> X[Produto]
    E -. transfere .-> X
    X --> M[Milestone]
    M --> I[Issues]
    I --> PR[PR e CI]
    PR --> V[Release]
