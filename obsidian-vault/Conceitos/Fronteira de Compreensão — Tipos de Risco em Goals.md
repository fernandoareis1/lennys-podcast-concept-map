---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Ravi Mehta]
---
# Fronteira de Compreensão — Tipos de Risco em Goals

**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Outcomes & metas]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Ravi Mehta]]

## Ideia central
"Outcomes over outputs" é uma boa orientação, mas comprometer-se com um outcome goal sem saber como movê-lo é uma armadilha. O time joga espaguete na parede, experimenta às cegas e pode mover a métrica sem entender por quê — ou não mover nada e perder a confiança do negócio.

A **Fronteira de Compreensão** é o ponto que separa o que o time sabe do que ainda não sabe. Antes de comprometer-se com um goal de outcome, é necessário entender em qual lado dessa fronteira você está. O tipo de goal deve corresponder ao tipo de risco atual:

| Risco | Diagnóstico | Goal correto |
|---|---|---|
| **Understanding risk** | Não sabemos quais são as alavancas da métrica | Goal de geração de conhecimento (ex: "mapear os 3 principais drivers de churn via qualitativo + quantitativo") |
| **Dependency risk** | Sabemos as alavancas, mas não temos as ferramentas/infra para testá-las | Goal de construção de capability (ex: "implementar o sistema de A/B test que nos permita testar X") |
| **Execution risk** | Temos tudo para executar, mas ainda não sabemos se conseguiremos executar bem | Goal de velocidade de execução (ex: "rodar 20 experimentos este trimestre") |
| **Strategic risk** | Temos hipótese sólida sobre como mover a métrica, mas ainda é hipótese | Goal de outcome com critérios claros de validação da hipótese |

## Como aplicar
1. **Diagnostique o risco atual** antes de definir o goal. Pergunte: "Se me pedirem para mover retenção em 10%, sei como fazer isso?" Se a resposta é "posso listar 10 experimentos mas não sei qual moverá a agulha" — você está em understanding risk.
2. **Resista à pressão de pular direto ao strategic risk.** Empresas experimentais e quantitativas têm o hábito de sempre pedir outcome goals. Pushback baseado em qual risco você está.
3. **Goals de understanding são legítimos e defendíveis.** "Este trimestre vamos entender o que drive retention" é um deliverable real. O produto do aprendizado — ex: um modelo de retenção com 3 alavancas identificadas — é mensurável.
4. **À medida que avança, o risco muda.** Um time que resolve understanding risk avança para dependency risk, depois execution, depois strategic. A fronteira de compreensão é móvel.

## Insights por autor
### [[Ravi Mehta]]
- "Se você pedir para eu mover retenção, posso listar 10 experimentos — mas não sei por que as pessoas continuam usando o produto. Então não faz sentido comprometer um goal de retenção, porque vou jogar espaguete na parede, algumas coisas vão funcionar, e talvez eu mova a métrica, mas não vou entender por quê."
- Os 4 tipos de risco: Understanding → Dependency → Execution → Strategic.
- "O objetivo é sempre gerar outcomes, mas às vezes há coisas que precisam acontecer antes para que você realmente entenda qual é o plano para atingir esses outcomes."
- Desenvolvido a partir de observação de múltiplas empresas que implementaram OKRs e falharam — a causa raiz frequentemente era comprometimento com outcome goals sem compreensão das alavancas.

> 🎧 [How to build your product strategy stack | Ravi Mehta (Tinder, Facebook, Tripadvisor, Outpace) (1:21:25)](https://www.youtube.com/watch?v=tncs0m5pmQg) · 2023-01-19

## Conceitos relacionados
[[OKRs (Christina Wodtke)]] · [[Outcomes vs Outputs]] · [[PM Orientado a Impacto]] · [[Product Strategy Stack — Missão ao Roadmap]] · [[Tudo no backlog é uma aposta]]
