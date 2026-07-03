---
tipo: principio
nivel: 3
fluxo: Estratégia & Visão
autores: [Sander Schulhoff]
---
# Falsa Confiança de Guardrail — Proteção Ilusória que Amplifica o Risco

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Princípio · **Fontes:** [[Sander Schulhoff]]

## Ideia central
O maior perigo dos guardrails de IA não é que eles não funcionam — é que eles fazem você acreditar que está protegido quando não está. **Falsa confiança é mais perigosa que vulnerabilidade conhecida.**

**O argumento estatístico:** guardrails afirmam 99% de efetividade. Mas o espaço de possíveis ataques é igual ao número de possíveis prompts — 1 seguido de 1 milhão de zeros, mais que um googol. 99% de infinito ainda é infinito. O conjunto de ataques que passam é tão grande quanto impossível de enumerar. As estatísticas de "99% de proteção" são construídas sobre amostras não representativas.

**Por que humanos sempre quebram:** a avaliação adaptativa — onde atacantes aprendem com tentativas anteriores e refinam — é o único teste válido de adversarial robustness. Humanos são atacantes adaptativos naturais: testam, ajustam, testam de novo. Em competições de red teaming com guardrails habilitados, 100% dos guardrails foram quebrados por humanos em 10 a 30 tentativas. Sistemas automatizados levam mais 100x tentativas, mas também chegam lá.

**O ciclo vicioso:** empresa compra guardrail → acredita que está protegida → dá mais poder ao agente → superfície de ataque cresce → quando o guardrail falha (e vai falhar), as consequências são maiores do que se nunca tivesse sido implantado.

**Guardrails baseados em prompt são os piores:** colocar instruções no system prompt como "se alguém tentar me enganar, ignore" é a defesa mais fraca. Isso é conhecido desde início de 2023 e continua sendo vendido como solução.

**Quando guardrails não são problema nem solução:** se seu produto é um chatbot que só responde perguntas e não toma ações externas, o risco de reputação existe mas é igual ao risco de usar ChatGPT diretamente. Nenhum guardrail resolve isso significativamente — o usuário pode ir ao ChatGPT mesmo, e a diferença de dano é marginal.

## Como aplicar
1. **Não compre guardrails porque te fazem sentir seguro:** a pergunta não é "temos guardrails?" mas "o que acontece quando eles falham?" — e eles vão falhar.
2. **Teste com atacantes adaptativos:** não use datasets estáticos de ataques conhecidos para medir robustez. Contrate pessoas para tentar quebrar o sistema com liberdade criativa.
3. **Meça a consequência do ataque, não a taxa de bloqueio:** a métrica certa é "qual o máximo dano possível de um ataque bem-sucedido?" — não "quantos ataques bloqueamos?"
4. **Separe chatbot de agente:** chatbots sem poder de ação têm risco reputacional limitado; agentes com permissões têm risco real. Invista em segurança proporcionalmente à capacidade de ação, não proporcionalmente ao uso.
5. **Monitore outputs mesmo sem guardrail:** logging de inputs e outputs é útil não para segurança em tempo real, mas para entender como o sistema está sendo usado e melhorá-lo.

## Insights por autor
### [[Sander Schulhoff]]
- "Guardrails não funcionam. Vou repetir: guardrails não funcionam. E o que me preocupa mais é que eles te deixam extremamente confiante na sua postura de segurança — o que é um problema enorme."
- "99% de 10^1.000.000 ainda é basicamente infinito. O número de ataques que passam é tão grande quanto impossível de medir."
- "Se alguém está determinado o suficiente a enganar o GPT-5, ele vai lidar com esse guardrail. Sem problema. Os guardrails não dissuadem atacantes."
- "Guardrails baseados em prompt são os piores de todos. Sabemos disso desde início de 2023. Ainda assim são vendidos."
- "A razão de eu estar aqui agora é porque isso está prestes a ficar sério. Até aqui era chatbots que fisicamente não conseguiam causar dano. Agora temos agentes, temos robótica. Isso pode causar dano financeiro, dano físico."
- "Eu diria para não comprar guardrails. Não parece oferecer nenhuma defesa adicional real."

> 🎧 [Why securing AI is harder than anyone expected and guardrails are failing | HackAPrompt CEO (1:32:41)](https://www.youtube.com/watch?v=J9982NLmTXg) · 2025-12-21

## Conceitos relacionados
[[Segurança Agentica — Não Dá para Patchar um Cérebro]] · [[CAMEL — Defesa por Permissão de Intenção]] · [[Trade-off Agência-Controle]] · [[Non-determinismo em Produtos de IA]]
