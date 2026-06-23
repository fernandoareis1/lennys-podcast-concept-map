---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Chip Huyen]
---
# O que realmente melhora apps de IA
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Chip Huyen]]

## Ideia central
Chip Huyen publicou uma tabela que viralizou porque bateu em um nervo. O gap entre o que times de IA pensam que melhora seus apps e o que realmente melhora é enorme:

**O que as pessoas pensam que melhora apps de IA:**
- Ficar atualizado com as últimas notícias de IA
- Adotar o framework agentic mais novo
- Agonizar sobre qual banco de dados vetorial usar
- Avaliar constantemente qual modelo é mais inteligente
- Fine-tunar um modelo

**O que realmente melhora apps de IA:**
- Falar com usuários
- Construir plataformas mais confiáveis
- Preparar dados melhores
- Otimizar fluxos de trabalho end-to-end
- Escrever prompts melhores

O padrão: times de IA tendem a otimizar por novidade e sofisticação técnica quando deveriam otimizar por impacto no usuário e qualidade de dados. As mesmas perguntas fundamentais de product development — quem é meu usuário, o que eles precisam, o que está impedindo o valor de chegar até eles — continuam sendo as mais importantes.

**Sobre escolher tecnologias novas:** duas perguntas críticas antes de adotar qualquer nova ferramenta: (1) Qual a diferença de performance entre solução ótima e não-ótima para esse problema? Se for pequena, o debate não vale o tempo. (2) Qual é o custo de trocar depois? Se uma tecnologia não testada trava você nela para sempre, pense duas vezes.

## Como aplicar
1. **Comece com o usuário, não com a tecnologia** — "Por que precisamos ficar atualizados com as últimas notícias de IA?" É uma pergunta válida. Falar com usuários e entender feedback concretamente melhora mais apps do que qualquer upgrade de modelo.
2. **Antes de adotar nova tecnologia**: pergunte quanto ela realmente impacta performance e qual o custo de trocar. Se a resposta for "pouco" e "muito", espere.
3. **Dados > Framework** — a qualidade dos dados de treinamento e dos dados de contexto (RAG) tem mais impacto na qualidade do output do que qual modelo ou framework você usa.
4. **Prompts são código** — engenharia de prompts é subestimada. Melhorar prompts sistematicamente pode dar ganhos comparáveis a mudar de modelo.
5. **Meça o que importa** — evals bem projetados para os casos de uso mais críticos do seu produto valem mais que centenas de métricas genéricas.

## Insights por autor
### [[Chip Huyen]]
- "A pergunta que me fazem muito é 'como ficar atualizado com as últimas notícias de IA?' Eu respondo: por quê? Se você falar com os usuários que entendem o que querem ou não querem, olhar para o feedback, você pode melhorar a aplicação de formas muito, muito maiores."
- "Aqui está uma nova tecnologia. Ela não foi testada por muitas pessoas, e se você adotá-la, ficará preso nela para sempre. Você realmente quer adotá-la? Talvez queira pensar duas vezes antes de se comprometer com novas tecnologias que ainda não foram bem testadas."
- "Para qualidade de resposta pura, a preparação de dados é simplesmente muito mais impactante do que agonizar sobre qual banco de dados vetorial usar."

## Conceitos relacionados
[[RAG — Qualidade de Dados como Diferencial]] · [[Era dos evals — o eval é o PRD do modelo]] · [[Pós-treinamento como nova fronteira]] · [[Build and buy]]
