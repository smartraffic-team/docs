# Limiar de Ativação (anti-flapping)

## Regras atuais

- janela de filtro: 2 s (`FILTER_WINDOW`)
- contagem filtrada por mediana
- verde adaptativo: `min(25, 20 + 2*mediana)`
- prioridade por demanda de veículos parados e idade de espera

## Melhorias recomendadas

- histerese para troca de prioridade (diferença mínima);
- permanência mínima de prioridade antes de nova troca;
- grace period para manter decisão em quedas curtas de medição.

Objetivo: reduzir oscilações visuais e trocas excessivas de via.
