# Interface Web Local

A interface Flask local (`http://localhost:5000`) é a tela de operação técnica.

## Itens principais

- duas câmeras lado a lado (A/B);
- contadores por via;
- estado dos sinais (verde/amarelo/vermelho);
- modo automático/manual e comandos.

## Fonte dos dados

- `/status` para snapshot operacional;
- `/video_feed/A` e `/video_feed/B` para stream.
