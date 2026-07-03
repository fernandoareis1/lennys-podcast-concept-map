---
tipo: aprofundamento
nivel: 4
fluxo: Growth & Aquisição
autores: [Benjamin Lauzier, Dan Hockenmaier, Ramesh Johari]
---
# Liquidez do marketplace — Evidências

**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Modelos de crescimento]] · **Camada:** L4
**Conceito base:** [[Liquidez do marketplace]]
**Fontes:** [[Benjamin Lauzier]] · [[Dan Hockenmaier]] · [[Ramesh Johari]]

Três especialistas com experiência direta em Lyft, Uber, Airbnb, Bumble e outros grandes marketplaces convergem em princípios sobre liquidez — com nuances e ênfases distintas.

---

## 1. Liquidez é o multiplicador de tudo · [[Benjamin Lauzier]]

Benjamin Lauzier, ex-Lyft e autor de How Marketplaces Win, define liquidez como **a sobreposição entre o que o supply quer oferecer e o que o demand quer comprar**. Sem essa sobreposição, toda outra estratégia é estéril.

A métrica de liquidez mais honesta é o **fill rate da demanda intencional**: de todos os usuários que chegam com intenção real de transacionar, quantos de fato transacionam? No Lyft, isso era: buscas com localização ativa → corridas concluídas.

Mais acionável é a **market health metric** — um preditor proxy que os times podem mover diretamente. No Lyft, era o ETA do motorista mais próximo:

> "Sabíamos que se o motorista mais próximo estivesse a ≤2 minutos, o usuário quase certamente pedia a corrida. Se fossem 5 minutos, ele verificava o Uber, caminhava, pegava o ônibus."

O threshold de 2 minutos era o ponto de inflexão: abaixo, probabilidade de conversão atingia o teto. Acima, caía precipitosamente. Esse tipo de threshold define onde alocar esforço de supply.

**Princípio operacional:** liquidez é **local**. Um marketplace pode ser líquido em São Paulo e ilíquido em Curitiba simultaneamente. Gerencie como portfólio de mercados em estágios diferentes — não como número agregado nacional.

> 🎧 [How marketplaces win: Liquidity, growth levers, quality, more (1:24:03)](https://www.youtube.com/watch?v=CYwgStMln6U) · 2024-09-29

---

## 2. Sem liquidez, nada mais importa · [[Dan Hockenmaier]]

Dan Hockenmaier (ex-Uber, Faire, fundador da Marketplace Strategy) leva essa ideia ao extremo:

> "Essentially until you have a liquid marketplace, nothing else matters. You have to prioritize getting to a liquid marketplace above everything else."

A implicação prática mais importante: **corte escopo para gerar liquidez**. É melhor ter um marketplace incrivelmente líquido em um slice estreito (uma geografia, uma categoria, um caso de uso) do que ter liquidez rala em todo lugar.

No Uber, o threshold equivalente era 4-5 minutos de espera: abaixo disso, a experiência é boa o suficiente para reter o comprador; acima, o usuário vai embora.

**Princípio operacional:** a liquidez é local, assim como Lauzier aponta — mas Hockenmaier adiciona que a decisão estratégica de onde lançar e expandir deve ser guiada por onde você consegue atingir threshold de liquidez mais rapidamente. Não dilua em muitos mercados antes de ter o modelo validado em um.

> 🎧 [How marketplace startups should think about growth (1:10:41)](https://www.lennyspodcast.com/how-marketplace-startups-should-think-about-growth-dan-hockenmaier-faire-uber-instacart/) · 2023-07-27

---

## 3. Scaled liquidity como litmus test · [[Ramesh Johari]]

Ramesh Johari (Stanford, advisor de Airbnb, Uber, Stripe, Bumble) adiciona a dimensão mais conceitual: **o que define ser ou não ser um marketplace é ter ambos os lados escalados**.

> "Não há sentido em falar de marketplace se você não tem nenhum dos dois lados escalados ainda. Escale um primeiro. Nesse momento, a melhor orientação é a mesma de qualquer startup."

O litmus test da "scaled liquidity": você tem muitos compradores E muitos vendedores na plataforma? Se não, independente do nome que você dê ao seu negócio, você ainda não é um marketplace no sentido operacional. Se tem apenas um lado escalado, seu trabalho é usar essa vantagem para atrair o outro (o Uber subsidiava drivers em novas cidades para atrair riders).

**Insight fundacional:** o marketplace não vende o produto (o quarto, a corrida). O marketplace vende a **remoção da fricção** de encontrar e transacionar. O valor é o custo de transação eliminado — o que significa que os dois lados (supply e demand) são igualmente clientes. Esse framing muda completamente como você pensa em monetização e retention.

**Cuidado com a disintermediação:** todo marketplace enfrenta o risco de supply e demand transacionarem diretamente (bypassing a plataforma). O modelo de monetização e os incentivos devem desincentivisar isso. Johari sugere cautela em assumir compromissos de plataforma cedo demais — eles podem criar travas que facilitam disintermediação em relações longas.

> 🎧 [Marketplace lessons from Uber, Airbnb, Bumble, and more | Ramesh Johari (Stanford professor) (1:23:36)](https://www.youtube.com/watch?v=BVzTfsUMaK8) · 2023-11-09

---

## Síntese: onde os três convergem

| Princípio | Lauzier | Hockenmaier | Johari |
|---|---|---|---|
| Liquidez é o output crítico | ✓ | ✓ | ✓ |
| Liquidez é local, gerencie por mercado | ✓ | ✓ | — |
| Threshold de saúde define prioridade de supply | ✓ | ✓ | — |
| Só é marketplace com ambos os lados escalados | — | — | ✓ |
| Produto = remoção de fricção, não produto em si | — | — | ✓ |
| Corte escopo para atingir liquidez mais rápido | — | ✓ | ✓ |

**Tensão produtiva:** Lauzier e Hockenmaier focam em como operar um marketplace que já existe (métricas, thresholds, portfólio de mercados). Johari foca em quando você ainda está definindo se é um marketplace — e adverte para não assumir a identidade cedo demais.

---

## Conceitos relacionados
[[Growth Loops vs Funil]] · [[Supply-First no Marketplace]] · [[Demanda como Moeda do Marketplace]] · [[Marketplace como Jardineiro]] · [[Whac-a-Mole — Redistribuição em Marketplaces]] · [[Filtros que fragmentam supply]]
