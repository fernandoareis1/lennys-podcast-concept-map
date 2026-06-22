---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Adriel Frederick, Aishwarya Naresh Reganti, Kiriti Badam]
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

## Aprofundamento ⬇
- [[Humans in the Loop (algoritmos) — Evidências]]

### [[Aishwarya Naresh Reganti]] + [[Kiriti Badam]]
- O "trade-off agência-controle": quanto mais autonomia você dá a um agente, menos controle tem. O agente precisa **ganhar confiança** antes de receber mais agência.
- Padrão em 3 estágios (ex. suporte ao cliente): V1 = sugerir ao agente humano (alta controle) → V2 = exibir resposta diretamente ao cliente → V3 = resolver ticket de forma autônoma + novas ferramentas.
- "74–75% das empresas entrevistadas tinham a confiabilidade como principal problema para não expor usuários ao produto de IA." (citando paper de Matei Zaharia, UC Berkeley/Databricks)
- Logging do comportamento humano no laço de sugestão é "error analysis de graça": o quanto do draft foi usado é um sinal direto de qualidade.
> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Experimentação — AB testing & cultura]] · [[OEC - Overall Evaluation Criterion]] · [[Twyman's Law]] · [[Non-determinismo em produtos de IA]] · [[CCCD — Calibração e Desenvolvimento Contínuos]]
