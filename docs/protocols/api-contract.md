# Contrato da API

## Autenticação

- usuários: `Authorization: Bearer <token>`
- ingestão: `x-ingestion-key`

## Recursos principais da ingestão

- `POST /api/v1/leituras`
- `POST /api/v1/historico-fases`
- `POST /api/v1/telemetria`

## Princípios

- usar timestamps UTC ISO 8601;
- enviar UUID estável em reenvios de leitura;
- enviar somente campos medidos;
- nunca enviar segredos ao frontend.
