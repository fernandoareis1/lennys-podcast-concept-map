---
tipo: tática
nivel: 3
fluxo: Experimentação & Dados
autores: [Crystal Widjaja]
---
# Experimentos Wizard of Oz
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Tática · **Fontes:** [[Crystal Widjaja]]

## Ideia central
Antes de construir, simule a experiência. Um experimento Wizard of Oz cria a aparência de uma feature para testar o comportamento do usuário sem que a feature realmente exista. A maioria das ideias de produto pode ser validada assim — mais rápido, mais barato, com dados reais de comportamento.

**Os casos da Gojek:**

1. **Assinatura via WhatsApp Group:**
   Precisavam testar um produto de assinatura sem construir nada. Solução: colocaram 100 motoristas num grupo de WhatsApp, instruíram a fazer o pitch "você é o único que pode vender assinaturas", pediam que avisassem quando cliente dissesse sim. Um intern ficava no WhatsApp o dia todo adicionando vouchers manualmente no backend e debitando $10 do saldo do motorista. Resultado: validaram conversion rates esperados de um produto de assinatura real.

2. **Onboarding via screenshot:**
   Precisavam testar um novo fluxo de onboarding, mas havia muita engenharia envolvida. Solução: o designer criou um overlay mostrando como o fluxo ficaria em cima de um screenshot existente, e mandaram como mensagem in-app. Usuários interagiram como se fosse real — suficiente para validar direção.

3. **Features via Typeform:**
   Para testar quizzes de personalidade e formulários sem desenvolvimento mobile, mandavam um Typeform via mensagem in-app. Isso foi tão frequente que eventualmente perceberam que deveriam construir infraestrutura de web deployment no backend para evitar esperar um mobile release para cada teste.

**Por que 30 dados pontos são melhores que zero:**
Crystal é direta: você não precisa de significância estatística para aprender. Com 30 usuários, a tendência é a mesma que com 30.000 — a precisão aumenta com mais dados, mas a direção raramente muda. Melhor ter dado imperfeito hoje do que dado perfeito em três meses.

**A regra da ideia sem experimento:**
"Se você não testou a hipótese, não tem dados de usuários fazendo aquilo agora — a ideia é basicamente inútil, não importa o quanto faça sentido no modelo." Não basta que faça sentido de mercado ou de produto — você precisa de evidência de como usuários reais respondem.

## Como aplicar
1. **Pergunte antes de qualquer feature:** "Como posso testar a hipótese central disso sem construir nada?"
2. **Inventarie as ferramentas de simulação disponíveis:** Typeform, email, WhatsApp, mensagem in-app, screenshot + overlay, CSV + script Python
3. **Defina o mínimo de dados que muda sua decisão:** 10 usuários que convertem? 3 que completam? Determine isso antes de correr o experimento
4. **Priorize velocidade de aprendizado:** o custo de oportunidade de um experimento falhado é baixo; o custo de construir a feature errada é 10-50x maior
5. **Quando o padrão se repetir, automatize:** a Gojek percebeu que estava repetindo o Typeform tanto que fez sentido construir infraestrutura de web deployment — padrão de Wizard of Oz indica feature que vale construir

## Insights por autor
### [[Crystal Widjaja]]
- "We had a captive audience in the car, a driver with incentive to cross-sell, and validated the subscription conversion rate without building anything — just a WhatsApp group and an intern by the phone."
- "What's better than zero data points is definitely 30. Mathematically, you're going to get the same trends, just with less precision."
- "If you don't have a tested hypothesis, if you can't think of a way to run an experiment, then honestly that idea is pretty useless — maybe it makes sense to the model, but consumer sentiment is weird."
- "We realized that if we built in-app web deployment infrastructure, we wouldn't have to wait for a mobile app release to test new features. The Wizard of Oz pattern told us what to build."

## Conceitos relacionados
[[Assumption Testing]] · [[Decidir com poucos dados é melhor que com zero]] · [[Loops de feedback são uma escolha]] · [[Medição vs Insight — Instrumentação Rica]] · [[Física do Crescimento — Restrições e Alavancas]]
