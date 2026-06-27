---
tipo: mindset
nivel: 3
fluxo: Estratégia & Visão
autores: [Ivan Zhao]
---
# Lego para Software — Produto Horizontal como Filosofia

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Mindset · **Fontes:** [[Ivan Zhao]]

## Ideia central
O princípio fundacional da Notion é ser um **"Lego para software"**: um conjunto de blocos primitivos reutilizáveis (pages, databases, views, relations) a partir dos quais qualquer pessoa pode construir praticamente qualquer ferramenta de trabalho — sem precisar programar.

Esse princípio gera duas tensões permanentes que Ivan Zhao gerencia conscientemente:
1. **Bricks vs. Boxes**: usuários hardcore querem os blocos (bricks); o mercado enterprise quer soluções prontas (boxes/Lego sets). O produto precisa entregar os dois — boxes no go-to-market, bricks no núcleo técnico.
2. **Construir em modo Lego vs. hard-code**: toda feature nova pode ser implementada como novo bloco reutilizável (mais lento, mais poderoso) ou como feature especializada (mais rápido, mas polui a arquitetura). Hard-code gera rejeição do organismo — tanto no código quanto nos usuários.

A Notion quase perdeu o rumo ao implementar "sprints" como feature hard-coded em vez de como novo bloco Lego. Demorou um ano para perceber e corrigir.

## Como aplicar
1. Antes de construir uma feature, pergunte: "isso é um novo bloco primitivo ou uma combinação de blocos existentes?"
2. Em go-to-market, empacote seus blocos em "Lego sets" (soluções verticalizadas) para segmentos específicos — mas nunca abra mão dos blocos no núcleo.
3. Use a consistência arquitetural como teste: "se este bloco novo se encaixa naturalmente com todos os outros, o sistema trabalha a favor de você. Se não, trabalha contra."
4. Para crescimento enterprise, invista em "soluções" (boxes) com ROI claro em P&L — mas mantenha a plataforma de blocos como diferenciador de longo prazo.
5. O melhor indicador de que você construiu em modo Lego: o produto permite que usuários criem coisas que você nunca imaginou.

## Insights por autor
### [[Ivan Zhao]]
- A visão vem de Douglas Engelbart (Augmenting Human Intellect) e Alan Kay (Smalltalk): não deve haver separação entre construtores e usuários — o mesmo medium deve servir a ambos.
- A estratégia B2C2B da Notion parte exatamente disso: consumidores adotam como bloco de notas, descobrem o poder dos blocos, trazem para o trabalho. Metade dos clientes B2B eram usuários pessoais antes.
- O erro corrigido em 2024: implementar sprints como feature hard-coded (não-Lego) gerou estranhamento em usuários, friccção no código e desalinhamento com o produto ao redor. Custo: ~1 ano de retrabalho.
- "Se você constrói em modo Lego dentro do Notion, o sistema trabalha por você. Se constrói de forma não-Lego, o sistema trabalha contra você."

> 🎧 [Notion's lost years, near collapse during COVID, staying small to move fast, building horizontal (1:12:18)](https://www.youtube.com/watch?v=IIPKMixTMfE)

## Conceitos relacionados
[[Brócoli com Açúcar — Esconder a Visão em Formato Palatável]] · [[Bundling e Unbundling — A Onda do Mercado]] · [[Software opinionado]] · [[Democratização do software via IA]]
