---
tipo: insight
nivel: 3
fluxo: Growth & Aquisição
autores: [Ramesh Johari]
---
# Rating Inflation e Fairness Distribuicional
**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Modelos de crescimento]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Ramesh Johari]]

## Ideia central
Sistemas de rating em marketplaces têm dois problemas crônicos e relacionados: **inflação ao longo do tempo** e **injustiça distribuicional com novos entrantes**. A média simples de ratings — padrão em praticamente todo marketplace — é uma escolha de design com consequências sérias sobre quem sobrevive na plataforma.

**Rating inflation:**
Ratings sobem sistematicamente ao longo do tempo por dois mecanismos:
1. **Reciprocidade:** avaliar alguém negativamente tem custo social (você está interagindo com essa pessoa). É "quase gratuito" dar 5 estrelas
2. **Normatização:** à medida que a média sobe, 4 estrelas passa a ser percebido como "punindo" — o referencial muda

O resultado: com o tempo, a distribuição de ratings comprime no topo, tornando menos informativa.

**Fairness distribuicional — o problema do novo entrante:**
Com média simples, uma avaliação negativa no início da trajetória de um vendedor é devastadora:
- Pesquisa empírica no eBay: primeiro rating negativo → queda de 8% na receita esperada imediata
- Risco significativo de saída da plataforma logo após o primeiro rating negativo

O marketplace perde supply valioso porque o sistema de rating não tem "memória de incerteza" — trata o primeiro review com o mesmo peso do centésimo, sem considerar que o novo entrante pode ter simplesmente tido azar.

**Solução: prior Bayesiano**
Em vez de média pura, use uma média ponderada que inclui uma **crença prévia** sobre o desempenho esperado (similar à abordagem de regularização). O prior "puxar" o rating de novos entrantes para a média do mercado até acumular evidência suficiente — dando chance de recuperação sem distorcer quem tem muitos reviews.

Aplica-se o mesmo princípio ao aprendizado em A/B tests: o resultado de um experimento não deve ser interpretado isoladamente, mas no contexto do que todos os experimentos anteriores ensinaram.

## Como aplicar
1. **Identifique inflação:** plote a mediana dos ratings ao longo do tempo por safra de supply. Se sobem sem melhora de qualidade, há inflação
2. **Redesenhe os labels de rating:** em vez de "ruim → excelente", use âncoras relativas ("excedeu expectativas", "como comparado à melhor experiência que você teve?")
3. **Separe novos entrantes:** considere exibir ratings só após acumular N mínimo de reviews, ou mostrar range de confiança em vez de média
4. **Implemente prior bayesiano:** faça o rating inicial de cada novo seller/provider começar na média do marketplace com alta incerteza, se movendo gradualmente com evidência acumulada
5. **Meça "som do silêncio":** inclua reviews não-deixados no denominador da métrica (taxa de resposta) — ausência de review é um sinal que deve entrar no modelo

## Insights por autor
### [[Ramesh Johari]]
- Rating inflation é ubíqua: oDesk, Uber, qualquer marketplace com review ao longo do tempo mostra esse padrão
- "There's a lot of information in ratings that are not left" — conceito de "sound of silence" (Steve Tadelis, eBay)
- Primeiro review negativo no eBay → 8% de queda imediata em receita esperada + preditor de exit da plataforma
- "The concept of averaging has some pretty important distributional consequences for who wins, who loses in the marketplace."
- Double-blind reviews (Airbnb, liderado por Lenny Rachitsky): esconder o review até que ambos avaliem → aumentou review rate significativamente, mais dados para o sistema
- "I believe pretty strongly in this distributional fairness element of designing rating systems. I think it's been understudied."
> 🎧 [Marketplace lessons from Uber, Airbnb, Bumble, and more | Ramesh Johari (1:23:36)](https://www.youtube.com/watch?v=BVzTfsUMaK8)

## Conceitos relacionados
[[Liquidez do marketplace]] · [[Marketplaces como Remoção de Transaction Costs]] · [[Predição vs. Causalidade em Dados]] · [[Experimentação como Disciplina Científica]]
