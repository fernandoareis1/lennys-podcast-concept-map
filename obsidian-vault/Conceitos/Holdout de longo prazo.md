---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Archie Abrams]
---
# Holdout de longo prazo
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Archie Abrams]]

## Ideia central
A maioria das análises de A/B tests para em 2 a 4 semanas. O problema: **30-40% dos experimentos que mostram lift no curto prazo não geram lift real no longo prazo**. O lift inicial frequentemente é efeito pull-forward (aceleração de ação que aconteceria de qualquer jeito) ou usuários marginais de baixo valor. A solução: **holdout de longo prazo** — manter uma coorte de controle permanente e revisitar automaticamente os resultados do experimento em 3, 6, 9 e 12 meses. Isso revela o verdadeiro impacto no negócio e cria accountability institucional.

## Como aplicar
1. **Holdout global de 5%**: mantenha 5% dos usuários em holdout permanente — eles nunca recebem as mudanças de um trimestre. Ao final do período, compare o GMV (ou sua métrica de longo prazo) desse grupo com o resto.
2. **Holdout de experimento individual**: para experimentos em novos usuários, rode 50/50 por algumas semanas, faça rollout para 100%, mas monitore a coorte que foi exposta ao experimento (não ao produto atual) por 12+ meses.
3. **Automatize revisões temporais**: a plataforma de experimentos deve notificar automaticamente responsáveis em 3, 6, 9, 12 meses com atualização de resultados. "Você não pode se esconder de como isso realmente afetou o negócio a longo prazo."
4. **Use para calibrar métricas de curto prazo**: quando você sabe que X% dos seus winners de curto prazo não se sustentam, você calibra seu nível de confiança e seus guardrails accordingly.
5. **Não paralise**: se há lift de curto prazo, ainda shippe — só não superestime o impacto. "Se você não moveu a métrica de curto prazo, não vai ter lift de longo prazo. Shippe se tiver lift; só seja razoável."

## Insights por autor
### [[Archie Abrams]]
- "Encorajo todo mundo: olhe para os experimentos que você achou que eram seus maiores winners. Olhe para as métricas downstream um, dois anos depois. Aposto que você vai se surpreender com quantas vezes a métrica é diferente do que você esperava."
- 30-40% dos experimentos: o efeito de curto prazo some ou desaparece depois de um ano. "É brutal. Provavelmente mais comum do que gostaríamos de acreditar."
- Tipos de descoberta nos holdouts: (1) lift some; (2) experimento se inverte; (3) mais raro e mais valioso — você descobriu uma coorte de merchants extremamente valiosos que suas métricas de curto prazo teriam ignorado.
- Caso de fricção monetária: reduzir fricção financeira (trials, incentivos) frequentemente parece trazer usuários de baixa qualidade no curto prazo mas causalmente aumenta sucesso de longo prazo — mais tempo para tentar = mais chance de acertar.
- Shopify usa GMV da coorte ao longo do tempo como métrica de longo prazo, não retenção — alinhado com o modelo de negócio onde alguns merchants grandes pagam pela coorte inteira.
> 🎧 [How to speak more confidently and persuasively (1:11:58)](https://www.youtube.com/watch?v=LpbBzmXrzEY) · 2024-03-31

## Conceitos relacionados
[[A-B Testing (Ronny Kohavi)]] · [[OEC - Overall Evaluation Criterion]] · [[A maioria das ideias falha no teste]] · [[Loops de feedback são uma escolha]]
