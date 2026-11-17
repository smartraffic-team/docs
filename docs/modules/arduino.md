# Firmware Arduino (C++)

Local: `arduino/arduino_code.ino`

## Função

- executa máquina de estados do semáforo;
- aplica transições seguras (amarelo + all-red);
- entra em fallback por watchdog sem comandos.

## Protocolo

- recebe comandos ST1 (`AUTO`, `MANUAL`, `KEEP`);
- envia `STATE ST1 ...` periodicamente.

## Importante

- Python decide planos de verde;
- Arduino decide execução temporal local e segurança de transição.
