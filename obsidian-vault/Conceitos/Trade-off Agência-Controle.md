---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Trade-off Agência-Controle
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Cada grau de autonomia concedido a um agente de IA é um grau de controle humano retirado. A agência não é binária: existe um espectro que vai de "agente só sugere" até "agente executa autonomamente workflows críticos". O erro mais comum é saltar direto ao topo desse espectro antes de ter estabelecido confiança no comportamento do sistema. Autonomia deve ser **conquistada**, não assumida.

## Como aplicar
1. **Mapeie o espectro** do seu produto: V1 = alta controle / baixa agência (ex: routing, sugestões); V2 = agente drafta, humano aprova; V3 = agente executa de ponta a ponta.
2. **Suba um degrau por vez.** O critério para avançar: você parou de ver novos padrões de comportamento inesperado no degrau atual.
3. **Restrinja por domínio/risco**: alguns tópicos (ex: cirurgia) nunca chegam a V3; outros (ex: blood tests de rotina) chegam rápido. Decida explicitamente.
4. Ao aumentar agência, mantenha **logging do que humanos fariam** — é feedback grátis para o flywheel de melhoria.
5. Se os resultados de confiança regridem (novo modelo, mudança de comportamento de usuários), volte ao degrau anterior.

## Insights por autor
### [[Aishwarya Naresh Reganti]] e [[Kiriti Badam]]
- Analogia: "É como treinar para subir o Half Dome. Você não vai para o Yosemite todo dia. Você começa por partes menores e melhora progressivamente."
- Exemplo de pré-autorização de seguros: IA pode aprovar MRIs rotineiros autonomamente (baixo risco), mas cirurgias invasivas precisam do humano (alto risco). A linha varia por caso.
- 74–75% das empresas entrevistadas em pesquisa da UC Berkeley/Databricks citaram **confiabilidade** como principal barreira para deploy de produtos de IA para usuários finais.
- "Não se trata de ser a primeira empresa a ter um agente entre seus concorrentes. Trata-se de ter construído os flywheels certos para melhorar ao longo do tempo."

> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Non-determinismo em Produtos de IA]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]] · [[Humans in the Loop (algoritmos)]] · [[Estratégia — Estratégia de produto]]
