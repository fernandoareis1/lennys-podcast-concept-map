---
tipo: tecnica
nivel: 3
fluxo: Growth & Aquisição
autores: [Austin Hay]
---
# Atribuição a prova do futuro
**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Distribuição & canais]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Austin Hay]]

## Ideia central
A maioria das empresas começa coletando UTMs e considera o problema de atribuição resolvido. Mas quando querem avançar para multi-touch attribution (MTA), descobrem que não têm os dados para fazê-lo — e precisam esperar meses para recoletá-los. A solução: **desenhe a infraestrutura de atribuição para MTA desde o dia 1**, mesmo que você só use first-touch ou last-touch agora. O custo de fazer isso certo no início é mínimo; o custo de retrofitar é enorme.

Fundo do problema: pós-iOS 14, o matching determinístico (IDFA → PII) acabou. Agora o cenário é probabilístico — redes de ads conhecem grupos, não indivíduos. Navegadores removem parâmetros de URL. Cookie blockers anulam rastreamento de terceiros. A infraestrutura certa é a única defesa contra essa erosão de dados.

## Como aplicar
1. **Colete UTMs em dois momentos**: no user attribute (no perfil do usuário: `utm_first_campaign`, `utm_last_campaign`) E nos eventos (cada page view/evento dispara os UTMs do momento, substituindo "last" a cada nova visita).
2. **Armazene parâmetros de cada rede de ads**: cada rede tem IDs próprios (Google Click ID, Facebook FPID, TikTok ID, Microsoft ID). Colete todos desde o início em uma lista mantida.
3. **Salve localmente no device**: armazene UTMs em first-party cookies/localStorage, substituindo o "last" cada vez que o usuário retorna. Isso dá o histórico completo entre sessões.
4. **Estrutura de dados warehouse**: com `utm_first_*` e `utm_last_*` no perfil do usuário + UTMs em cada evento, o time de dados consegue coalescer todas as touchpoints intermediárias e reconstruir o caminho completo para MTA quando necessário.
5. **Não espere o problema aparecer**: a pergunta não é "precisamos de MTA agora?" mas "quando precisarmos de MTA, vamos ter os dados?" Se a resposta for não, mude a arquitetura hoje.

## Insights por autor
### [[Austin Hay]]
- "A melhor prática que todo mundo deveria implantar do dia 1 é desenhar o sistema para MTA e então usar o que faz sentido conforme você cresce."
- "A maioria das pessoas só coleta UTMs e acha que seu trabalho está feito. Mas é mais complexo: você tem que pensar em primeiro e último, nos passos do meio, e projetar de forma que você está colocando no perfil do usuário e no evento."
- Pós-iOS 14: "Dos 2010 a 2020, tivemos os anos dourados do matching determinístico. Você poderia saber o IDFA e vincular à PII. Você não consegue mais fazer isso." → marketers agora trabalham com dados probabilísticos, extrapolando de 30% da população para 100%.
- "A maioria das empresas não volta para recriar a infraestrutura. Quando querem MTA depois, precisam esperar para recoletar os dados. Não faça isso."
> 🎧 [The ultimate guide to Martech (1:24:37)](https://www.youtube.com/watch?v=B79p85DHLkU) · 2023-08-13

## Conceitos relacionados
[[Holdout de longo prazo]] · [[Métricas absolutas vs. taxas de conversão]] · [[Experimentação — AB testing & cultura]] · [[Growth — Distribuição & canais]]
