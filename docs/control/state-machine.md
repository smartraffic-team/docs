# Máquina de Estados do Semáforo

Estados firmware observados:

- `A_GREEN`
- `A_YELLOW`
- `ALL_RED`
- `B_GREEN`
- `B_YELLOW`

Transição segura padrão:

```mermaid
stateDiagram-v2
  [*] --> ALL_RED
  ALL_RED --> A_GREEN
  A_GREEN --> A_YELLOW
  A_YELLOW --> ALL_RED
  ALL_RED --> B_GREEN
  B_GREEN --> B_YELLOW
  B_YELLOW --> ALL_RED
```

No Python (`traffic.py`), o plano define durações de verde A/B; o firmware executa a transição física.
