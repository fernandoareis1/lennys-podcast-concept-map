---
tipo: framework
nivel: 3
fluxo: Ativação & Retenção
autores: [Noah Weiss]
---
# Métrica de Times com Sucesso — North Star que Alinha Toda a Org

**Fluxo:** [[07 - Ativação & Retenção]] · **Tema:** [[Retenção — Ativação & onboarding]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Noah Weiss]]

## Ideia central
Quando o Slack percebeu que o negócio self-service havia estagnado em 2019, a raiz do problema não era apenas experiência de onboarding — era que **não havia uma métrica de ativação que alinhasse toda a organização**. As equipes de features diferentes não tinham como saber se estavam contribuindo para o motor de crescimento do produto.

A solução foi descobrir, via pesquisa quantitativa, um limiar de uso que **prediz conversão de forma robusta**: **5 ou mais pessoas usando Slack na maioria dos dias úteis da semana**. Equipes que atingem esse limiar têm **400% mais chance de upgrade** nos 6 meses seguintes. Esta métrica virou o north star de ativação do Slack — chamada de "Successful Teams."

## O processo de descoberta
1. Analisar curvas de cohort para identificar onde a saúde do funil se diferencia
2. Testar hipóteses sobre qual combinação de profundidade × largura × frequência prediz conversão
3. Validar correlação com dados históricos de upgrade
4. Formular o threshold como métrica binária (sim/não por equipe), não média
5. Distribuir a responsabilidade por essa métrica para **todos os times de produto**, não apenas o time de self-service

## Por que funciona como north star organizacional
- É suficientemente precoce no funil para que muitas equipes possam influenciá-la
- É suficientemente lagging para ser real (requer hábito de equipe, não evento único)
- É compreensível para qualquer PM, designer ou engenheiro — sem interpretação estatística
- Cria alinhamento sem microgestão: todos sabem o que "sucesso" significa

> "Successful Teams: 5+ people using Slack the majority of the work week. Teams that hit that are 400% more likely to upgrade in the next 6 months."

## A armadilha do north star inicial
Antes dessa descoberta, o Slack usava "equipes criadas" (very top of funnel) e "clientes pagos" (very bottom). O gap entre as duas métricas era grande demais para que equipes no meio do funil soubessem em qual métrica impactavam. O "Successful Teams" preencheu esse gap.

## Distinção com o contexto da "S-Curve de PMF"
Mesmo produto — público diferente. O threshold de 5 × maioria da semana foi descoberto **para a nova audiência** (não-technologists, times maiores, empresas enterprise). O threshold para o público original (desenvolvedores, startups) era muito mais baixo. PMF precisa ser redefinido para cada nova S-curve de audiência.

## Insights por autor
### [[Noah Weiss]]
- "5 people using Slack the majority of the work week to just communicate at all — that team is 400% more likely to upgrade over the next 6 months."
- "That seemed like a very low bar. But it turns out if you could get that level of critical mass, the rest would take care of itself."
- "We wound up motivating not just the self-service team but all the feature teams across the company to drive more new successful teams."
- "PMF is almost like you keep stacking S-curves: you get PMF in a small group, exponential growth, then you hit the ceiling and jump to the next curve."
> 🎧 [The 10 traits of great PMs, AI, and Slack's approach to product | Noah Weiss (Slack, Google)](https://www.youtube.com/watch?v=XrRlVOWe5GE) · 2023-07-23

## Conceitos relacionados
[[Métrica de Ativação de Taxa Baixa — Correlação com Retenção]] · [[Auditoria do Funil PLG]] · [[Growth como sistema, não time]] · [[Teoria do Usuário Adjacente]]
