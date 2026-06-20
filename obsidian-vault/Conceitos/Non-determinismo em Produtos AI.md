---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Non-determinismo em Produtos AI
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Produtos AI diferem radicalmente de software tradicional em dois eixos: (1) **input não-determinístico** — o usuário pode expressar a mesma intenção de infinitas formas em linguagem natural; (2) **output não-determinístico** — o LLM é uma API probabilística que não garante a mesma resposta para a mesma entrada. O resultado: você não controla input, processo nem output — todos são fluidos. Isso invalida modelos mentais de software "determinístico" como o Booking.com, onde cada clique leva a um resultado previsível.

## Como aplicar
1. Redesenhe o processo de QA: não há "caminhos felizes" fixos para testar; teste por distribuição de comportamentos.
2. Separe decisões determináticas (código clássico ou modelos ML) de decisões que exigem LLM; não use LLM onde regras simples bastam.
3. Projete a UX esperando variação: mensagens de erro, fallbacks e handoff humano precisam ser explícitos.
4. Invista em logging robusto desde o dia 1 — é a única forma de entender como usuários realmente interagem.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Você não sabe como o usuário vai se comportar com seu produto, e também não sabe como o LLM vai responder."
- LLMs são sensíveis a phrasing de prompts e são caixas-pretas — você não controla a superfície de output.
- A camada de intenção que antes era resolvida com botões e formulários é agora substituída por linguagem natural fluida.

### [[Kiriti Badam]]
- Recomenda começar pequeno e forçar o time a pensar no problema, não na complexidade da solução.
- A tentação de construir agents complexos desde o dia 1 faz o time perder o foco no problema real.

> 🎧 [Why most AI products fail (7:36–13:19)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Agency-Control Trade-off]] · [[CC/CD Framework]] · [[Humans in the Loop (algoritmos)]] · [[A maioria das ideias falha no teste]]
