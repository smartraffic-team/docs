# Fluxo de Dados

## Fluxo online

1. `smarttraffic_app.py` captura frames A/B.
2. `vision.py` detecta carros/pessoas e calcula estado de medição.
3. `traffic.py` calcula tempos de verde e envia comandos ST1 ao Arduino.
4. `ingestion.py` grava eventos na fila SQLite e envia para API.
5. API grava leituras/fases/telemetria no MySQL.
6. Plataforma consulta API e exibe dashboards.

## Fluxo com falha de API

- controle local continua ativo;
- fila local acumula pendências;
- reenvio ocorre quando API volta.

## Fluxo com falha de câmera

- via sem medição não gera demanda fictícia;
- controlador usa estratégia/fallback conforme estado válido disponível.
