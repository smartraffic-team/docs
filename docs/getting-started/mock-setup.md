# Simulação da Maquete

Este projeto é executado em maquete acadêmica.

Checklist mínimo para simular:

- duas webcams em índices distintos;
- Arduino com firmware ST1 gravado;
- porta serial correta em `SMARTTRAFFIC_ARDUINO_PORT`;
- Flask local exibindo `/video_feed/A` e `/video_feed/B`.

Exemplo de variáveis no PowerShell:

```powershell
$env:SMARTTRAFFIC_CAMERA_A_INDEX='1'
$env:SMARTTRAFFIC_CAMERA_B_INDEX='0'
$env:SMARTTRAFFIC_ARDUINO_PORT='COM5'
python smarttraffic_app.py
```
