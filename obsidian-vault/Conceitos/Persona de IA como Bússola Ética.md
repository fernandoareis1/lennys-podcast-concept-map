---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Ryan J. Salva]
---
# Persona de IA como Bússola Ética

**Tema:** [[Estratégia — Estratégia de produto]] · **Fluxo:** [[02 - Estratégia & Visão]]

Quando o produto de IA entra em zonas cinzentas éticas — conteúdo ofensivo, bias, limites de linguagem — uma persona clara para a IA age como bússola que orienta as decisões de produto. A equipe do GitHub Copilot usou a metáfora do **AI pair programmer** para resolver esse problema de governança.

## O problema

Copilot no início não tinha filtros. Quando surgiu conteúdo problemático (linguagem ofensiva, comentários enviesados), o time precisava tomar decisões de produto difíceis: quais palavras bloquear? Em que contextos? Um blocklist simples é "fraught with peril" — toda palavra tem contextos onde é legítima.

A solução não foi uma política de conteúdo. Foi uma **persona**.

## A metáfora do pair programmer

> *"If Copilot is your AI pair programmer and they're whispering crazy stuff into your ear and they're bringing politics into it or gender identity into it... you're probably not going to be able to focus on your work. It's going to be really distracting."*

Um pair programmer humano sentado ao seu lado:
- Sugere código mas não toma decisões finais — você fica no controle
- Mantém foco no trabalho, não em política ou provocações
- Apoia sem substituir seu julgamento

Essa metáfora respondeu imediatamente a questões como:
- Deve bloquear essa palavra? → "Um pair programmer diria isso?"
- Deve dar uma resposta completa ou parcial? → "Um pair programmer daria acesso de uma vez ou progressivamente?"
- O AI pode ser usado para algo além de código? → "Um pair programmer saiu do escopo do trabalho"

## A transição para modelos de responsabilidade

Blocklists simples foram substituídos por modelos de detecção de "sentimento" (Responsible AI da Azure) — AI detectando AI problemática. Mas o critério avaliador continuou sendo o mesmo: "um pair programmer profissional diria isso?"

## Aplicação geral

Qualquer produto de IA se beneficia de uma persona explícita:
1. Crie uma persona com nome/metáfora clara (assistente, pair, colaborador, coach)
2. Use essa persona como filtro de decisão quando o comportamento do modelo for ambíguo
3. A persona também define o que o AI **não deve ser** (substituto, julgador, etc.)
4. Documente a persona para o time de produto usar em decisões diárias

**Princípio central:** IA deve aumentar a capacidade humana, não substituir o julgamento humano. "We do not want Copilot auto-generating code where a thinking, reasoning, breathing human being is not on the other side of that keyboard."

**Relacionado:** [[Trade-off Agência-Controle]] · [[IA Constitucional]]
