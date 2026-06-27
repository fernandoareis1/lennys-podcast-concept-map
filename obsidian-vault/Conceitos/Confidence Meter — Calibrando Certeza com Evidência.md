---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Itamar Gilad]
---
# Confidence Meter — Calibrando Certeza com Evidência

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Itamar Gilad]]

## Ideia central
A maioria dos times superestima sua confiança em ideias ao pontuar o "C" do ICE. O Confidence Meter é uma escala de 0–10 que mapeia **classes de evidência** a graus de confiança: opiniões e decks valem 0.01–0.1; revisões de stakeholders e estimativas chegam a 1–2; dados anedóticos e de mercado chegam a 3–5; testes reais (smoke tests, protótipos, AB tests) chegam a 7–9. Usar a régua torna o debate sobre prioridade factual, não político.

## Como aplicar
- Antes de pontuar o "C" do ICE, mapeie a melhor evidência disponível para o Confidence Meter.
- Opiniões internas (mesmo do CEO): máximo 0.1.
- Validação qualitativa (12 entrevistas): ≈ 3–4.
- Teste de fumaça/Wizard of Oz: ≈ 5–6.
- AB test com resultado significativo: ≈ 8–9.
- Use o nível de confiança para decidir *quanto investir* no próximo passo — não para aprovar ou rejeitar a ideia definitivamente.
- Parar de investir quando a confiança atingir um limiar aceitável (nem sempre precisa chegar a 9).

## Insights por autor
### [[Itamar Gilad]]
- No Gmail Tabbed Inbox, usaram Wizard of Oz (manipulação manual de e-mails) para ganhar confiança suficiente antes de construir a categorização real com ML.
- Problema comum: equipes atribuem confiança 8/10 baseadas em pitch deck e aprovação do gestor — o Confidence Meter mostra que isso vale 0.1.
- "Se você rodar um experimento secreto e mostrar os dados, o fundador ou muda de ideia ou fica furioso — e o furioso provavelmente não é razoável."
- Conectar o nível de confiança ao investimento elimina o falso dilema: não precisa de AB test para mudar a ordem dos settings; precisa de muito mais para pivotal a estratégia.
> 🎧 [Becoming evidence-guided | Itamar Gilad (1:12:52)](https://www.youtube.com/watch?v=aJWSn-tz3jQ)

## Conceitos relacionados
[[GIST — Framework de Produto Orientado a Evidência]] · [[ICE (priorização)]] · [[Assumption Testing]] · [[Experimentação — Aprender com pouco e qualitativo]]
