---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Adriel Frederick]
---
# Humano no Loop Algorítmico

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Adriel Frederick]]

## Ideia central
Em produtos com forte componente algorítmico (ML, otimização, precificação dinâmica), o trabalho central do PM é decidir **o que o algoritmo faz** e **o que o humano decide** — e então construir a interface que torna essa divisão funcional. Algoritmos não entendem efeitos de longo prazo, não entendem o que o usuário vai sentir, e não entendem a intenção estratégica do produto. O humano precisa estar no loop — não como supervisor passivo, mas como tomador de decisão ativo com as ferramentas certas.

## Como aplicar

### 1. Defina a fronteira algoritmo-humano
- Liste as decisões que o produto precisa tomar repetidamente.
- Para cada decisão, pergunte: o algoritmo tem toda a informação e pode otimizar isso sozinho? Ou há julgamento estratégico, contexto externo, ou consequências de longo prazo que exigem uma pessoa?
- Algoritmo → ótimo para otimizar dentro de um objetivo definido em milhões de instâncias.
- Humano → ótimo para definir o objetivo, os constraints, e responder a contextos que o algoritmo não vê (mudança de mercado, decisão do concorrente, crise operacional).

### 2. Dê ao humano informação, não só dados
- O humano no loop precisa de um painel que mostre o **estado do jogo**: o que está acontecendo no mercado? Como estou performando vs. minha meta? Onde o algoritmo está limitado?
- Exemplo Lyft: ops managers precisavam ver tempo de espera, preço vs. concorrente, demanda por cidade — e aí tomar decisões que o algoritmo não podia tomar sozinho (snowstorm, mudança tributária, resposta a competitor).

### 3. Construa as ferramentas de controle como produto de primeira classe
- Controle operacional é requisito de primeira ordem, não afterthought.
- Adriel aprendeu isso da forma difícil: construiu um algoritmo de precificação sofisticado que funcionou em 3 cidades — mas era impossível de operar em 100+ cidades porque ninguém havia tratado as ferramentas de controle como produto.
- Resultado: teve que reconstruir do zero, desta vez colocando flexibilidade operacional como constraint central de design.

### 4. O algoritmo amplifica a intenção humana
- Não é "máquina vs. humano" — é "humano define intenção → máquina amplifica em escala".
- Analogia de Adriel: você não tenta usar chave de fenda de cabeça reta num parafuso phillips. Ferramentas diferentes para problemas diferentes. O PM é designer de ferramentas — define quanto vai no tool e quanto fica com a pessoa.

## Insights por autor
### [[Adriel Frederick]]
- "When you are working on algorithmic heavy products, your job is figuring out what the algorithm should be responsible for, what people are responsible for, and the framework for making decisions."
- "Algorithms don't understand long term effects often, nor do they understand how people might respond to it, nor do they understand your intent for the product."
- "I think about it as designing an interface and make it an extension of yourself rather than a black box on its own."
- A lição do Lyft pricing: "We got caught up in the algorithmic complexity and sweet sauce of it — we didn't consider operational requirements when building it."
- Zuck e o emoji de raiva: decidiu explicitamente não alimentar o algoritmo com reações de raiva — esse julgamento de longo prazo só um humano pode fazer.

> 🎧 [Humanizing product development | Adriel Frederick (00:38)](https://www.youtube.com/watch?v=uMhBej6-Ey4)

## Conceitos relacionados
[[A-B Testing (Ronny Kohavi)]] · [[Usuário Marginal]] · [[Empowered Teams vs Feature Teams]] · [[Rejeição Orgânica em R&D]]
