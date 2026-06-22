---
tipo: insight
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Non-determinismo em produtos de IA
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
Ao contrário de software tradicional (fluxos determinísticos de botões e formulários), produtos de IA operam com dois pontos de não-determinismo simultâneos: (1) **input não-determinístico** — usuários interagem em linguagem natural de inúmeras formas; (2) **output não-determinístico** — o LLM é uma API probabilística sensível ao fraseado do prompt e age como caixa-preta. Isso torna impossível prever o comportamento do sistema da mesma forma que se prevê um software convencional, exigindo uma abordagem radicalmente diferente de construção, teste e iteração.

## Como aplicar
1. Abandone a expectativa de comportamento 100% previsível; projete para **monitorar e calibrar**, não para definir de uma vez.
2. Mapeie os dois eixos: "como os usuários vão frasear o pedido?" e "quais são as variações de output possíveis do LLM?".
3. Construa datasets de comportamento esperado antes de lançar — nem que sejam 10 exemplos curados — para ter uma linha de base de calibração.
4. Use monitoramento de produção (sinais implícitos e explícitos) para capturar padrões de uso não antecipados.
5. Aceite que qualquer model upgrade (ex.: GPT-4o → GPT-5) recalibra o sistema — preveja ciclos de recalibração.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Você está trabalhando com uma API não-determinística. Você não sabe como o usuário vai se comportar nem como o LLM vai responder. Então você não entende bem as três dimensões: input, processo e output."
- A "beleza" do não-determinismo: o nível de entrada do usuário é muito mais baixo do que em software tradicional — mas isso também é o problema.
- Ticket de suporte falso da Air Canada: agente aluciou uma política de reembolso que não existia; empresa foi responsabilizada legalmente.
> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

### [[Kiriti Badam]]
- O não-determinismo força a equipe a começar pequena: "quando você começa pequeno, é forçado a pensar em qual problema estou resolvendo."
- Empresas bem-sucedidas na adoção de IA são as que constroem flywheels rápidos para estimar comportamento, não as que chegam primeiro.
> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Humans in the Loop (algoritmos)]] · [[CCCD — Calibração e Desenvolvimento Contínuos]] · [[Assumption Testing]] · [[Decidir com poucos dados é melhor que com zero]]
