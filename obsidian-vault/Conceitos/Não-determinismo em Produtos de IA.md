---
tipo: insight
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Não-determinismo em Produtos de IA
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
Produtos de IA diferem do software tradicional por operar com **não-determinismo duplo**: (1) na *entrada*, usuários expressam intenções em linguagem natural de formas infinitamente variáveis; (2) na *saída*, o LLM responde de maneira probabilística e sensível ao fraseamento do prompt. Em software tradicional a decision-engine mapeia intenção → ação de forma previsível. Em IA, você não sabe como o usuário se comportará *nem* como o LLM responderá — input, processo e output são todos incertos.

## Como aplicar
1. Projete para a variedade de intenções, não apenas para o "happy path" de input.
2. Trate o LLM como uma API não-determinística: planeje para outputs variáveis, não só para o caso esperado.
3. Implemente logging desde o dia 1: sem dados sobre como usuários interagem você não tem base para calibrar.
4. Não escale antes de entender o espaço de variação — calibração primeiro, crescimento depois.
5. Reconheça o paradoxo: o não-determinismo é também o ponto mais poderoso da IA (barreiras baixas de uso via linguagem natural).

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Você não sabe como o usuário vai se comportar com seu produto, e também não sabe como o LLM vai responder a isso — são três variáveis que você não controla totalmente."
- LLMs são sensíveis a fraseamentos de prompt e são caixas pretas: impossível antecipar o espaço de outputs sem experimentação real em produção.
- O não-determinismo torna a IA mais acessível (comunicação natural), mas cria o desafio de obter resultados determinísticos com tecnologia não-determinística.

### [[Kiriti Badam]]
- "Quando você não começa com o agente com todas as ferramentas e todo o contexto desde o dia 1, você se força a pensar: *qual problema específico vou resolver?*"
- Iniciar com escopo mínimo combate a tendência de se perder na complexidade da solução e esquecer o problema a resolver.

> 🎧 [Why most AI products fail: Lessons from 50+ AI deployments at OpenAI, Google & Amazon (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Framework CCCD]] · [[Evals vs. Monitoramento em Produção]] · [[Humans in the Loop (algoritmos)]] · [[A-B Testing (Ronny Kohavi)]]
