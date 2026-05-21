# Architecture

How a keystroke becomes a commit.

```mermaid
flowchart LR
  A[You type] --> B[(IndexedDB)]
  B --> C{Online?}
  C -- yes --> D[Batch into one commit]
  C -- no --> E[Queue on device]
  E --> D
  D --> F[(Your GitHub repo)]
```

See [[deploy-runbook]] for how it ships.
