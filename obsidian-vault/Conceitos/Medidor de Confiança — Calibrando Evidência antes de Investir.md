---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Itamar Gilad]
---
# Medidor de Confiança — Calibrando Evidência antes de Investir
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Itamar Gilad]]

## Ideia central
Times usam ICE (Impact, Confidence, Ease) para priorizar ideias — mas tendem a dar a si mesmos **8/10 de confiança baseados em opiniões**. Isso subverte o sistema: se confiança não é calibrada por evidência, o score de ICE é inútil.

O Confidence Meter é uma escala de 0 a 10 que mapeia **tipos de evidência** para **níveis de confiança** permitidos, prevenindo que opinião passe por certeza.

**A escala (do mais fraco ao mais forte):**

| Nível | Tipo de evidência | Confiança máx. |
|-------|-------------------|----------------|
| 0–0.1 | Própria convicção, pitch deck, tema estratégico ("é sobre AI!") | 0.1 |
| 0.1–1 | Revisão com colegas/stakeholders; back-of-envelope calculation | 1 |
| 1–3 | Dados anedóticos; entrevistas com poucos usuários; análise de concorrente | 3 |
| 3–5 | Pesquisas de mercado; análise de dados em escala; competitive deep-dive | 5 |
| 5–7 | Testes qualitativos: Wizard of Oz, fake door, usability com mockup | 7 |
| 7–9 | Early adopter program; alpha/beta; dog food interno | 9 |
| 9–10 | AB test / experimento controlado; stage release com holdback | 10 |

**Por que o nível de confiança determina o investimento:**
- Se confiança é 1 (back-of-envelope), não invista meses de eng — invista em um teste barato que eleva para 5-7
- Se confiança é 7 (usability test passou), você tem permissão para construir uma versão alpha
- Algumas ideias de baixíssimo risco (mudança de ordem de settings) podem ir direto para release sem escalar até 10

**O insight sobre concorrentes:** "O concorrente lançou essa feature" dá 2–3 de confiança no máximo — não valida que funciona para você ou para seus usuários. "A maioria das features de concorrentes não funciona que nem eles esperavam" é igualmente verdadeiro.

## Como aplicar
1. **Em toda reunião de priorização**: ao apresentar uma ideia com score ICE, peça ao time que determine o nível de confiança usando a escala. Se for < 3, o investimento correto não é "construir" — é "testar mais barato".
2. **Crie uma regra: confiança declara o próximo passo, não o projeto**: confiança 2 → próximo step é entrevista ou análise de dados. Confiança 5 → próximo step é Wizard of Oz ou mockup. Confiança 7 → próximo step é alpha.
3. **Use como ferramenta para dizer não diplomaticamente**: em vez de "sua ideia é ruim", diga "qual é o nível de confiança desta ideia? 1.5? Que step barato podemos rodar para chegar a 4-5 antes de comprometer sprints?"
4. **Separe experimento de teste**: experimento = tem grupo controle (A/B). Teste = não tem. Ambos sobem a confiança, mas experimento sobe mais.
5. **Saiba quando parar**: ideias de baixo risco não precisam chegar a 9. Se o impacto esperado é pequeno e o custo de rollback é zero, lance na confiança 4-5.

## Insights por autor
### [[Itamar Gilad]]
- "Teams tend to give themselves a high confidence. They say it's an eight and I'm pretty convinced, so it's eight for confidence. I found this a bit disturbing because it kind of subverts the whole system."
- "An opinion — your own self-conviction you feel it's a great idea — gives you 0.01 out of 10. Maybe you created a shiny pitch deck? Slightly harder to do but still very low confidence. Maybe you connected it to a theme — it's about AI! That makes it a good idea? Absolutely not."
- "Data could be anecdotal — you find a few data points in your data or you talk to a handful of customers. Or maybe one competitor has that same feature. In many companies I meet, if the leading competitor has this feature, validation is done. It never works honestly — you should not assume that your competitor knows what they're doing any more than you do."
- Sobre o Gmail Tabs: "One of the first early versions was actually we showed the tabbed inbox working to people. But it wasn't really Gmail, it was just a facade of HTML and behind the scenes we manually sorted their messages. People were like, 'Wow, this is actually very cool.' And that gave us some evidence to go and say, 'We should try and build this thing.'"
- "Part of the trick is knowing when to stop, not just trying to force your way all the way up when you don't have to."

> 🎧 [Becoming evidence-guided (1:12:52)](https://www.youtube.com/watch?v=aJWSn-tz3jQ) · 2023-09-21

## Conceitos relacionados
[[GIST Framework — Goals, Ideas, Steps, Tasks]] · [[ICE (priorização)]] · [[A maioria das ideias falha no teste]] · [[Assumption Testing]] · [[Experimentação — AB testing & cultura]]
