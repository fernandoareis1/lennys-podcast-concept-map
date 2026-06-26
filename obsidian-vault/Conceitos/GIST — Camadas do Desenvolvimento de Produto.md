---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Itamar Gilad]
---
# GIST — Camadas do Desenvolvimento de Produto
**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Estratégia vs execução]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Itamar Gilad]]

## Ideia central
GIST é um meta-framework que organiza o desenvolvimento de produto em quatro camadas hierárquicas. Cada camada responde a uma pergunta diferente e exige instrumentos diferentes. A maioria dos problemas de produto pode ser diagnosticado identificando em qual camada a organização está falhando.

## As 4 camadas

### G — Goals (Metas)
O que estamos tentando alcançar? Camada de **outcomes**, não de outputs.
- Ferramentas: OKRs, North Star metric, árvore de métricas, top KPI de negócio
- Sinal de disfunção: metas vagas, muitas, focadas em output ("lançar 10 features") em vez de outcome ("aumentar retenção em 15%")

### I — Ideas (Ideias)
Hipóteses sobre como alcançar as metas. Fundamentalmente incertas — a ideia mais brilhante pode ser errada.
- Ferramentas: ICE score, Medidor de Confiança, assumption mapping
- Sinal de disfunção: roadmaps de features fijas, débito de ideias (sempre as mesmas vozes determinam o que entra), falta de priorização explícita

### S — Steps (Passos)
Maneiras de implementar e validar a ideia simultaneamente — loops de build-measure-learn.
- Ferramentas: testes de baixa fidelidade (fake door, Wizard of Oz, smoke tests), alpha/beta, A/B testing, stage releases
- Não são sprints de engenharia — são **marcos de aprendizado**: ao final de um passo, a equipe sabe mais sobre se a ideia funciona
- Sinal de disfunção: pouca experimentação, e mesmo quando existe experimentação, pouco aprendizado

### T — Tasks (Tarefas)
Trabalho granular gerenciado em Kanban, Jira, GitHub Issues. O que dev teams focam no dia a dia.
- Sinal de disfunção: engenheiros focados em story points e outputs, sem senso de por que o trabalho importa para o objetivo maior

## O GIST Board (nível de time)
Ferramenta prática para o dia a dia do time:
- **Direita**: 3-4 key results do time (da camada Goals)
- **Centro**: Ideias priorizadas por ICE score
- **Esquerda**: Próximos passos para validar cada ideia
- **Revisão**: A cada 2 semanas para ajustar com base em aprendizados

"Se você tem isso, cria muito mais contexto na mente do time. Eles precisam fazer menos perguntas. Você precisa dizer menos o que fazer. Eles sabem o que é sucesso."

## Onde está seu maior problema?
| Sintoma | Camada afetada | Por onde começar |
|---|---|---|
| Metas vagas ou focadas em output | Goals | North Star metric, árvore de métricas |
| Debates infinitos sobre ideias | Ideas | ICE score, Medidor de Confiança |
| Muito build, pouco aprendizado | Steps | Validações de baixo custo |
| Time desengajado | Tasks | GIST board, missão por KR |

"Se a transformação é grande demais, você vai se fatigar e apenas criar muito processo para muitas pessoas sem ver resultados — e em um trimestre vai desistir."

## Insights por autor
### [[Itamar Gilad]]
- "São quatro áreas que você precisa olhar e perguntar: estamos fazendo a coisa certa em cada uma?"
- "O passo não é um marco de engenharia ou de design — é um marco de aprendizado. Construímos algo e ao longo do caminho crescemos o escopo do que construímos."
- "Se você tem o GIST board, cria muito mais contexto na mente do time e eles precisam fazer menos perguntas. Você precisa dizer menos o que fazer. Eles sabem o que é sucesso."
> 🎧 [Becoming evidence-guided (0:21:26)](https://www.youtube.com/watch?v=aJWSn-tz3jQ)

## Conceitos relacionados
[[Evidence-Guided vs. Opinion-Based]] · [[ICE Score e o Medidor de Confiança]] · [[Outcome Roadmap vs. Release Roadmap]] · [[OKRs]] · [[Empowered Teams vs Feature Teams]]
