# Architecture

```mermaid
flowchart LR
  U[User] -->|Query| O[Orchestrator]
  O --> M[MarketAgent]
  O --> N[NewsAgent]
  O --> F[FilingsAgent]
  M --> E[Evaluator]
  N --> E
  F --> E
  E --> R[Unified Report Bundle]
