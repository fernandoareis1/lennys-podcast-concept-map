---
tipo: tecnica
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Jag Duggal]
---
# Segmentação Bullseye — Produto que Falhou
**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Descoberta contínua & validação]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Jag Duggal]]

## Ideia central
Quando um produto não atinge o threshold de PMF no geral (ex: Sean Ellis Score < 50%), não o mate — faça drill de segmentação para encontrar o subsegmento que **ama** o produto. Esse subsegmento é o "bullseye": o wedge para reformular o produto e expandir a partir dali. O produto que "falhou" para a massa pode ser amado por um nicho que revela o caminho certo.

## O caso Assistente de Pagamentos do Nubank
O Nubank lançou um produto de pagamento de contas (bill-pay). O score geral ficou abaixo do threshold. Decisão fácil: matar. Decisão correta: segmentar.

Ao analisar os dados por cohort, encontraram que clientes com **4+ boletos cadastrados em pelo menos 2 das 4 modalidades de pagamento** tinham Sean Ellis Score de **70%**. O produto era adorado — mas apenas por quem tinha onboarded profundamente.

A conclusão: o problema não era o produto — era o onboarding. A maioria dos usuários não tinha configurado o suficiente para experimentar o valor real. A solução: redesenhar o onboarding para que os usuários chegassem ao estado "4+ boletos em 2+ modalidades" antes de avaliar o produto.

## O framework de quatro perguntas para encontrar o bullseye
Jag Duggal usa consistentemente quatro dimensões de segmentação:

1. **Quem** — qual perfil demográfico (renda, idade, região, comportamento)?
2. **O que** — qual parte do produto estavam usando (feature específica, frequência)?
3. **Por quê** — qual dor específica o produto estava aliviando para eles?
4. **Como entraram** — qual canal, qual momento de vida, qual contexto?

A interseção dessas quatro respostas é o bullseye. Depois de encontrar, a pergunta operacional se torna: como tornamos mais fácil para mais usuários chegarem a esse estado?

## Por que funciona melhor do que matar o produto
Matar o produto desperdiça o aprendizado. Mesmo que o produto eventualmente seja descontinuado, entender o bullseye revela:
- Qual dor real existe no mercado
- Qual sub-segmento é mais receptivo
- Qual hipótese de onboarding testar

Isso acelera iterações futuras, mesmo em produtos diferentes.

## Relação com outros frameworks
- [[Sean Ellis Test (40%)]] — o score por cohort é a métrica; o bullseye é o achado quando o score geral decepciona
- [[Churn como fonte de discovery]] — as pessoas no bullseye que saem revelam o teto de valor do produto

## Insights por autor
### [[Jag Duggal]]
- "We found a small cohort with 4+ commitments on 2+ payment rails and their Sean Ellis score hit 70%."
- "The key is we need to make it easy for customers to onboard multiple bills across multiple rails." — a solução era onboarding, não o produto
- Segmentar por cohort antes de matar um produto é hábito padrão no Nubank
> 🎧 [Be fundamentally different (00:23:50)](https://www.youtube.com/watch?v=8A7wXK2MncQ)

## Conceitos relacionados
[[Sean Ellis Test (40%)]] · [[Fundamentalmente Diferente, Não Incrementalmente Melhor]] · [[Churn como fonte de discovery]] · [[Retenção com Contexto — Benchmark 60%]]
