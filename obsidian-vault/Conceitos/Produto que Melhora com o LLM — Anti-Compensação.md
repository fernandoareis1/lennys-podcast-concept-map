---
tipo: principio
nivel: 3
fluxo: Estratégia & Visão
autores: [Tamar Yehoshua]
---
# Produto que Melhora com o LLM — Anti-Compensação

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Princípio · **Fontes:** [[Tamar Yehoshua]]

## Ideia central
Muitos times de produto, ao construir sobre LLMs, gastam energia construindo **compensações para as limitações atuais dos modelos**: guardrails para alucinações, UIs para lidar com não-determinismo, fallbacks para quando o modelo erra. Tamar Yehoshua chama isso de armadilha: **esse trabalho todo vai embora quando os modelos melhoram** — e os modelos vão melhorar.

A pergunta estratégica correta não é "como compensamos as limitações de hoje?" mas: **"o que construímos que fica ainda mais valioso quando os modelos ficarem melhores?"**

> "Too many people are building things to make up and compensate for the LLMs — all that work is going to go away. You have to understand that your differentiator is something that will continue to be there as the LLMs get better and smarter."

## O padrão errado: compensação temporária
Exemplos de apostas de diferenciação que têm vida útil curta:
- "Nossa vantagem é que verificamos manualmente cada resposta do LLM" — quando o modelo melhorar, o custo de verificação manual some como moat.
- "Nossa UI foi desenhada para mostrar confiança e incerteza porque o modelo erra muito" — quando o modelo errar menos, você perdeu sua vantagem.
- "Nosso processo de onboarding ensina o usuário a fazer bons prompts" — quando os modelos entenderem linguagem natural perfeitamente, esse onboarding não serve para nada.

Esses são investimentos corretos para funcionar hoje — o problema é tratar qualquer um deles como **diferenciador duradouro**.

## O padrão correto: vantagem que cresce com o modelo
O diferenciador certo é aquele que **se beneficia de LLMs mais capazes**:

- **Dados proprietários e contexto acumulado** — o modelo mais poderoso ainda precisa de contexto do cliente; quem tem mais contexto de alta qualidade tem mais vantagem.
- **Integrações profundas no workflow do usuário** — quando o modelo melhora, integração profunda entrega mais valor, não menos.
- **Comunidade e efeitos de rede** — se a rede cresce com o tempo, modelos melhores só amplificam o valor da rede.
- **Confiança e compliance enterprise** — segurança, auditoria e confiança corporativa não diminuem com LLMs mais capazes; pelo contrário, o escopo de uso aumenta.

No caso da Glean: o diferenciador não é compensar alucinações — é ter acesso seguro e conectado a todos os dados internos da empresa. Modelos melhores tornam esse contexto ainda mais valioso.

## A armadilha do não-determinismo enterprise
Tamar aponta um segundo problema prático ao construir para enterprise: **usuários corporativos esperam determinismo**. Software tradicional, quando dado o mesmo input, dá o mesmo output. LLMs não.

A solução não é esconder o não-determinismo — é **gerenciá-lo ativamente**:
- Mostre aos usuários o que funciona: exemplos de prompts que dão bons resultados.
- Ofereça sugestões de prompts em contextos relevantes.
- Seja explícito sobre quando o sistema pode variar e por quê.
- Ajude o usuário a calibrar expectativas sem criar a falsa impressão de determinismo.

Isso não é compensação temporária — é UX de IA que permanece relevante mesmo quando os modelos melhoram, porque a expectativa do usuário enterprise de previsibilidade não vai embora.

## Teste prático
Para cada diferenciador que você está construindo, faça a pergunta: **"Se o LLM ficasse 5× mais capaz amanhã, esse diferenciador ficaria mais ou menos valioso?"**

- Mais valioso → invista.
- Menos valioso ou neutro → trate como investimento tático de curto prazo, não como moat estratégico.

## Insights por autor
### [[Tamar Yehoshua]]
- "Too many people are building things to make up and compensate for the LLMs — all that work is going to go away."
- "You have to understand that your differentiator is something that will continue to be there as the LLMs get better and smarter."
- Gerenciar expectativas de determinismo enterprise via sugestões de prompts e exemplos do que funciona, não escondendo o não-determinismo.

> 🎧 [Lessons in product leadership and AI strategy from Glean, Google, Amazon, and Slack | Tamar Yehoshua](https://www.youtube.com/watch?v=ZoSeOltKqQk) · 2024-09-26

## Conceitos relacionados
[[Non-determinismo em Produtos de IA]] · [[Construir para o disco futuro]] · [[O Pior Modelo que Você Já Usará — Modelo Maximalismo]] · [[Destruir-se antes que Alguém o Destrua — O Imperativo da IA]] · [[Contexto como Camada Diferenciadora de Produto IA]]
