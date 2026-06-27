---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Itamar Gilad]
---
# Métricas Tree — Desdobramento do North Star

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Itamar Gilad]]

## Ideia central
A Metrics Tree é uma árvore hierárquica que conecta o North Star Metric (valor entregue ao usuário) e o Top KPI (valor capturado pelo negócio) a todas as métricas intermediárias que os afetam. Ela resolve dois problemas comuns: (1) times com metas departamentais desalinhadas puxando em direções opostas; (2) incapacidade de estimar o impacto real de uma mudança específica no número que mais importa.

## Como aplicar
1. Defina **North Star Metric** = principal medida de valor entregue ao usuário (ex: WhatsApp = mensagens enviadas; Airbnb = noites reservadas).
2. Defina **Top KPI** = principal medida de valor capturado (receita, margem).
3. Expanda cada um em sub-métricas que os determinam matematicamente (funil × fatores de retenção × monetização).
4. Identifique métricas que aparecem **nos dois lados** da árvore — essas são as mais alavancadas.
5. Atribua métricas de sub-árvores a times específicos para criar ownership claro.
6. Use a árvore para estimar: "se movermos ativação 10%, o que acontece com o North Star?"

## Insights por autor
### [[Itamar Gilad]]
- A Metrics Tree separa North Star (valor ao usuário) de Top KPI (valor ao negócio) — a maioria das empresas só tem o segundo.
- Métricas que ficam na interseção das duas árvores revelam onde concentrar energia.
- A topologia de times deveria derivar da Metrics Tree, não da arquitetura do software.
- Sem a árvore, é impossível ter uma conversa racional sobre priorização — todo debate vira política.
- Exemplo: Amplitude mede "usuários de aprendizado ativo semanais" (usuários que encontraram um insight e compartilharam com 2+ pessoas) — muito mais poderoso que MAU genérico.
> 🎧 [Becoming evidence-guided | Itamar Gilad (1:12:52)](https://www.youtube.com/watch?v=aJWSn-tz3jQ)

## Conceitos relacionados
[[GIST — Framework de Produto Orientado a Evidência]] · [[North Star Metric]] · [[OKRs]] · [[Priorização — Outcomes & metas]]
