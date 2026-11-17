# Serial Python ↔ Arduino (ST1)

Formato base:

- Comandos: `AUTO {seq} {a_ms} {b_ms}`, `MANUAL {seq} {A|B}`, `KEEP {seq}`
- Estado: `STATE ST1 seq phase elapsed_ms duration_ms mode target`

## Regras de validação

- fases permitidas: `A_GREEN`, `A_YELLOW`, `B_GREEN`, `B_YELLOW`, `ALL_RED`;
- timeout serial do controlador: 2 s;
- sem resposta/ACK: controle marca indisponível e interrompe comandos.

## Segurança operacional

- watchdog do firmware mantém ciclo local sem Python;
- transições aceitas completam amarelo/all-red antes de nova troca.
