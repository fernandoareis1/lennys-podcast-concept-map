---
tipo: framework
nivel: 3
fluxo: Ativação & Retenção
autores: [Patrick Campbell]
---
# Retenção Tática vs. Estratégica — Os 25-40% Ignorados

**Fluxo:** [[07 - Ativação & Retenção]] · **Tema:** [[Retenção — Retenção & churn]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Patrick Campbell]]

## Ideia central
Retenção tem dois componentes completamente distintos que precisam ser gerenciados separadamente. Times de produto quase sempre focam apenas em um deles — e ignoram 25 a 40% do problema de churn.

**Retenção Estratégica**: tudo que o time de produto faz bem. ICPs corretos, time-to-value, roadmap certo, missão métrica, features certas, eliminar paper cuts. É o trabalho central do product leader.

**Retenção Tática**: falhas de pagamento, otimização de cobrança, fluxos de cancelamento, offboarding, planos de pausa, planos de manutenção. Geralmente ninguém cuida disso porque product teams estão focados no futuro, não em "resolver problemas de operação".

## O problema de perspectiva do produto
Times de produto são naturalmente forward-looking — eles querem construir o próximo roadmap, resolver o próximo problema de usuário. O resultado é que uma categoria inteira de churn — 25 a 40% — é deixada sem dono.

E esse churn tático **não é difícil de resolver**: implementar emails de recuperação de cartão falhado, construir um fluxo de cancelamento com uma boa pergunta de salvage, oferecer plano de pausa em vez de cancelamento total. Duas semanas de trabalho podem eliminar 25% do seu churn problem.

## O fluxo de cancelamento: 18-30 segundos
Patrick Campbell analisou **2 milhões de fluxos de cancelamento** (ProfitWell/Paddle). As descobertas:

1. **Você tem 18 a 30 segundos**: o usuário está em um "freight train" mental — já decidiu sair. A janela é curta.

2. **Duas perguntas que funcionam**:
   - "Por que você está saindo?" — múltipla escolha, não resposta livre (1 em 100 respostas abertas é útil)
   - "O que você gostou do produto?" — **esta é a chave**: força o usuário a pensar no que valorizava, ativando o efeito nostalgia e interrompendo o freight train

3. **Depois das respostas**: ofereça salvage offer, plano de pausa ou plano de manutenção baseado nos dados de engajamento + resposta do usuário.

A pergunta sobre "o que gostou" parece contra-intuitiva — por que perguntar ao usuário que está saindo sobre o que gostou? Exatamente porque ela cria ruptura cognitiva: a pessoa estava focada no problema, e você a força a recuperar memórias positivas. Isso para o trem.

## Falhas de pagamento: churn involuntário invisível
Uma fração significativa do churn é **involuntária** — cartão expirado, limite excedido, atualização de número. Times de produto ignoram porque não é "problema de produto". Mas é churn real.

Soluções simples (reminder antes de expirar, retry inteligente com backoff, email de recuperação com link direto para atualizar cartão) resolvem boa parte do problema. Patrick chegou a oferecer isso como produto gratuito no ProfitWell Metrics — o impacto era tão alto que criava stickiness.

## Quem deve cuidar disso
Patrick sugere que **times de finanças** assumam a retenção tática — são eles que têm visibilidade em falhas de pagamento e renovações, e não têm o viés de "preciso construir features novas". Times de produto podem ser consultados, mas não devem ser os DRIs.

O pior cenário: ninguém é dono, o problema fica entre produto, finanças e sucesso do cliente, e 25-40% do churn permanece sem endereço.

## Insights por autor
### [[Patrick Campbell]]
- "Most of the time, tactical retention is about 25 to 40% of your churn problem — significant amount, but you don't really look at it because you're focused on features."
- "We looked at 2 million cancellation flows. You have 18 to 30 seconds when someone hits the cancel button."
- "'What did you like about the product?' — that's the question that works. That person is on a freight train to cancel. The minute you ask what they liked, you tap into the nostalgia effect and stop the train."
- "Finance teams should just take this on. Product teams are always going to be thinking on the future rather than fixing this right now."
> 🎧 [10 lessons on bootstrapping a $200m business | Patrick Campbell (ProfitWell)](https://www.youtube.com/watch?v=FjLSCrSg5QY) · 2023-02-19

## Conceitos relacionados
[[Churn como fonte de discovery]] · [[Retenção como Prova de Valor Real]] · [[Retenção é a base do crescimento]] · [[Trial Reverso — Freemium mais Trial Combinados]]
