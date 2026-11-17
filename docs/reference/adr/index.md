# Decisões de Arquitetura (ADR)

## ADR-001 — Controle local primeiro
Decisão: semáforo é decidido localmente em Python/Arduino.

## ADR-002 — API como persistência e distribuição
Decisão: API não controla LED físico; apenas registra e serve dados.

## ADR-003 — Fila persistente para ingestão
Decisão: uso de SQLite local para reenvio e resiliência sem bloquear controle.

## ADR-004 — Via sem medição não gera demanda fictícia
Decisão: ausência de câmera/medição não é tratada como zero de tráfego.
