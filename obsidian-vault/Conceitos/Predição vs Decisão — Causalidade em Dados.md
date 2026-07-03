---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Ramesh Johari]
---
# Predição vs Decisão — Causalidade em Dados

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Ramesh Johari]]

## Ideia central
Machine learning prediz correlações — mas decisões de negócio exigem causalidade. Perguntar "quem tem o maior LTV?" é diferente de perguntar "quanto a mais esse cliente vai gastar PORQUE eu enviei esta promoção?". Confundir os dois leva a decisões que parecem racionais mas desperdiçam recursos ou não geram impacto.

O que diferencia data scientists excepcionais: eles têm no fundo da mente que o objetivo é **ajudar o negócio a tomar decisões** — não apenas fazer previsões acuradas.

## Como aplicar
1. **Reformule sempre a pergunta:** em vez de "quem tem maior LTV?", pergunte "qual é o incremento de LTV causado pela minha intervenção?" Em vez de "qual candidato tem mais chance de ser contratado?", pergunte "qual ranking de candidatos leva a mais contratações BEM-SUCEDIDAS?"
2. **Pense em diferenças, não em absolutos:** o efeito causal é sempre um diferencial (com vs. sem a intervenção). Modelos preditivos entregam absolutos; modelos de uplift entregam diferenciais.
3. **Use experimentos como a ponte:** a única forma confiável de medir causalidade é aleatorização — um experimento (A/B test) onde a intervenção é atribuída aleatoriamente. Predição sem experimento mede correlação que pode ser espúria.
4. **Cuidado com o ML como substituto de decisão:** um modelo de hiring que prevê quem será contratado com base em histórico passado vai perpetuar os mesmos padrões, não necessariamente melhorar os matches. A pergunta correta é: "qual ranking de candidatos vai produzir contratações melhores?"
5. **Quando não há experimento:** use inferência causal (instrumental variables, difference-in-differences, regression discontinuity) para estimar o efeito causal de intervenções observacionais.

## Insights por autor
### [[Ramesh Johari]]
- "Predição é sobre encontrar padrões. Decisão é sobre causalidade. Você aprende no ensino médio que correlação não é causação. Mas quando construímos modelos de ML, pedimos às pessoas que façam previsões — o que é correlação. Quando pedimos que tomem decisões, pedimos que pensem em causalidade."
- Exemplo clássico: mandar promoções para clientes de alto LTV parece certo ("você está mandando para os mais valiosos"). Mas se eles já iam comprar de qualquer forma, o incremento causado pela promoção é zero. Você desperdiçou recursos e comprometeu a margem.
- "A primeira e mais importante coisa que um data scientist deve ter em mente é que seu objetivo é ajudar o negócio a TOMAR DECISÕES. A distinção entre causalidade e correlação importa muito aqui."
- "Bons data scientists pensam em dois algoritmos de ranking não apenas em termos de qual prediz melhor o comportamento passado, mas qual leva a MAIS reservas, mais contratações bem-sucedidas, mais matches de qualidade no futuro."

> 🎧 [Marketplace lessons from Uber, Airbnb, Bumble, and more | Ramesh Johari (Stanford professor) (1:23:36)](https://www.youtube.com/watch?v=BVzTfsUMaK8)

## Conceitos relacionados
[[A/B Testing (Ronny Kohavi)]] · [[Experimentação como Disciplina Científica]] · [[Falha Conclusiva — Design de Experimento Definitivo]] · [[Diagnosticar com Dados, Tratar com Design]]
