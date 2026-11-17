# FAQ / Troubleshooting

## Docker não conecta (`dockerDesktopLinuxEngine`)
Abra o Docker Desktop e aguarde `Running`.

## API sem conexão com banco
Confirme `DATABASE_URL` e se `database` está ativo.

## Câmera piscando detecção
Validar iluminação/ROI e parâmetros de detecção; há histerese básica já aplicada.

## Semáforo sem resposta
Checar firmware ST1, porta COM e health serial no `/status`.
