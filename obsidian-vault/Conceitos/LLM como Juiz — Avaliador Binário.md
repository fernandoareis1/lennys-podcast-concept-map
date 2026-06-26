---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# LLM como Juiz — Avaliador Binário
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Depois de identificar os modos de falha via [[Análise de Erro com Open Coding]], o próximo passo é criar avaliadores automáticos para monitorar cada falha em escala. Um **LLM como Juiz** é um prompt altamente focado que avalia **um único modo de falha** e responde apenas **verdadeiro/falso**. A simplicidade binária é intencional: scores de 1–5 são intratáveis e não comunicam nada concreto.

O judge funciona tanto em testes offline (CI/CD antes de cada deploy) quanto em **monitoramento online** — rodando sobre amostras de traces de produção toda semana para medir a taxa de falha em tempo real.

## Como aplicar
1. **Escreva um prompt focado**: descreva exatamente um modo de falha e quando ele ocorre. Liste os critérios objetivamente. Saída: `true` ou `false`.
2. **Valide o judge contra labels humanos**: antes de publicar, compare o veredito do LLM com a sua própria avaliação manual dos mesmos traces. Use uma matriz de confusão, não apenas taxa de concordância — 90% de acordo pode esconder um juiz que nunca detecta erros raros.
3. **Itere o prompt** até os falsos-positivos e falsos-negativos caírem a um nível aceitável.
4. **Implante em dois contextos**: (a) suite de testes unitários para CI, usando traces conhecidos; (b) cron job semanal amostrado de produção para monitoramento contínuo.
5. **Mantenha 4–7 judges**, não centenas — priorize os modos de falha mais frequentes ou de maior risco ao negócio.

## Insights por autor
### [[Hamel Husain]]
- "Quando você reporta métricas, ninguém sabe o que 3.2 versus 3.7 significa. A decisão tem de ser sim ou não."
- "Antes de publicar o judge, verifique se ele concorda com o seu julgamento. Use a matriz de confusão, não só a taxa de concordância — 90% de acordo pode ser enganoso quando o erro é raro."
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

### [[Shreya Shankar]]
- "O judge avalia apenas uma coisa: é muito mais fácil do que o problema original do agente. O LLM consegue fazer isso com muita confiabilidade quando o escopo é estreito."
- "Você pode usar o judge em testes unitários OU em monitoramento online. Amostre 1.000 traces por semana e veja a taxa de falha em dados reais de produção — isso não é teste, mas é medição extremamente específica de qualidade."
- "Critérios derivam conforme você revisa outputs. Você descobre falhas que nunca teria imaginado antes de ver os dados." (do paper "Who Validates the Validators?")
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

## Conceitos relacionados
[[Análise de Erro com Open Coding]] · [[Era dos evals — o eval é o PRD do modelo]] · [[OEC - Overall Evaluation Criterion]] · [[A-B Testing (Ronny Kohavi)]]
