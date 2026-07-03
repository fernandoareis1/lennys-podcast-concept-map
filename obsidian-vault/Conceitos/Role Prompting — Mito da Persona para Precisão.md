---
tipo: princípio
nivel: 3
fluxo: Experimentação & Dados
autores: [Sander Schulhoff]
---
# Role Prompting — Mito da Persona para Precisão

**Tema:** [[Experimentação — AB testing & cultura]] · **Fluxo:** [[05 - Experimentação & Dados]]

Role prompting ("Você é um médico especialista com 20 anos de experiência...") é uma das técnicas mais ensinadas em prompt engineering — e também uma das mais mal compreendidas. Para tarefas de precisão em modelos modernos, ela **não produz diferença estatisticamente significativa**.

## O mito

A crença é: atribuir uma persona especialista ao modelo melhora a qualidade das respostas em tarefas que requerem conhecimento profundo.

Intuitivamente faz sentido — se você pedisse a ajuda de um médico vs. de um amigo, esperaria respostas diferentes.

## O que a pesquisa mostra

Os dados coletados por Sander Schulhoff no Learn Prompting e nos experimentos do HackAPrompt mostram:

- Em modelos modernos (GPT-4+, Claude), role prompting **não tem impacto estatisticamente significativo** em tarefas de precisão (matemática, código, raciocínio lógico, factual QA)
- O modelo já foi treinado com output de especialistas; a persona não desbloqueia conhecimento adicional que não estaria disponível de outra forma
- Em GPT-3 e modelos mais antigos, o efeito era observável — provavelmente porque few-shot não era padrão e a persona servia como sinal de calibração

## Quando role prompting FUNCIONA

Role prompting tem efeito real para **tarefas expressivas e de estilo**:
- "Escreva como Shakespeare" → muda o estilo
- "Responda como um professor paciente para crianças de 8 anos" → muda o tom e complexidade
- "Você é um escritor humorístico" → muda o tom

A distinção: personas mudam **como** o modelo se expressa, não **o que** ele sabe.

## Implicação para quem cria prompts

Tokens gastos em role prompting para tarefas de precisão são tokens desperdiçados. Redirecione para:
- Mais exemplos (few-shot)
- Contexto adicional relevante
- Instruções explícitas sobre o formato de saída desejado

A intuição "parece que deveria funcionar" é precisamente o tipo de hipótese que precisa ser testada — e os dados dizem não.
