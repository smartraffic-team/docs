# Alternância por Inatividade

## Situação atual

- quando não há medição válida, o plano recua para ciclo fixo;
- sem comando válido por watchdog, firmware entra em fallback local.

## Efeito prático

- evita travamento de semáforo por falha de câmera/API;
- mantém atendimento periódico das vias.

## Cuidados operacionais

- monitorar estado serial e pendências de comando;
- validar tempos de fallback em testes físicos.
