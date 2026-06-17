---
tipo: aprofundamento
nivel: 4
fluxo: Experimentação & Dados
conceito_pai: A-B Testing (Ronny Kohavi)
autores: [Ronny Kohavi]
---
# 📜 A/B Testing — Evidências (Ronny Kohavi)

**↑ Card:** [[A-B Testing (Ronny Kohavi)]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L4 (Aprofundamento)
**Fonte:** [[Ronny Kohavi]] — *The ultimate guide to A/B testing* (1:23:08)

> Casos, números e a mecânica completa. Versão curta no [[A-B Testing (Ronny Kohavi)|card]].

---

## O caso que virou abertura do livro
Mover a segunda linha do anúncio do Bing para a primeira (título maior) — uma ideia "meh" que ficou meses no backlog mal avaliada:

> "That simple idea increased revenue by about 12%. (…) This thing was worth $100 million at the time. (…) And the key thing is it didn't hurt the user metrics." *(05:37–07:22)*

O primeiro reflexo foi achar que era bug — **Twyman's Law** ("too good to be true, let's find a bug"). Replicaram várias vezes; era real. → [[Twyman's Law]] · [[OEC - Overall Evaluation Criterion]]

## Memória institucional (abrir em nova aba)
"Abrir o resultado em nova aba" foi testado em 2008 (Hotmail/MSN), muito benéfico — e **esquecido**. Ao chegar no Airbnb, reintroduziu e viu grandes ganhos de novo.

> "When you have winners, make sure to address them and remember them." *(09:18–10:35)*

Práticas: **reunião trimestral dos experimentos mais surpreendentes**, deck de sucessos/fracassos, histórico pesquisável. Na Microsoft, ~**20–25 mil experimentos/ano** (~100 novos *treatments*/dia). E goodui.org cataloga padrões que costumam funcionar. *(16:07–20:45)*

> Surpreendente = quando |estimativa − resultado| é grande. Foco também nos **perdedores surpreendentes**. *(17:32–18:36)*

## Ganhos vêm inch by inch
> "Most of the time the winnings are made inch by inch." O time de relevância do Bing tem meta de **+2% de OEC/ano** (somando 0,1% + 0,15%...). No Airbnb, **250 experimentos** de relevância somaram **+6% de receita** — e **92% falharam**. *(10:57–13:17)*

## Todo mundo se acha diferente (e é humilhado)
Taxas de falha reais: **Microsoft ~66% · Bing ~85% · Airbnb 92%**; Booking e Google Ads publicam 80–90%.

> "Every group that starts to run experiments always starts off thinking that somehow they're different (…) and they're all humbled." *(13:31–15:29)* → [[A maioria das ideias falha no teste]]

## Teste tudo — com portfólio
> "Any code change you make, any feature you introduce has to be in some experiment, because even small bug fixes can have surprising impact. (…) You need a portfolio — some incremental, and some high risk, high reward. (…) If you go for something big, be ready to fail 80% of the time." *(21:07–22:42)*

Aposta grande real: integrar busca do Bing com social (Twitter/Facebook) custou **100 pessoas-ano**. *(22:42–23:14)*

## O perdedor que ensina
Um novo indexador do Windows melhorava a relevância offline — mas **matava a bateria** (CPU): "something that comes from left field that you didn't expect (…) let's document it." *(18:36–19:23)*

---

## Conceitos ligados
[[OEC - Overall Evaluation Criterion]] · [[Twyman's Law]] · [[A maioria das ideias falha no teste]] · [[Assumption Testing]] · [[Decidir com poucos dados é melhor que com zero]]
