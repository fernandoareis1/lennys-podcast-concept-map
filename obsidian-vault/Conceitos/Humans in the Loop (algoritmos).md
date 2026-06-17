---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Adriel Frederick]
---
# Humans in the Loop (algoritmos)
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Adriel Frederick]]

## Ideia central
Algoritmos de ML/IA são ferramentas que amplificam a intenção humana, não substitutos de julgamento estratégico. PMs de produtos algorítmicos têm como trabalho central definir: **o que o algoritmo decide** (otimização em tempo real) × **o que o humano decide** (objetivos, restrições, contexto estratégico). Alimentar tudo ao algoritmo sem essa divisão leva a resultados ótimos no curto prazo e desastrosos no longo.

## Como aplicar
1. Liste todas as decisões recorrentes no seu produto. Separe em: "o algoritmo pode otimizar isso" vs. "isso requer contexto estratégico/humano".
2. Para as decisões humanas, projete uma interface: quais dados essa pessoa precisa ver? Quais controles ela precisa ter?
3. Algoritmo → amplitude: executa milhares de variações da intenção do humano. Humano → direção: define objetivo, restrições, timing.
4. Cuidado com "techno utopians" que querem remover o humano do loop: algoritmos não entendem efeitos de longo prazo, não entendem como pessoas reagirão, não entendem a intenção do produto.

## Insights por autor
### [[Adriel Frederick]]
- No Lyft: o algoritmo de preços precisava de um humano para lidar com nevascas em Chicago, mudanças de concorrentes, taxas novas — eventos que o algoritmo não "via".
- Lição dura: construíram um algoritmo de pricing incrível tecnicamente, mas que não deixava operadores mudar preços com flexibilidade. Precisaram reconstruir do zero para colocar humano no loop.
- "Quando você trabalha em produtos pesados em algoritmos, seu trabalho é definir pelo que o algoritmo é responsável, pelo que as pessoas são responsáveis, e o framework para tomar decisões."

> 🎧 [Humanizing product development (1:07:26)](https://www.youtube.com/watch?v=uMhBej6-Ey4)

## Conceitos relacionados
[[Experimentação — AB testing & cultura]] · [[OEC - Overall Evaluation Criterion]] · [[Twyman's Law]]
