# O que é o SmartTraffic

O SmartTraffic é um protótipo acadêmico para controle semafórico adaptativo em maquete.

Objetivo principal:

- medir fluxo por visão computacional;
- operar semáforos locais via Arduino;
- registrar dados operacionais em API + MySQL;
- exibir dados em plataforma web.

Princípios do projeto:

- o controle **é local** (Python + Arduino);
- API/banco **não** acionam LED diretamente;
- leitura de câmera não equivale a veículos únicos;
- ausência de leitura não é ausência de veículos.

Estado atual resumido:

- operação com duas câmeras no Flask local;
- API NestJS integrada com ingestão por fila SQLite;
- dashboard React integrado à API;
- mobile ainda em fase planejada no roadmap.
