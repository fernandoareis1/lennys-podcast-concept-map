---
tipo: conceito
nivel: 3
fluxo: Experimentação & Dados
autores: [Timothy Davis]
---
# Incrementalidade vs. Atribuição — Crédito Real de Paid

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Conceito · **Fontes:** [[Timothy Davis]]

## Ideia central
**Atribuição** diz qual canal recebeu o crédito pelo clique ou pela conversão. **Incrementalidade** responde uma pergunta diferente e mais difícil: *aquela conversão teria acontecido de qualquer forma, mesmo sem o anúncio?*

A distinção importa porque a atribuição é biased por definição — ela credita o canal que tocou o usuário por último (ou que aparece na jornada), não o canal que causou a conversão. O resultado é que times superestimam o valor de canais específicos e subinvestem em canais que influenciam a decisão mas não recebem crédito na atribuição.

> "Attribution, by itself, is biased. It does not answer the question of whether the person clicking on or seeing an ad would've converted anyways, even in the absence of that ad."

## O caso do eBay
O caso mais famoso de incrementalidade revelando desperdício foi o do eBay em 2012: ao rodar um experimento de incrementalidade no brand spend, descobriram que a maioria dos usuários que clicavam nos anúncios pagos da marca teriam chegado ao site organicamente de qualquer maneira (a marca tinha alta recall e presença orgânica forte). O resultado: o eBay cortou quase todo o brand spend — e o tráfego não caiu.

O contra-argumento: competidores preenchiam o espaço deixado. Mas para marcas com forte tração orgânica, o fenômeno é real.

## Como rodar testes de incrementalidade
**GeoX (Geo Experiment)**
Divide mercados em grupos de tratamento e controle por região geográfica. Um grupo continua vendo os anúncios; o outro, não. Compara resultados para isolar o incremento.

**Conversion Lift Test**
A plataforma (Google, Meta, LinkedIn) intencionalmente não exibe o anúncio para um grupo de controle quando você "ganha" o leilão — exibe o anúncio do segundo colocado no lugar. Esse grupo de controle revela o que teria acontecido sem o anúncio.

Todos os grandes players (Google, Meta, LinkedIn) oferecem suporte a Conversion Lift, mas exigem volumes mínimos de spend — tipicamente acima de $50K/mês na plataforma. Abaixo disso, o sinal não é estatisticamente confiável.

## Incrementality Adjusted Factor (IAF)
O resultado dos testes alimenta um fator de ajuste por canal (IAF) que corrige o crédito real de cada canal no mix. Em vez de usar os números brutos de atribuição para decidir onde investir, o IAF dá uma visão mais precisa do retorno incremental de cada dólar.

## Quando isso é irrelevante
Para times iniciando paid growth (spend abaixo de $50K/mês por plataforma), o custo e a complexidade dos testes de incrementalidade superam o benefício. O foco deve ser:
1. Ter atribuição técnica básica funcionando (UTMs, eventos)
2. Rodar Signs of Life Tests por canal
3. Só então, ao escalar, adicionar camada de incrementalidade

## Aplicação prática
- Não use atribuição last-click como proxy para incrementalidade — são métricas diferentes com conclusões potencialmente opostas
- Ao atingir escala ($50K+/plataforma/mês), solicite Conversion Lift ao rep da plataforma — eles têm interesse em te ajudar, pois ganham mais se você investir certo
- Calibre o IAF por plataforma e por região — canais de brand awareness têm comportamento diferente de performance channels

## Conceitos relacionados
[[Atribuição a prova do futuro]] · [[Signs of Life Test — Exploração Mínima de Canal]] · [[A-B Testing (Ronny Kohavi)]] · [[Holdout de longo prazo]]

> 🎧 [The ultimate guide to paid growth | Timothy Davis](https://www.youtube.com/watch?v=zNJyb3R_Pnc) · 2024-07-28
