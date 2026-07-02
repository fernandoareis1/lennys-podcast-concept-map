---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Nicole Forsgren]
---
# SPACE Framework — Medir Produtividade Além do Output

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** framework · **Fontes:** [[Nicole Forsgren]]

## Ideia central
A produtividade de engenharia não pode ser capturada por uma única métrica. O SPACE framework define **cinco dimensões** que se reforçam mutuamente — e a ausência de qualquer uma delas cria uma visão distorcida.

## As 5 dimensões do SPACE

| Dimensão | O que mede |
|---|---|
| **S — Satisfaction** | Satisfação com ferramentas, processos, trabalho, e time |
| **P — Performance** | Outcomes: o que foi entregue e qual o impacto? |
| **A — Activity** | Contagens de atividade: PRs, commits, deploys (útil como sinal, não como north star) |
| **C — Collaboration** | Como sistemas e pessoas se comunicam; proporção de trabalho delegado a AI vs. humanos |
| **E — Efficiency/Flow** | Conseguem entrar em flow? Qual o lead time das coisas? |

## Por que SPACE funciona na era de IA
Diferente do DORA (quatro métricas prescritivas de velocidade e estabilidade do pipeline), **SPACE não prescreve métricas específicas** — é um framework que te guia a escolher quais métricas coletar. Isso é sua força: aplica-se bem mesmo quando AI muda os workflows, porque as dimensões permanecem relevantes.

### Evolução com IA: Trust como 6ª dimensão emergente
Com IA gerando partes crescentes do código, Nicole propõe adicionar **Trust** como dimensão emergente:
- Há alucinações? Com que frequência?
- O código tem a confiabilidade esperada?
- Corresponde ao estilo e padrões do time?
- O engenheiro consegue confiar no output sem revisão pesada?

"Trust wasn't as important before, but now it's very, very front of mind."

## Métricas prescritivas vs. frameworks
- **DORA** (Deployment Frequency, Lead Time, MTTR, Change Fail Rate): métricas prescritivas, use apenas para o que foram designadas — avaliar velocidade e estabilidade do pipeline. AI não invalida isso, mas add-ons são necessários.
- **SPACE**: framework orientador — use-o para descobrir quais métricas fazem sentido no *seu* contexto.

A regra de Nicole: **"If it is a prescriptive metric, it needs to be used only in the way it was prescribed."**

## Armadilha: Lines of Code na era de IA
Linhas de código sempre foram uma métrica fraca, mas AI as tornou ativamente prejudiciais:
- "If the goal is more lines of code, I can prompt something to write the longest piece of code ever."
- LLMs tendem a ser verbose por natureza — maximizar LOC incentiva complexidade e technical debt.
- Única utilidade restante: diferenciar código humano vs. AI para analisar code survivability e qualidade downstream.

## Insights por autor
### [[Nicole Forsgren]]
- "We still want to look at satisfaction. We still want to look at performance, what's the outcome. We still want to look at activity."
- "Communication and collaboration, this is also super important because it's how our systems communicate with each other, and also how our people do."
- "Efficiency and flow: can people get in the flow? How much time does it take to do things?"
- "We can't just blindly apply the existing metrics we've used before because we'll miss super important phenomenon and changes in the way people work."

> 🎧 [How to measure AI developer productivity in 2025 | Nicole Forsgren](https://www.youtube.com/watch?v=SWcDfPVTizQ)

## Conceitos relacionados
[[Métricas Simples vs Compostas — Clareza Bate Perfeição]] · [[Métricas de Proxy para Outcomes de Longo Prazo]] · [[DevEx — Os 3 Pilares Flow, Carga Cognitiva e Feedback]] · [[Medição vs Insight — Instrumentação Rica]]
