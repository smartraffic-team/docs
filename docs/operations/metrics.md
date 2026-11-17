# Métricas e Contadores

## Coletadas localmente

- carros e pessoas por via;
- veículos parados estimados;
- tempo de espera mais antigo por via;
- estratégia ativa (`adaptativo`, `prioridade_via_a`, `prioridade_via_b`, `ciclo_fixo`).

## Persistidas na API

- leituras `QUADRO`;
- histórico de fases;
- telemetria de dispositivos.

## Interpretação correta

- contagem por quadro não representa veículos únicos;
- `0` é medição válida sem objeto;
- `null/—` é indisponível.
