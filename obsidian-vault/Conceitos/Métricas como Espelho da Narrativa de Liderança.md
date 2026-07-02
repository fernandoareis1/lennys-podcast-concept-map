---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Nicole Forsgren]
---
# Métricas como Espelho da Narrativa de Liderança

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** técnica · **Fontes:** [[Nicole Forsgren]]

## Ideia central
Para que métricas de produtividade (ou qualquer outra) ganhem tração com liderança, precisam ser **enquadradas na linguagem que a liderança já usa**. Não faça os executivos trabalhar para entender o valor — traduza o seu trabalho para o que eles já estão falando.

**A regra:** observe as palavras e temas que dominam as conversas de liderança. Essas palavras revelam o que mais importa. Construa métricas que falem diretamente a esses temas.

## Mapeamento de narrativa → métricas

| Narrativa da liderança | Métricas de impacto a apresentar |
|---|---|
| "Estamos perdendo market share" / "competitividade" | Velocidade de feature-to-production ou feature-to-experiment; quão rapidamente conseguimos aprender? |
| "Precisamos de mais margem" / "profit margin" | Custos economizados: cloud costs de builds otimizados, redução de vendors, headcount recovered |
| "Precisamos de maior velocidade" / "velocity" | Deployment frequency, lead time, tempo do commit ao deploy |
| "Precisamos nos transformar" / "disruption" | Capacidade de experimentação: quantos A/B tests podemos rodar por semana? |

## Por que enquadramento importa mais que a métrica
"We don't want to make them work to understand what it is that we're doing and the value that we provide."

Mesmo uma ótima melhoria de DevEx fracassa internamente se não é comunicada na língua certa. Um time que reduziu build time em 40% e presenta esse resultado como "economizamos 2h/dev/dia" terá muito menos impacto do que "liberamos X% do custo de engenharia mensalmente para trabalho de maior valor."

## Como aplicar
1. **Escute antes de medir**: antes de definir métricas, fique atento às palavras que liderança usa repetidamente. "Velocity"? "Transformation"? "Margin"?
2. **Reframeie se necessário**: se eles chamam tudo de "produtividade de engenharia", use esse termo. Se chamam de "velocity", adote velocity.
3. **Correlação é suficiente**: não é necessário provar causalidade perfeita. "Quando aceleramos DevEx E adotamos AI tools juntos, nossa time-to-experiment caiu de 3 semanas para 3 dias." Disclose ambas as contribuições.
4. **Múltiplas audiências, múltiplas métricas**: engenheiros querem ouvir sobre tempo economizado e redução de toil; liderança quer ouvir sobre velocidade e custo. Prepare versões diferentes.

## Exemplo de transparência sobre atribuição
"Yes, we rolled out AI tools. We also had this effort in DevEx. They partnered very closely together. Both of them probably contributed to this. If we had AI tools without the DevEx improvements, we probably would've had some improvements, but not nearly as much." — o honestidade sobre atribuição aumenta credibilidade.

## Insights por autor
### [[Nicole Forsgren]]
- "It depends on what your leadership chain really cares about. Think about the messaging you've been hearing. Have they been talking about market share? Losing market share?"
- "If they're calling it velocity, and velocity is what matters to them, think about how to frame this in terms of velocity."
- "If you can slightly reframe it... because then it will resonate with them. We don't want to make them work to understand what it is that we're doing."

> 🎧 [How to measure AI developer productivity in 2025 | Nicole Forsgren](https://www.youtube.com/watch?v=SWcDfPVTizQ)

## Conceitos relacionados
[[SPACE Framework — Medir Produtividade Além do Output]] · [[Dados Sintéticos — Sem Parede de Dados no Pós-Treinamento]] · [[Diagnosticar com Dados, Tratar com Design]] · [[Métricas Simples vs Compostas — Clareza Bate Perfeição]]
