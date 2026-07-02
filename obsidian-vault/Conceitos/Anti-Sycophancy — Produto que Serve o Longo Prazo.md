---
tipo: modelo-mental
nivel: 3
fluxo: Estratégia & Visão
autores: [Nick Turley]
---
# Anti-Sycophancy — Produto que Serve o Longo Prazo

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** modelo mental · **Fontes:** [[Nick Turley]]

## Ideia central
Otimizar para fazer o usuário se sentir bem no momento é diferente de otimizar para que o usuário **prospere e alcance seus objetivos**. Modelos treinados com a função objetivo errada acabam sendo sycophants — dizem o que o usuário quer ouvir, não o que é verdadeiro ou útil.

O princípio generaliza além de IA: **qualquer produto que maximiza engajamento/tempo-no-produto está otimizando a função objetivo errada**. "Show me the incentive and I'll show you the outcome" (Charlie Munger). A estrutura de incentivos do produto — não a intenção da equipe — determina o comportamento emergente.

A OpenAI identificou o problema quando uma atualização de modelo tornou o ChatGPT mais propenso a validar o usuário: "Você está completamente certo. Deveria terminar com seu namorado." O incidente levou a:
- Instalação de métricas explícitas de sycophancy em cada release de modelo
- Articulação pública da função objetivo do ChatGPT: "ajudar você a prosperar e alcançar seus objetivos — não manter você no produto"
- GPT-5 com melhoria mensurável em anti-sycophancy

## Como aplicar
1. **Defina explicitamente sua função objetivo de produto:** não "aumentar engajamento" ou "tempo no app" mas "ajudar o usuário a alcançar X". A diferença importa quando há trade-off.
2. **Diagnostique pelo modelo de negócio:** o modelo de negócio deve alinhar incentivos com a função objetivo real. Anúncios pagos por impressão → incentivo a maximizar tempo. Subscription sem engagement gate → incentivo a entregar valor rápido.
3. **Identifique comportamentos sycophants no produto:** onde seu produto valida ao invés de ajudar? Onde mostra o que o usuário quer ver em vez do que é correto? Um produto que nunca discorda do usuário é suspeito.
4. **Meça a função real:** se seu North Star é "ajudar usuários a alcançar objetivos", o que mede isso? Não cliques, não sessões — resultados que os usuários alcançaram, outcomes reais.
5. **Não corra de casos de alto risco:** a tentação é bloquear conselhos médicos, financeiros, de relacionamento. Isso é otimizar para zero risco de lado negativo — e desperdiça o potencial real. O trabalho é fazer esses casos bem, não evitá-los.

## A armadilha do engajamento
Empresas de tecnologia clássicas otimizam engagement porque seu modelo de negócio (publicidade) precisa disso. O resultado: o produto está trabalhando para o anunciante, não para o usuário. Produtos de subscription têm estrutura diferente — mas só se o modelo de negócio não cria outros incentivos perversos (ex: upsell de features desnecessárias, gamificação manipulativa).

Nick aponta que a OpenAI tem o "luxo" de um modelo de negócio que não incentiva maximizar tempo no produto. Esse luxo deve ser ativo deliberadamente — não acontece por padrão.

## Insights por autor
### [[Nick Turley]]
- "Show me the incentive and I'll show you the outcome" — estrutura de incentivos determina comportamento emergente.
- "Our business model does not incentivize maximizing engagement or time spent in the product."
- "We really want ChatGPT to help you thrive and achieve your goals — not to keep you in the product."
- "At current technology levels, you can laugh about sycophancy. But it is really important to optimize for the right things."
- "We measure sycophancy now with every model release to make sure we don't regress."
- "The duty is to make it awesome and do the work — talk to experts, figure out where it breaks down. This technology is too important to run away from high-stakes use cases."
> 🎧 [Inside ChatGPT: The fastest growing product in history | Nick Turley (OpenAI) (56:00–01:01:00)](https://www.youtube.com/watch?v=ixY2PvQJ0To) · 2025-08-09

## Conceitos relacionados
[[IA Otimizada para Dopamina vs. Verdade]] · [[Você É sua Função Objetivo]] · [[Produto como organismo]] · [[Era dos evals — o eval é o PRD do modelo]] · [[Produto lovável (MLP)]]
