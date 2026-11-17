# Executando o Protótipo

Ordem recomendada:

1. Banco (`database`)
2. API (`api`)
3. Computer Vision (`computer-vision`)
4. Plataforma (`SmartTraffic-platform`)

## Comandos

### Banco

```powershell
cd ..\database
docker compose up -d --wait
```

### API

```powershell
cd ..\api
npm run dev
```

### Computer Vision

```powershell
cd ..\computer-vision
python smarttraffic_app.py
```

### Plataforma

```powershell
cd ..\SmartTraffic-platform
npm run dev
```

## URLs

- Flask local: http://localhost:5000
- API: http://localhost:3000
- Swagger: http://localhost:3000/api/docs
- Plataforma: http://localhost:5173
