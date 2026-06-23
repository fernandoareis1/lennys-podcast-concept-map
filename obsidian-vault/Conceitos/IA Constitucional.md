---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Benjamin Mann]
---
# IA Constitucional
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Benjamin Mann]]

## Ideia central
Constitutional AI é o mecanismo pelo qual a Anthropic alinha Claude sem depender de human raters para cada resposta. O processo: define-se uma **constituição** de princípios em linguagem natural (derivados da Declaração de Direitos da ONU, termos de privacidade da Apple, princípios criados internamente), pede-se ao próprio modelo que critique sua resposta inicial contra cada princípio aplicável, e o modelo reescreve a resposta para estar em conformidade — aprendendo assim a produzir respostas alinhadas por padrão.

O resultado é RLAIF (Reinforcement Learning from AI Feedback) em vez de RLHF (de humanos): a IA se auto-melhora de forma escalável e com valores explicitados publicamente, não implícitos em decisões de raters anônimos.

Um efeito colateral relevante para produto: o processo de alinhar o modelo com esses valores foi o que **criou a personalidade do Claude** — a capacidade de fazer recusas sem fechar o usuário, de mostrar empatia em conversas difíceis, de ser genuinamente útil sem ser sycophantic. Segurança e personalidade são o mesmo trabalho.

## Como aplicar
1. **Publique os princípios do seu produto**: se você tem um produto de IA, explicitar os valores que regem seu comportamento (como uma constituição) aumenta confiança de clientes e reguladores.
2. **Use o modelo para revisar o modelo**: em produtos de IA, itere com o modelo criticando seus próprios outputs antes de expor ao usuário. Frameworks de auto-avaliação reduzem custo de humanos no loop.
3. **Separe valores de comportamento**: a constituição define "o quê respeitar"; o treinamento ensina "como respeitar". Essa separação permite iterar em valores sem retreinar do zero.
4. **Envolva stakeholders na definição da constituição**: Anthropic publica e solicita input sobre a constituição — o equivalente corporativo seria incluir clientes-chave no processo.

## Insights por autor
### [[Benjamin Mann]]
- "Não queremos deixar os valores implícitos em quais human raters encontramos. Nós mesmos decidimos quais devem ser os valores desse agente."
- "O processo: o modelo gera uma resposta, verifica se cumpre o princípio constitucional, se não cumpre reescreve. Depois removemos o 'trabalho do meio' e o modelo aprende a produzir a resposta correta diretamente."
- "O caráter e a personalidade do Claude foram diretamente resultado da nossa pesquisa de alinhamento. Não é algo separado de segurança — é a mesma coisa."
- "Claude é um dos modelos menos sycophants porque colocamos enorme esforço em alinhamento real, não em otimizar métricas de engajamento."
> 🎧 Episódio com Benjamin Mann, co-founder da Anthropic (frontmatter do transcript com erro — URL não disponível)

## Conceitos relacionados
[[Non-determinismo em Produtos de IA]] · [[Teste de Turing Econômico]] · [[Software opinionado]]
