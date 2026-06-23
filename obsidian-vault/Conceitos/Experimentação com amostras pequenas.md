---
tipo: framework
fluxo: Experimentação & Dados
nivel: 3
autores: [Brian Tolkin]
---
# Experimentação com amostras pequenas

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework
**Fontes:** [[Brian Tolkin]]

## Ideia central
Quando o volume de transações é baixo (imóveis, contratos enterprise, processos de alto valor), A/B testing tradicional não é sempre viável. A solução não é abandonar rigor — é **escolher técnicas alternativas de aumento de convicção** e ser honesto sobre os limites de cada uma. Forçar falsa precisão é pior do que nenhuma análise.

## Insights por autor
### [[Brian Tolkin]]
- **Primeiro passo obrigatório: análise de poder**. Plugue tráfego esperado, efeito mínimo detectável desejado e runtime aceitável em uma calculadora de poder. Se o resultado diz "6 meses para significância", você tem uma decisão explícita a tomar — não um experimento automático.
- **Experimento de longa duração**: para decisões importantes onde o sinal é difícil de obter de outro jeito, configure e esqueça. Lance em junho, use os resultados para o planejamento de 2025. Aceitar 6 meses de runtime é legítimo — o erro é esperar 1 mês e agir como se tivesse resultado.
- **Alternativas quando volume é baixo**:
  - Dados observacionais com diff-in-diff
  - Cidades-irmã / mercados-gêmeos como controles naturais
  - Segmentação por geo em vez de user-level
  - Reduzir threshold de confiança para 80% quando o custo do erro é baixo
  - Holdouts de longo prazo para validar intuição pós-ship
- **Regra de ouro**: se nenhuma técnica está disponível, use julgamento — mas construa um **loop de feedback pós-lançamento** (volume de tickets de suporte, adoção da feature, NPS) para saber se estava certo.
- Não cometa o erro de "fingir significância": um resultado insignificante que você sabia que ia ser insignificante é uma falha de processo, não de produto.
- Paralelo com Uber: em alta escala, podia testar tudo. Em Opendoor (transações raras de imóveis), o mesmo rigor exige criatividade no método.

> 🎧 [Lessons from scaling Uber and Opendoor | Brian Tolkin (Head of Product at Opendoor, ex-Uber) (1:14:40)](https://www.youtube.com/watch?v=sRukk520Fds) · 2024-08-04

## Conceitos relacionados
[[A-B Testing (Ronny Kohavi)]] · [[Holdout de longo prazo]] · [[A maioria das ideias falha no teste]] · [[Hiperimportância de poucas decisões]]
