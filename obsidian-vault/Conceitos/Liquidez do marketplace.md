---
tipo: framework
nivel: 3
fluxo: Growth & Aquisição
autores: [Benjamin Lauzier]
---
# Liquidez do marketplace
**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Modelos de crescimento]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Benjamin Lauzier]]

## Ideia central
Liquidez é **como marketplaces vencem**: mede a capacidade de conectar compradores e vendedores de forma eficiente. Visualmente, é a sobreposição entre o que o supply quer oferecer e o que o demand quer comprar. Sem liquidez suficiente, nenhuma outra estratégia de crescimento sustenta.

A **métrica de liquidez** é a taxa de preenchimento (*fill rate*) da demanda intencional: de todos os usuários que chegam com intenção real de transação, quantos de fato transacionam? (ex: buscas com data no Airbnb → reservas; aberturas de app Lyft → corridas concluídas.)

Mais acionável que o fill rate é a **métrica de saúde de mercado (market health metric)**: um indicador proxy que prediz a liquidez antes dela acontecer e que os times podem mover diretamente. No Lyft, era o ETA do motorista mais próximo — se ≤2 minutos, a probabilidade de conversão atingia teto; acima disso, caía precipitosamente.

## Como aplicar
1. **Defina seu fill rate**: de quem chega com intenção clara, quantos transacionam? Esse é o indicador de output.
2. **Encontre o preditor de saúde de mercado**: qual variável correlaciona mais fortemente com o fill rate e pode ser controlada pelo time de supply? (ETA, número de profissionais disponíveis em raio X, etc.)
3. **Estabeleça o threshold**: determine o ponto de inflexão onde o preditor "satura" a probabilidade de conversão. Abaixo dele, tudo é urgente. Acima, retornos marginais.
4. **Monitore por mercado/categoria**: liquidez é local — um marketplace pode ter excelente liquidez em São Paulo e péssima em Curitiba. Gerencie como portfólio de mercados.
5. **Construa o flywheel**: mais supply → mais liquidez → melhor experiência para demanda → mais transações → mais earnings para supply → mais supply.

## Insights por autor
### [[Benjamin Lauzier]]
- "Liquidez é como marketplaces vencem. É a medida da sua capacidade de conectar compradores e vendedores de forma eficiente."
- "É o multiplicador direto da eficiência do seu marketplace. Está no centro da sua visão, é por isso que você existe."
- Sobre o ETA: "Sabíamos que se o motorista mais próximo estivesse a ≤2 minutos, o usuário quase certamente pedia a corrida. Se fossem 5 minutos, ele verificava o Uber, caminhava, pegava o ônibus."
- "A métrica de saúde de mercado é muito mais acionável para os times. Se você é o time de supply, pode ver se adicionar 100 motoristas realmente está reduzindo ETAs."
> 🎧 [How marketplaces win: Liquidity, growth levers, quality, more (1:24:03)](https://www.youtube.com/watch?v=CYwgStMln6U) · 2024-09-29

## Conceitos relacionados
[[Growth Loops vs Funil]] · [[Retenção é a base do crescimento]] · [[Teoria do Usuário Adjacente]]
