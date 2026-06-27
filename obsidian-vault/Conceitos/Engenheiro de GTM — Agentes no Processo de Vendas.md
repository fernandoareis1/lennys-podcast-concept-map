---
tipo: conceito
nivel: 3
fluxo: Growth & Aquisição
autores: [Jeanne DeWitt Grosser]
---
# Engenheiro de GTM — Agentes no Processo de Vendas

**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Distribuição & canais]] · **Camada:** L3
**Tipo:** Conceito · **Fontes:** [[Jeanne DeWitt Grosser]]

## Ideia central
O Engenheiro de GTM (Go-To-Market Engineer) é um papel emergente que une expertise de vendas com capacidade de engenharia para construir agentes de IA que automatizam os workflows repetitivos de GTM. No Vercel, o lead agent foi construído por um único engenheiro de GTM em 6 semanas (25-30% do tempo) e reduziu o time de SDRs de inbound de 10 para 1, mantendo a mesma taxa de conversão. O custo do agente: ~$1.000/ano, contra mais de $1M em salários. O processo: shadow o melhor SDR, documente o workflow humano passo a passo, codifique como agente, mantenha humano no loop para QA enquanto treina. O mesmo princípio foi aplicado ao "deal-bott" (que analisa calls do Gong e identifica por que deals são perdidos — muitas vezes uma conclusão diferente do que o AE reportou) e ao pipeline bott em tempo real.

## Como aplicar
1. Identifique o workflow mais repetitivo e legível do seu processo de GTM (geralmente inbound qualification).
2. Coloque um engenheiro de GTM para fazer shadow do melhor performer e documentar cada passo.
3. Construa o agente com humano no loop: o agente executa, humano revisa e aprova antes de enviar.
4. Meça os mesmos KPIs que mediria o humano (conversão, tempo para converter, qualidade das respostas).
5. Quando a taxa de aprovação humana for alta o suficiente, reduza o humano no loop e redeaploy para funções de maior valor (outbound, enterprise).
6. Perfil ideal: sales engineer com formação técnica, não engenheiro aprendendo vendas.

## Insights por autor
### [[Jeanne DeWitt Grosser]]
- "10 SDRs → 1 SDR que é QA do agente, com os outros 9 movidos para outbound. Custo do agente: $1.000/ano."
- O deal-bott revelou que o maior deal perdido no trimestre não foi por preço (como o AE reportou), mas por nunca ter chegado ao economic buyer.
- "Vendedores passam apenas 30-40% do tempo com clientes. Com agentes, podemos chegar a 70%."
- GTM engineers na Vercel são ex-sales engineers com CS degree — entendem tanto o craft de vendas quanto de código.
> 🎧 [What world-class GTM looks like in 2026 | Jeanne DeWitt Grosser (1:26:02)](https://www.youtube.com/watch?v=RmnWHz8HD74)

## Conceitos relacionados
[[GTM como Produto — Experiência não Transação]] · [[De Saber a Fazer — A Transição dos Agentes de IA]] · [[GTM pelo alinhamento comprador-usuário]]
