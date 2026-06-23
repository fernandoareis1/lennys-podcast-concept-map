---
tipo: tecnica
nivel: 3
fluxo: Growth & Aquisição
autores: [Ben Williams]
---
# Loop produto-conteúdo
**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Modelos de crescimento]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Ben Williams]]

## Ideia central
Um dos loops de aquisição mais poderosos para produtos B2B developer-focused é o **loop produto-conteúdo**: o produto gera conteúdo útil que aparece no ambiente natural dos usuários-alvo (GitHub, Google, etc.) e esse conteúdo traz novos usuários de volta ao produto.

**O que torna esse loop diferente de marketing de conteúdo convencional**: o conteúdo é gerado pelo próprio produto em resposta às ações dos usuários, não por uma equipe editorial. É **company-generated, company-distributed** — a empresa controla o que está sendo distribuído, mas a distribuição acontece automaticamente como parte do produto funcionando.

**Exemplo canônico do Snyk**: usuário conecta GitHub ao Snyk → Snyk escaneia o código → Snyk automaticamente cria Pull Requests para corrigir vulnerabilidades → outros desenvolvedores no repositório vêem os PRs → alguns clicam no link Snyk → criam conta → conectam seus próprios repositórios → loop continua. O conteúdo do PR educava sobre a vulnerabilidade, era branded no Snyk e incluía CTA.

**Segundo exemplo (Snyk Advisor)**: produto sidecar que indexa pacotes open source e cria páginas de "saúde" de pacote que aparecem no Google. Centenas de milhares de páginas geradas automaticamente = SEO em escala sem esforço editorial.

## Como aplicar
1. **Mapeie os outputs naturais do seu produto**: o que seu produto produz que tem valor intrínseco para quem ainda não usa seu produto? (relatórios, correções, análises, páginas de dados, notificações)
2. **Coloque esses outputs no ambiente natural do usuário-alvo**: não peça para pessoas virem ao seu dashboard — empurre o valor para onde elas já vivem (GitHub, Slack, email, Google).
3. **Inclua branding e CTA no output**: quem ver o output deve saber quem produziu e ter uma forma fácil de chegar ao produto.
4. **Feche o loop com um onboarding de baixa fricção**: de quem ver o output até quem usa o produto, o número de cliques deve ser mínimo.
5. **Meça o loop separado de outros canais**: taxa de conversão de "visualizou output externo" → "criou conta" → "ativou" é a métrica do loop, não confunda com tráfego orgânico genérico.

## Insights por autor
### [[Ben Williams]]
- "O que fazia a integração com GitHub ser única: não apenas os PRs faziam algo útil no código, mas toda a descrição explicava sobre a vulnerabilidade, educava os usuários, e era branded Snyk dizendo 'Se você acha isso útil, clique aqui.'"
- "Era ao mesmo tempo um loop de aquisição e um loop de engajamento — mantinha usuários existentes voltando e trouxe muitos usuários novos."
- Sobre controlar o conteúdo: "Não era só distribuição — nós controlávamos o conteúdo. Isso é diferente de depender de usuários para distribuir algo."
- Snyk Advisor: "Centenas de milhares de páginas geradas automaticamente. Quem busca um pacote no Google encontra nossa página, aprende sobre a saúde dele e tem um CTA para o Snyk."
- Sobre descoberta orgânica: "O Snyk Advisor era tanto um loop de aquisição quanto uma feature com valor genuíno — developers realmente queriam saber se um pacote era bem mantido."
> 🎧 [How Snyk built a product-led growth juggernaut (1:31:34)](https://www.youtube.com/watch?v=21sFTZzIfUk) · 2022-11-06

## Conceitos relacionados
[[Growth Loops vs Funil]] · [[Construir em público]] · [[Distribuição vence produto]] · [[Ciclo das novas plataformas de distribuição]]
