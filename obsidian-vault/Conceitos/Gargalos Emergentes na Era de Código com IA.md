---
tipo: modelo-mental
nivel: 3
fluxo: Priorização & Roadmap
autores: [Mike Krieger]
---
# Gargalos Emergentes na Era de Código com IA

**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Priorização & foco]] · **Camada:** L3
**Tipo:** modelo mental · **Fontes:** [[Mike Krieger]]

## Ideia central
Quando IA remove um gargalo de produção (escrever código), novos gargalos emergem no processo imediatamente a montante e a jusante. O líder de engenharia ou produto que ganha velocidade de código com IA rapidamente descobre que o próximo gargalo é decisão e alinhamento (upstream) ou review e merge de PRs (downstream). Resolver o gargalo original expõe o próximo — e assim sucessivamente. Entender essa dinâmica é crítico para não ficar celebrando velocidade de implementação enquanto o sistema está congestionado em outro ponto.

## O padrão da teoria das restrições aplicado à engenharia com IA
Na Anthropic, quando Claude Code acelerou drasticamente a produção de código:
- O queue de code review e merge ficou congestionado — precisaram re-arquitetar o merge queue
- O gargalo upstream de "decisão e alinhamento" tornou-se visível porque anteriormente era mascarado pela lentidão de implementação
- Mais de 50% dos PRs sendo gerados por IA exigiu pensar diferente sobre processo de review

## Implicações para produto
- Automatizar implementação sem automatizar context e decisão cria gargalo upstream mais doloroso
- Velocidade de desenvolvimento exige velocidade equivalente de decisão — os processos de product management precisam ser redesenhados junto com os de desenvolvimento
- O bottleneck migra, não desaparece: pergunte sempre "qual é o gargalo agora?" em vez de "eliminamos o gargalo?"

## Insights por autor
### [[Mike Krieger]]
- "We had to completely re-architect [the merge queue] because so much more code was being written and so many more pull requests were being submitted. Over half of our pull requests are Claude Code generated."
- "I've just found all these new bottlenecks in our system, there's an upstream bottleneck, which is decision making and alignment... other bottlenecks emerge."
- "It's like the critical path theory... I just found all these new bottlenecks in our system."
> 🎧 [Instagram co-founder on building AI products at Anthropic (Mike Krieger)](https://www.youtube.com/watch?v=DKrBGOFs0GY)

## Conceitos relacionados
[[Gargalo como bússola de priorização]] · [[Produto na Interseção Modelo-Produto — Vantagem Única de IA]] · [[De Saber a Fazer — A Transição dos Agentes de IA]] · [[Custos de Terceira Ordem da Complexidade]]
