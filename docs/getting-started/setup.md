# Setup do Ambiente

## 1) Banco local

```powershell
cd ..\database
Copy-Item .env.example .env
docker compose up -d --wait
```

## 2) API

```powershell
cd ..\api
Copy-Item .env.example .env
npm install
npm run prisma:generate
```

## 3) Frontend

```powershell
cd ..\SmartTraffic-platform
Copy-Item .env.example .env
npm install
```

## 4) Computer vision

```powershell
cd ..\computer-vision
python -m pip install -r requirements.txt
```

## Variáveis críticas

- API: `DATABASE_URL`, `JWT_SECRET`, `INGESTION_KEY`, `CORS_ORIGINS`
- CV: índices de câmera e porta serial (`SMARTTRAFFIC_ARDUINO_PORT`)
