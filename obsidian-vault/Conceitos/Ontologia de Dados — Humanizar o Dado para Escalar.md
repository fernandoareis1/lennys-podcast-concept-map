---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Nabeel S. Qureshi]
---
# Ontologia de Dados — Humanizar o Dado para Escalar

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** insight · **Fontes:** [[Nabeel S. Qureshi]]

## Ideia central
Dentro de grandes organizações, os dados existem mas são inacessíveis: tabelas com nomes ininteligíveis (tipo "S3_F1_Z"), sistemas legados como SAP que guardam informações críticas mas de forma impenetrável, e nenhuma forma de conectar esses dados a conceitos humanos reais (um avião, uma ordem de serviço, uma peça). A ontologia é a camada que mapeia tabelas técnicas para conceitos compreensíveis — e quando isso é feito corretamente, qualquer usuário consegue perguntar "onde está o avião 79?" sem saber nada de SQL. Esse insight surgiu na Palantir ao trabalhar com a Airbus e se tornou um dos maiores diferenciais do Foundry como produto.

## Como aplicar
- Antes de construir UIs, faça o mapeamento ontológico: quais são os conceitos principais do domínio do cliente?
- Identifique as entidades-chave (avião, pedido, peça, funcionário) e como elas se relacionam.
- Traduza os campos técnicos de banco de dados para termos humanos — nomes que o usuário final usaria naturalmente.
- O modelo de dados para o usuário deve esconder completamente a complexidade técnica subjacente.
- Essa camada de ontologia é reutilizável entre clientes do mesmo setor — é onde o produto se torna plataforma.

## Insights por autor
### [[Nabeel S. Qureshi]]
- "A ontologia surgiu de uma coisa muito concreta: pegávamos tabelas que poderiam ter sido escritas em linguagem alienígena — nomes como S3_F1_Z — e as mapeávamos para conceitos humanos. Uma vez que você faz isso, o usuário pode simplesmente perguntar 'onde está o avião agora?' e o produto responde."
- "Aprendemos esse 'segredo' vivendo dentro das empresas por tanto tempo. A integração de dados é brutalmente dolorosa em qualquer grande organização — e resolver isso generalizou para o produto inteiro."
> 🎧 [How Palantir built the ultimate founder factory | Nabeel S. Qureshi (founder, writer, ex-Palantir) (1:37:29)](https://www.youtube.com/watch?v=xQkSenlJvwA)

## Conceitos relacionados
[[Forward Deployed Engineer — Engenheiro no Campo]] · [[Estratégia — Estratégia de produto]] · [[RAG — Qualidade de Dados como Diferencial]] · [[Software opinionado]]

## Aprofundamento ⬇
