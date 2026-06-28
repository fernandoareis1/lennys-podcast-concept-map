---
tipo: principio
nivel: 3
fluxo: Experimentação & Dados
autores: [Julia Schottenstein]
---
# Pior é Melhor — Tech Debt como Problema de Champanha
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Princípio · **Fontes:** [[Julia Schottenstein]]

## Ideia central
Dois mantras de Julia Schottenstein que combatem o perfeccionismo em desenvolvimento de produto:

1. **Worse is better** — bom o suficiente e em produção é melhor que perfeito e na sua cabeça. Você não consegue antecipar como as pessoas vão usar o produto; o shipping é o momento que gera aprendizado real.

2. **Tech debt é um problema de champanha** — ter dívida técnica significa que pessoas estão usando o produto. O scheduler ingênuo do dbt (um grande loop sobre uma tabela de jobs) foi "embaraçoso" para o time, mas foi o scheduler que precisava existir para descobrir que havia escala suficiente para justificar reconstruir.

## A história do scheduler do dbt
O scheduler inicial do dbt Cloud era extremamente simples: um for loop que percorria todos os jobs e perguntava "é hora de rodar esse job?". O time o considerava "naive e embarrassing". Mas foi exatamente o que permitiu descobrir que havia 8.000 empresas usando o scheduler com 10 milhões de runs por mês — escala suficiente para justificar a reconstrução com distributed schedulers, Celery workers e RabbitMQ.

O que o time NÃO precisava no lançamento era de infraestrutura complexa, porque não havia usuários para justificá-la. O tech debt que surgiu foi a evidência de que o produto tinha chegado à escala.

## Por que funciona
- Você não consegue antecipar todos os edge cases antes de ship — os usuários os revelam
- A pressão pelo aperfeiçoamento antes do launch é frequentemente perfeccionismo disfarçado de rigor técnico
- Tech debt em produção é sempre mais fácil de corrigir do que produto certo que ninguém usa

## Como aplicar
1. **Defina "bom o suficiente" antes de começar** — qual é o critério mínimo para que o produto funcione para o seu caso de uso mais simples?
2. **Ship com consciência do débito** — não ignore a dívida técnica; documente-a e trate-a como backlog prioritário quando escala justificar
3. **Use o tech debt como sinal de saúde** — se você está acumulando dívida, é porque está crescendo. Preocupe-se quando não há dívida porque não há usuários.
4. **Combata o perfeccionismo com urgência de aprendizado** — o custo de não aprender com usuários reais é maior que o custo de ter uma solução menos elegante

## Insights por autor
### [[Julia Schottenstein]]
- "Worse is better and tech debt is a champagne problem" — os dois mantras para combater perfeccionismo
- O scheduler ingênuo do dbt: "We were a little embarrassed by it. It was a big old for loop over a big old jobs table." Mas foi suficiente para ir de zero a 8.000 empresas.
- "We couldn't have had a distributed scheduler with Celery workers and RabbitMQ at launch — we had no users. So these two sayings just remind people: let's ship, let's get it out into users' hands."
- Inspiração em *Gödel, Escher, Bach* de Douglas Hofstadter — livro favorito de lógica de Julia
> 🎧 [M&A, competition, pricing, and investing](https://www.youtube.com/watch?v=y9hmrMBRPDI) · 2023-07-13

## Conceitos relacionados
[[MVP — O Teste de Hipótese Mínimo]] · [[Decidir com poucos dados é melhor que com zero]] · [[Falha Conclusiva — Design de Experimento Definitivo]] · [[Dívida Técnica como Alavanca Estratégica]] · [[Solve before Scale]]
