# API de Integração

Local: `api/` (NestJS + Prisma)

## Papel

- autenticação JWT para usuários;
- ingestão protegida por `x-ingestion-key`;
- persistência de leituras/fases/telemetria/eventos.

## Endpoints relevantes

- `/api/v1/leituras`
- `/api/v1/historico-fases`
- `/api/v1/telemetria`
- `/api/v1/dashboard/resumo`

## Regras

- semáforo físico não é controlado pela API;
- API registra e distribui dados para clientes.
