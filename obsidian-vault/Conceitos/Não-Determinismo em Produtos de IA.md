---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Não-Determinismo em Produtos de IA
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
Produtos de IA diferem do software tradicional em dois eixos críticos: (1) **não-determinismo** — tanto o input do usuário (linguagem natural, imprevisível) quanto o output do LLM (probabilístico, sensível ao prompt) são não-determinísticos; (2) **troca agência-controle** — quanto mais autonomia você cede a sistemas agênticos, menos controle humano resta. Ignorar esses dois eixos é a causa raiz mais comum de falhas em produtos de IA.

## Como aplicar
- Trate o LLM como uma "API não-determinística": projete para variabilidade, não para uniformidade de output.
- Mapeie antes do deploy: "Se o output for inesperado, qual é o pior cenário? O humano ainda consegue corrigir?"
- Nunca salte direto para agente autônomo (V3) — o não-determinismo se compõe em sistemas mais longos e torna depuração muito mais difícil.
- Em sistemas agênticos, a falta de controle é perigosa: o agente pode tomar decisões que comprometem clientes ou a empresa antes de alguém perceber.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Você trabalha com uma API não-determinística. Não sabe como o usuário vai se comportar nem como o LLM vai responder — input, processo e output são todos incertos ao mesmo tempo."
- Produto tradicional (ex.: Booking.com): intenção → botões → ação determinística. Produto de IA: intenção → linguagem natural → resultado probabilístico.
- LLMs são sensíveis ao fraseado do prompt e funcionam como caixas-pretas — você não controla totalmente como o output vai aparecer.

### [[Kiriti Badam]]
- "Não comece com agentes com todas as ferramentas e todo o contexto da empresa no dia 1 esperando que funcione. Comece onde o impacto é mínimo e o controle humano é máximo."
- Ao escalar autonomia, você também descobre problemas de dados que não existiam: taxonomias bagunçadas, funções duplicadas, regras não documentadas.

> 🎧 [Why most AI products fail | Aishwarya + Kiriti (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Escada de Agência-Controle em IA]] · [[CC — Calibração e Desenvolvimento Contínuo]] · [[DHM Model]] · [[Problem Space vs Solution Space]]
