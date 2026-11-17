# Modelo de Dados

Referência operacional: schema V2.1 do repositório `database`.

Tabelas centrais:

- `vias`
- `semaforos`
- `leituras_trafego`
- `historico_fases`
- `telemetria_dispositivos`
- `eventos_sistema`

Convenções:

- IDs BIGINT serializados como string na API;
- datas em UTC/ISO 8601;
- via sempre identificada (`A`/`B`) no fluxo de leitura.
