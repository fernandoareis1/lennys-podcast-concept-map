---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Sri Batchu]
---
# Tradução Métrica — North Star por Camadas

**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Outcomes & metas]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Sri Batchu]]

## Ideia central
Criar uma **camada de tradução** que converte a métrica local de cada sub-time na north star da empresa. Cada time opera no dia a dia com sua própria métrica — mas para planejamento, cross-priorização e alocação de recursos, tudo colapsa para uma moeda comum.

## O problema que resolve
Em organizações de growth com múltiplos times (paid, lifecycle, ativação, SEO, etc.), as equipes otimizam métricas locais. Sem uma camada de tradução, não há como comparar: "vale mais alocar um engenheiro para o time de checkout ou para o time de busca?"

Com a tradução, a resposta vira: "qual desses gera mais MAO (ou pipeline SQL, ou outra north star) por unidade de recurso?"

## Como funciona

1. **Definir a north star** da empresa (1-2 métricas; uma de volume, uma de eficiência)
2. **Mapear as métricas locais** de cada time (load time, conversão de checkout, N buscas por sessão, etc.)
3. **Calcular o fator de tradução** para cada métrica: "se melhorarmos X em 1 ponto, qual é o impacto esperado na north star?" (via regressão ou holdout de longo prazo)
4. **Usar a tradução para planejamento e cross-priorização** — não para decisões marginais do dia a dia

## Casos concretos

**Instacart** — North star: Monthly Active Orderers (MAO)
- Time de checkout tinha sua métrica de conversão local
- Mas a pergunta de alocação era: "1 ponto de conversão no checkout = quantos MAO adicionais?"
- Fator atualizado a cada 6 meses com dados mais recentes

**Ramp** — North star: dollars de SQL pipeline
- Se o time de website muda copy na landing page, o impacto direto é conversão de formulário
- A tradução diz: "2 bips de conversão = X dólares de SQL pipeline"
- Isso determina se o projeto vale o esforço versus outras iniciativas

## Regras de uso
- Não usar para **decisões marginais** (5-10% de diferença) — nesses casos, use julgamento
- Atualizar os fatores de tradução periodicamente (ex: a cada 6 meses) com dados novos
- Usar holdouts de longo prazo para validar as traduções empiricamente

## Insights por autor
### [[Sri Batchu]]
- "We have a translation layer for every team's metric into MAO. It would be like if you got one extra weekly order from the same customer, it would have point X impact on the company's MAO."
- "The framework helped with reducing the cognitive overload of decision making to only those that are marginal. The ones that are obvious with big impact become clear even if the measurement framework isn't perfect."
- "We update all of the translations every six months for the new planning cycle based on new information."
- "For planning and resource allocation and reporting, we use the translation layers to look at everything on a MAO basis."

> 🎧 [Lessons from scaling Ramp | Sri Batchu (Ramp, Instacart, Opendoor)](https://www.youtube.com/watch?v=RcYCU5UAZOk) · 2023-06-25

## Conceitos relacionados
[[Seis Regras de Metas Claras — Foco como Comunicação]] · [[Estrutura de Impacto em Três Degraus]] · [[Visão e Missão Cascateada para Times de Growth]] · [[OKRs (Christina Wodtke)]]
