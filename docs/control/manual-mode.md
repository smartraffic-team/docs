# Modo Manual

## Regras

- troca manual exige estado serial saudável;
- comandos em transição/pending são recusados;
- firmware ainda aplica transições seguras.

## API local

- `POST /semaforo/modo` com `manual`/`automatico`
- `POST /semaforo/manual` com via `A` ou `B`

## Operação recomendada

1. confirmar estado online;
2. ativar `manual`;
3. enviar troca de via;
4. aguardar ACK/estado antes de novo comando.
