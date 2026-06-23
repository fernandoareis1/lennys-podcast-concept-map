---
tipo: framework
nivel: 3
fluxo: Growth & Aquisição
autores: [Ben Williams]
---
# Profundidade antes de amplitude
**Fluxo:** [[06 - Growth & Aquisição]] · **Tema:** [[Growth — Modelos de crescimento]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Ben Williams]]

## Ideia central
O erro mais comum na busca por PMF é expandir o escopo muito cedo. A estratégia que funciona é **ir fundo em um único persona, contexto e caso de uso antes de ir amplo**. Snyk começou apenas com desenvolvedores Node.js que queriam garantir que dependências open source eram seguras — não "desenvolvedores em geral", não "segurança em geral".

O critério do nicho não é ser pequeno — é ser **estreito o suficiente para construir uma solução verdadeiramente convincente rapidamente, mas amplo o suficiente para ter viabilidade de crescimento**. Os 2 milhões de desenvolvedores Node.js com 200.000 pacotes sendo baixados 2,5 bilhões de vezes por mês não eram um nicho pequeno — eram uma comunidade com massa crítica suficiente.

**Por que funciona**:
- Você consegue validar a solução rapidamente porque a variabilidade é baixa
- Um desenvolvedor JavaScript não vai relevar você por não suportar Golang — mas vai abandonar o produto se uma feature-chave para ele não existir
- Momentum early-stage é mais valioso que cobertura ampla
- PMF estabelecido em um nicho é a base para expansão adjacente credível

## Como aplicar
1. **Defina "persona + contexto + caso de uso" em uma frase**: não "desenvolvedores de segurança" mas "desenvolvedores Node.js construindo aplicações com open source dependencies que querem garantir que essas dependências são seguras."
2. **Resista à tentação de ampliar antes do momento certo**: o sinal de que chegou a hora de expandir é quando a retençãono nicho original está forte e você está atingindo limites naturais de crescimento nele.
3. **Escolha o nicho com base em profundidade possível + tamanho viável**: o nicho precisa ser pequeno o suficiente para você dominar, mas grande o suficiente para existir empresa ali.
4. **Valide o produto nesse nicho antes de qualquer outra coisa**: não adicione suporte para outros ecossistemas até ter os primeiros já nailados.
5. **Use a comunidade como validador contínuo**: comunidades de nicho são rápidas para dar feedback e para espalhar quando algo é bom. Se a comunidade não reage, o produto ainda não chegou lá.

## Insights por autor
### [[Ben Williams]]
- "Um desenvolvedor JavaScript simplesmente não vai se importar se você suporta Golang ou Rust, mas absolutamente vai se importar se um feature-chave como automated package upgrades não está disponível para o ecossistema dele."
- "Era estreito o suficiente para poder focar em construir uma solução convincente para um problema real, mas também amplo o suficiente para ter algo viável do ponto de vista de crescimento."
- "Nail that initial use case for that specific community — narrow enough to be able to really focus, but wide enough to be something viable from a growth perspective."
- "Não ir amplo demais cedo demais foi absolutamente crítico para o Snyk. A atração da oportunidade maior pode ser muito tentadora, mas você tem que construir tração sólida antes de lançar uma rede mais ampla."
- Expansão: suporte a novos ecosistemas virou a segunda fase após PMF no Node.js — e quando as primeiras pessoas de sales foram contratadas.
> 🎧 [How Snyk built a product-led growth juggernaut (1:31:34)](https://www.youtube.com/watch?v=21sFTZzIfUk) · 2022-11-06

## Conceitos relacionados
[[Teoria do Usuário Adjacente]] · [[Growth como sistema, não time]] · [[Kindling vs Fire strategies]] · [[Fish where the fish are — nicho e boring business]]
