---
tipo: framework
nivel: 3
fluxo: Design & UX
autores:
  - Gustav Söderström
---
# 🎯 UI Tolerante a Falhas — Projetar para a Performance do ML

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3 (Conceito)

**Autor:** [[Gustav Söderström]]

---

## A ideia central

A interface de usuário deve ser projetada para a **performance real** do seu modelo de machine learning — não para a performance ideal que você deseja ter.

Se o seu sistema de recomendação acerta 1 em cada 4 sugestões, construir uma UI que mostra um único item (apostando tudo em 1 resultado) garante frustração 75% do tempo. A UI correta para esse nível de performance mostra 4 itens simultaneamente.

## O exemplo do Midjourney

O Midjourney estreou mostrando 4 imagens em baixa resolução lado a lado. Parecia limitação técnica — era design inteligente. A performance do modelo era aproximadamente 1 em 4; ao mostrar 4 resultados, a probabilidade de ao menos um ser bom subia dramaticamente. Só depois de identificar o "vencedor" o usuário pedia alta resolução.

Isso é UI tolerante a falhas: o design absorve a incerteza do modelo em vez de expô-la como falha do produto.

## O botão de play único — o mito

O Spotify levou anos para entender isso internamente. O instinto de produto queria um único "botão de play mágico" que tocasse exatamente o que o usuário queria. O problema: para isso funcionar, a precisão do modelo precisaria ser literalmente 100% — ausência total de erro preditivo.

> "If you're going to have a single play button, the quality of your machine learning needs to be literally 100% or zero prediction error, and that's never the case." — Gustav Söderström

A UI que apostava no single play button falhava silenciosamente. Usuários não sabiam se o algoritmo era ruim ou se haviam tocado no botão errado.

## O princípio geral

1. **Meça a taxa de acerto real** do seu modelo (não a métrica de laboratório — a taxa no produto em produção)
2. **Projete a UI para essa taxa**: se acerta 1 em N, mostre N itens
3. **Escale a aposta à medida que o modelo melhora** — não antes

Esse princípio atravessa eras (curadoria, recomendação, geração) e categorias (música, vídeo, e-commerce).

## Conceitos relacionados
- [[Curation para Recommendation para Generation — As 3 Eras da Internet]] — cada era tem sua taxa de acerto característica
- [[Non-determinismo em Produtos de IA]] — o output não-determinístico é a realidade que a UI precisa absorver
- [[Recall vs. Discovery — A Dicotomia da Homepage]] — diferentes modos de uso têm diferentes tolerâncias a falha
