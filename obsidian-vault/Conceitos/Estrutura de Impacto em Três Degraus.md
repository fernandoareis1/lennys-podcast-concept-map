---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Matt LeMay]
---
# Estrutura de Impacto em Três Degraus

**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Outcomes & metas]] · **Camada:** L3
**Tipo:** framework · **Fontes:** [[Matt LeMay]]

## Ideia central
Um framework prático em 3 passos para alinhar qualquer time de produto a resultados de negócio reais. Em vez de deixar OKRs se cascatearem em 10 camadas de abstração até perderem sentido, cada meta de time orbita a meta da empresa em **exatamente um grau de separação** — e cada item de trabalho usa a mesma unidade de medida da meta do time.

## Os três degraus

### Degrau 1: Meta de time a um passo da meta da empresa
- **Regra**: a meta do time deve derivar diretamente da meta da empresa com no máximo um operador matemático.
  - Exemplo: empresa quer $10M de ARR → time de growth quer "converter 1.000 usuários de single-product para multi-product (que valem $X de ARR cada)."
- **Anti-padrão**: cascata de 5-10 níveis onde a conexão com a meta da empresa se perde.
- **Teste**: consegue explicar em uma frase como a meta do time contribui para a meta da empresa com um número concreto?

### Degrau 2: Impacto como pano de fundo constante
- **Regra**: recorde a meta de impacto em **cada momento** do ciclo de produto — planejamento, sprint, escrita de épicos, priorização, retrospectivas.
- **Por quê**: sem recordação ativa, o foco naturalmente deriva para features e entregáveis (output) em vez de resultados (outcome).
- **Ritual prático**: comece cada planning com "Nossa meta é X. Como o que estamos planejando move X?"

### Degrau 3: Mesma unidade de medida em toda a priorização
- **Regra**: ao estimar impacto de iniciativas (ICE, RICE, etc.), use a mesma unidade da meta do time — não pontos abstratos de impacto.
- Exemplo: se a meta é "converter 1.000 usuários de single-to-multi", estime cada iniciativa em número de conversões esperadas. "Esta feature converte ~200 usuários" vs "este experimento converte ~50 usuários."
- **Resultado**: comparações de priorização tornam-se concretas e honestas; trade-offs ficam visíveis.

## Como aplicar
- **Reescreva as metas do time** usando a fórmula: [Meta da empresa] × [Contribuição do time] = [Meta do time] (uma frase, um número).
- **Adicione uma slide de impacto** no início de cada planning — não o que o time vai fazer, mas o que o time vai alcançar.
- **Revise a unidade de medida** da priorização. Se o time usa "pontos de impacto" abstratos, converta para a unidade da meta (usuários, receita, retenção).
- **Crie um painel único**: meta do time + métrica de progresso atual + gap para fechar. Mantenha visível para todo o time.
- **Use o framework para rejeitar trabalho**: "Qual é o impacto esperado dessa iniciativa em nossa meta de X?" — se a resposta for vaga, o trabalho provavelmente pertence à [[Espiral da Morte de Baixo Impacto]].

## Insights por autor
### [[Matt LeMay]]
- "The first step... in setting team goals, no more than one step away from company goals. Don't let it get cascaded into oblivion."
- "If you have a team goal of converting a certain number of single-product users to multi-product users, and you know exactly how much revenue is on the line, that number informed every decision that was made by that team for the rest of the year."
- "Step three is to connect every bit of work back to impact... are we estimating and measuring impact in the same unit of measure as our goals? Because if we're doing that, then we're keeping ourselves honest."
> 🎧 [The one question that saves product careers (1:32:09)](https://www.youtube.com/watch?v=ts9ZvlkeWGs)

## Conceitos relacionados
[[Pergunta Salvadora do CEO]] · [[Espiral da Morte de Baixo Impacto]] · [[OKRs (Christina Wodtke)]] · [[PM Orientado a Impacto]] · [[Métricas de input vs. output]]
