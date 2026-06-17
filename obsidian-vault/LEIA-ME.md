---
tipo: doc
---
# LEIA-ME — Como este vault funciona

## O que é
Um **mapa de conceitos** do Lenny's Podcast para o Obsidian. O eixo é o **conceito** (framework / mindset / insight), não o autor. Os autores entram como **fontes** das ideias.

## Como abrir no Obsidian
1. Instale o [Obsidian](https://obsidian.md) (grátis).
2. *Open folder as vault* → selecione esta pasta (`obsidian-vault`).
3. Comece por [[Home]] e abra a **Graph View** (Ctrl/Cmd+G).

## Estrutura
```
obsidian-vault/
├── Home.md              ← índice / entrada
├── Fluxos/              ← 10 hubs (fases do trabalho de produto)
├── Conceitos/           ← frameworks, mindsets, insights (os nós principais)
└── Autores/             ← fontes (leves; ligam conceitos no grafo)
```

## Anatomia de uma nota de conceito
- **Fluxo** a que pertence (link pro hub)
- **Ideia central** — o que é, em 2-3 linhas
- **Como aplicar** — passos práticos
- **Insights por autor** — citação + tática + link pro episódio (com timestamp quando útil)
- **Conceitos relacionados** — links que alimentam o grafo

## Camadas (profundidade progressiva)
O conteúdo é organizado em **5 camadas**: quanto mais você desce, mais denso o texto. Cada camada é uma pasta:

| Camada | Pasta | Cor no grafo | Densidade |
|---|---|---|---|
| L0 · Mapa | `Home.md` | — | índice |
| L1 · Fluxo | `Fluxos/` | 🟩 verde | ~100 palavras |
| L2 · Tema | `Temas/` | 🟧 laranja | ~120 palavras |
| L3 · Conceito | `Conceitos/` | 🟦 azul | ~300 palavras (card + aplicação) |
| L4 · Aprofundamento | `Aprofundamento/` | 🟪 roxo | 600–1200+ palavras (citações, debate, casos) |

Desça assim: **[[Home]] → Fluxo → Tema → Conceito → Aprofundamento**. No **Local Graph** de qualquer nota, aumente o slider *Depth* para revelar camada por camada.

> 🚧 *Piloto:* só o fluxo [[01 - Discovery & Pesquisa]] está no modelo de 5 camadas por enquanto. Os demais fluxos ainda estão "achatados" (Conceitos direto no hub) e serão migrados.

(cores em `.obsidian/graph.json`, aplicadas automaticamente)

## Status atual: PILOTO
8 episódios processados para validar o formato:
Bob Moesta · Teresa Torres · April Dunford · Christina Wodtke · Ronny Kohavi · Elena Verna · Casey Winters · Brian Chesky.

**Próximo passo:** validar o formato e escalar para os 303 episódios.
