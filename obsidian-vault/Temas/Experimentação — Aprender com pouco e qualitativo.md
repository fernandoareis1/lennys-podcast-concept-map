---
tipo: tema
nivel: 2
fluxo: Experimentação & Dados
---
# 🔬 Tema · Aprender com pouco / qualitativo

**Fluxo:** [[05 - Experimentação & Dados]] · **Camada:** L2 (Tema)

Nem tudo precisa de um experimento gigante: quebrar a ideia em **suposições** pequenas e aceitar que **decidir com pouco dado é melhor que com zero** (há loops de feedback que corrigem).

## Conceitos (L3)
- [[MVP — O Teste de Hipótese Mínimo]] — experimento mínimo para validar uma hipótese específica (não "produto mais básico")
- [[Assumption Testing]] — testar a suposição, não a ideia inteira
- [[Decidir com poucos dados é melhor que com zero]] — vire a pergunta do rigor
- [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]] — ciclo iterativo de build → deploy → calibrar para produtos de IA
- [[Loops de feedback são uma escolha]] — encurte qualquer "loop de 10 anos" identificando marcos necessários-mas-não-suficientes
- [[Experimentos Wizard of Oz]] — simule a feature sem construir: WhatsApp + interns, screenshot overlay, Typeform; 30 dados pontos > zero; tendência é estável, só a precisão muda
- [[Medição vs Insight — Instrumentação Rica]] — medição = fato sem contexto; insight = contexto + por quê + ação; eventos com 5-10 propriedades permitem segmentar o "porquê"
- [[Falha Conclusiva — Design de Experimento Definitivo]] — falha = não aprender; maximize o treatment para poder descartar a hipótese definitivamente e parar de repetir o mesmo teste
- [[Análise de erros qualitativa para produtos de IA]] — open coding → axial coding → contagem para descobrir modos de falha reais em apps de LLM
- [[Confidence Meter — Calibrando Certeza com Evidência]] — escala 0–10 que mapeia classes de evidência a graus de confiança; calibra o "C" do ICE e desacopla investimento de opinião
- [[Métricas Tree — Desdobramento do North Star]] — árvore que conecta North Star + KPI de negócio a todas as sub-métricas; revela interseções de alto impacto e cria ownership por time
- [[Pior é Melhor — Tech Debt como Problema de Champanha]] — ship a versão ingênua; você não consegue antecipar edge cases sem usuários reais; tech debt = prova de que pessoas usam o produto
- [[Diagnosticar com Dados, Tratar com Design]] — dados revelam o que está acontecendo (não o que construir); design inventa a solução; dados = quantitativo + qualitativo + comportamento social; empresas de IA crescem em "instintos e vibes" até o crescimento parar; análise conversacional requer novas metodologias
- [[Dados Sintéticos — Sem Parede de Dados no Pós-Treinamento]] — pré-treinamento tem parede de dados; pós-treinamento via RL com tarefas sintéticas não tem; Canvas foi construído com 3 comportamentos treinados sinteticamente; diversidade de dados sintéticos é a fronteira de pesquisa ativa

- [[Algoritmo de Bridging — Acordo entre Divergentes]] — buscar acordo surpresa entre divergentes como sinal mais confiável de verdade neutra
- [[Contexto é Tudo — Engenharia de Prompt Como Habilidade Humana]] — modelo tem inteligência humana mas zero contexto; crap in crap out; forneça quem você é, o que faz e o que quer antes de qualquer pergunta; smiley faces e "faça uma pausa" melhoram outputs
- [[Data-Driven como Red Flag]] — "data-driven" como dogma pode mascarar falta de pesquisa qualitativa; dados dizem o quê, não o porquê
- [[Prototipagem nos Extremos — Encontrar o Espaço Certo]] — empurre para extremos opostos de um atributo, construa ambos, e use a fricção de cada ponta para encontrar o equilíbrio real
- [[Discovery-Delivery em Paralelo, Não em Sequência]] — discovery e delivery devem ocorrer simultaneamente em loop contínuo; modelo sequencial "discovery antes do sprint" cria times que entregam com velocidade na direção errada
- [[10% Rule — Hipótese Antes da Metade]] — após 10% do tempo alocado, deve existir algo funcional que testa a hipótese central; velocidade e qualidade não são trade-offs — são ambos produto de competência
- [[Ship para Aprender — Produto Emergente de IA]] — em IA, propriedades são emergentes: só dá para saber o que polir após lançar; ship é o começo, não o fim da iteração

## Fluxos vizinhos
[[01 - Discovery & Pesquisa]]
