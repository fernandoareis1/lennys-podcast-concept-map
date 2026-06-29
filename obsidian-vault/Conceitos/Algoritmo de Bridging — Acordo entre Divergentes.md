---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Jay Baxter, Keith Coleman]
---
# Algoritmo de Bridging — Acordo entre Divergentes

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Jay Baxter]] · [[Keith Coleman]]

## Ideia central
O insight central por trás do Community Notes: em vez de buscar **maioria** (que amplifica viés) ou **consenso** (que é impossível em tópicos polarizados), busque **acordo surpresa** — notas que pessoas que normalmente discordam entre si classificam como úteis.

Quando dois usuários com histórico de opiniões opostas concordam que uma nota é útil, isso é um sinal extremamente confiável de que a nota é: precisa, neutra e verdadeiramente informativa. Não é uma votação majoritária — é um filtro de bridging que corta polarização.

**Por que funciona:**
- Maioria simples amplifica o grupo dominante na plataforma.
- PageRank e variantes são manipuláveis por anéis de votos coordenados.
- Bridging é inerentemente anti-manipulação: você precisaria recrutar pessoas de lados opostos para coordenarem um fake.

O algoritmo usa Matrix Factorization para identificar vetores de "identidade política" latentes e detectar quando raters de diferentes grupos concordam — esse é o sinal de ouro.

## Como aplicar
1. Em sistemas de rating/moderação: não use maioria simples; crie mecanismos que detectem acordo trans-grupos.
2. Em pesquisa qualitativa: procure pontos de convergência entre personas que normalmente divergem — esses pontos são os mais robustos e menos tendenciosos.
3. Em decisões de produto: se pessoas de lados opostos de um debate interno concordam que algo é bom, esse é seu sinal mais confiável.
4. Em calibração de qualidade: prefira conservadorismo (mostrar poucos, mostrar bons) a cobertura (mostrar tudo, incluindo duvidosos). Community Notes mostra ~8% das notas propostas.

## Insights por autor
### [[Jay Baxter]]
- "We actually look for agreement from people who have disagreed in the past. And what we see is when people actually have that sort of surprising agreement, that's what makes the notes so neutral and accurate and well-written."
- O primeiro algoritmo implementado foi uma variante de PageRank — focado em anti-manipulação, mas que amplificava viés de grupos majoritários. Só após dados reais do piloto ficou claro que bridging era o caminho.
- A técnica foi descoberta por comparação direta (bake-off interno entre algoritmos) — não por hipótese prévia.
- Estudos externos independentes confirmaram: ver um post com nota vs. sem nota muda o nível de concordância das pessoas com as afirmações do post.
- 50-60% de queda nos reposts após uma nota ser aplicada — o efeito viral se colapsa rapidamente.

### [[Keith Coleman]]
- "We wanted all of humanity to participate. Because if we have all of humanity, we then have the data to understand what notes will be helpful to actual humanity."
- A opção conservadora (0.4 no score de utilidade) foi deliberada: "We live or die based on the quality of the notes. We'd rather not show a note that maybe good than the other way around."
- A confiança no sistema vem diretamente da qualidade das notas — e a qualidade vem do conservadorismo do threshold.

> 🎧 [An inside look at X's Community Notes | Keith Coleman & Jay Baxter (1:47:58)](https://www.youtube.com/watch?v=8dgyqYHLcCI)

## Conceitos relacionados
[[Experimentação — Aprender com pouco e qualitativo]] · [[Falsificação e Pensamento Científico]] · [[Nuance acima de Frameworks — O Limite das Metodologias]]
