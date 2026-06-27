---
tipo: tecnica
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Jag Duggal]
---
# Bullseye Cohort — Quem Realmente Ama o Produto

**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Descoberta contínua & validação]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Jag Duggal]]

## Ideia central
Quando o produto não atinge o limiar de PMF na média, a resposta não é desistir — é **procurar o cohort interno que já ama**. Dentro de qualquer base de usuários existe um subconjunto ("bullseye cohort") cujo Sean Ellis Score dispara bem acima do limiar. Esse grupo revela o que o produto precisa ser para todos os demais: quem são, o que fazem de diferente, o que valorizam de específico.

O Nubank encontrou isso no produto de pagamento automático de contas: a média estava em ~40% de "muito decepcionados", mas dentro dela havia um cohort com 4+ contas cadastradas em 2+ diferentes meios de pagamento — e o seu score subia para 70%. Essa descoberta redirecionou todo o roadmap: o problema não era automação de contas (feature genérica), mas **consolidação multi-rail** (diferença fundamental).

## Como aplicar
1. Rode o Sean Ellis Survey em todos os usuários ativos na fase inicial.
2. Não olhe só a média — segmente por comportamento (frequência de uso, profundidade de uso, tipo de caso de uso).
3. Identifique o cohort com score mais alto. Esse é o "bullseye".
4. Entrevista direta: ligue para 10 pessoas desse cohort. Até a quinta ligação você já consegue prever o que as demais vão dizer.
5. Reformule o roadmap para expandir esse bullseye até que ele se torne o segmento majoritário.
6. Monitore o Sean Ellis Score periodicamente para verificar se a expansão está funcionando.

## Insights por autor
### [[Jag Duggal]]
- No produto Assistente de Pagamentos do Nubank: usuários com 4+ contas em 2+ rails tinham Sean Ellis Score de 70% contra ~40% da média. "Esse era o bullseye."
- No Ultravioleta (cartão premium): o cohort que gastava o suficiente para ter a anuidade zerada amava o produto; os demais, não tanto. Isso guiou o design das regras de benefício.
- "Don't worry about serving 1,000 customers, taking three weeks. Just call 10 of them. Pick up the phone yourself."
- "By the time you've made your fifth call, you could predict what customers six, seven, eight, nine and ten are going to tell you."
- Ligações, não pesquisa via e-mail: "You can get tone of voice. Brazilians and Mexicans are incredibly expressive. There's a degree of real fine-grain sense that statistics never tell you."

> 🎧 [Be fundamentally different, not incrementally better | Jag Duggal (Nubank, Facebook, Google) (1:35:17)](https://www.youtube.com/watch?v=8A7wXK2MncQ) · 2024-05-16

## Conceitos relacionados
[[Sean Ellis Test (40%)]] · [[Hipótese Antes da Pesquisa]] · [[Melhores Clientes Recentes como Espelho]] · [[Máquina de Word-of-Mouth — Sinal Real de PMF]]
