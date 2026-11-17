# Computer Vision (YOLO + OpenCV)

Local: `computer-vision/`

## Arquivos-chave

- `smarttraffic_app.py`: app Flask principal
- `vision.py`: captura, detecção e overlays
- `traffic.py`: lógica de controle e prioridades
- `ingestion.py`: fila SQLite e envio para API

## Responsabilidades

- capturar A/B de forma independente;
- detectar `car` e `person`;
- produzir estado de medição válido/inválido;
- manter controle local mesmo sem API.

## Observações

- labels visuais atuais: `Carro` e `Pessoa` (sem `%`);
- foi aplicada histerese simples para reduzir flicker de detecção.
