---
tipo: principio
nivel: 3
fluxo: Experimentação & Dados
autores: [Tobi Lütke]
---
# Goodhart's Law — Métricas como Metas

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Princípio · **Fontes:** [[Tobi Lütke]]

## Ideia central
**Goodhart's Law**: qualquer métrica que se torna uma meta deixa de ser uma boa métrica.

O mecanismo é o mesmo do overfitting em machine learning: quando você treina um modelo para otimizar uma função de perda (proxy da tarefa real), o modelo aprende a "trapacear no benchmark" em vez de aprender a fazer a tarefa real. O mesmo acontece com organizações: quando uma métrica vira objetivo, times aprendem a otimizar a métrica sem necessariamente criar o valor que ela pretendia capturar.

> "Goodhart's law just says 'any metric that becomes a goal ceases to be a good metric.' Same exact thing as overfitting, just for businesses."

## Por que isso é um problema sistêmico
Nenhuma métrica isolada é um heurístico completo para um negócio complexo. Negócios têm milhares de tensões simultâneas que não podem ser mantidas em harmonia otimizando para um número fixo.

O corolário: **o espaço de valor mais rico é o não-quantificável**. Tobi estima que a sobreposição entre "o que é mais valioso" e "o que é facilmente quantificável" é apenas ~20% — o que deixa 80% do espaço de valor invisível para quem só olha para métricas.

Os exemplos que Tobi cita: fun (diversão), delight (deleite), qualidade de artesanato. São as mais poderosas forças motoras de produto de longo prazo, e são exatamente as que não aparecem em dashboards.

> "The most powerful unquantifiable things in the world of business are fun and delight. If people have fun when they're doing something, that is downstream from so many other things."

## A lógica inversa
Se todas as métricas apontam para baixo mas todos dizem "estou tendo muito mais divertimento" — o que vai acontecer a seguir, com algum delay, é que todas as métricas vão subir. Isso não é magia, é precedência causal: fun e delight são upstream, métricas são downstream.

Por isso a Shopify não tem OKRs no sentido do Vale do Silício para o core do produto: não porque seja contra métricas (têm analytics extremamente sofisticados), mas porque tornar uma métrica em meta de promoção destrói a capacidade de perseguir o não-quantificável.

## Goodhart's Law em outros domínios
- **Escola**: marks (notas) deveriam ser proxy de aprendizado. Crianças que "fazem batota" para tirar boa nota são overfitting na função de perda da escola.
- **ML**: qualquer loss function é proxy da tarefa real. Overfitting no benchmark ≠ performar bem na tarefa.
- **Recrutamento**: anos de experiência como proxy de habilidade → candidatos que gaming the metric sem necessariamente ter a habilidade.

A universalidade de Goodhart's Law é o sinal de que é uma verdade endurante — campos diferentes chegam à mesma conclusão com terminologias diferentes.

## Aplicação prática
- Use métricas como inputs de informação, não como outputs de avaliação de performance
- Reserve pelo menos uma parte do roadmap para iniciativas guiadas por convicção e gosto, não por metrics
- Monitore proxies não-quantificáveis: "o time está com mais energia?", "o produto ficou mais divertido?"
- Tenha cuidado com sistemas de incentivo (promoção, bônus) atrelados diretamente a uma única métrica

## Conceitos relacionados
[[OEC - Overall Evaluation Criterion]] · [[A maioria das ideias falha no teste]] · [[Métricas Simples vs Compostas — Clareza Bate Perfeição]] · [[Path Dependence — Re-derivar das Raízes]] · [[Jogo de 100 Anos — Horizonte como Estratégia]]

> 🎧 [Tobi Lütke's leadership playbook: First principles, infinite games, and maximizing human potential](https://www.youtube.com/watch?v=tq6vdDJQXvs) · 2025-02-02
