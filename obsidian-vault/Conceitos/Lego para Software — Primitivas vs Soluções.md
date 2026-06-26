---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Ivan Zhao]
---
# Lego para Software — Primitivas vs Soluções
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Ivan Zhao]]

## Ideia central
Existe uma diferença fundamental entre dois modelos de produto de software: **Lego bricks** (primitivas composáveis que o usuário combina) versus **Lego boxes** (soluções pré-montadas com uso específico). A visão da Notion é ser caixa de Lego bricks — mas à medida que sobe o mercado (upmarket), é necessário também oferecer boxes. O erro é esquecer de manter os bricks por baixo.

"Lego is the only toy I ever wanted, and I want the same feeling of creativity and playfulness to the toy that people can use every day."

## A distinção central

### Lego Bricks (primitivas)
- Blocos simples, sem função predefinida
- O usuário decide como combinar
- Alta flexibilidade, baixo time-to-value inicial
- Exemplo: blocos da Notion, células do Excel, primitivas do Unix
- Atraem power users, desenvolvedores, empresas com workflows únicos

### Lego Boxes (soluções)
- Solução pré-montada para um caso de uso específico
- O usuário segue o template
- Baixa flexibilidade, alto time-to-value imediato
- Exemplo: templates da Notion, planilhas do Google Sheets para PME
- Atraem o mercado de massa, reduzem fricção de adoção

## A tensão upmarket
Quando o Notion começou a subir para enterprise, a pergunta era: como vender para uma empresa que quer um CRM, mas você é uma plataforma composable?

A resposta: **venda a box (solução de CRM), mas mantenha os bricks por baixo**. O cliente enterprise compra a caixa de Lego montada, mas a empresa que vende pode ajustar os bricks se necessário. O perigo é hard-code a solução e perder a flexibilidade — se o sistema de projeto da Notion tivesse sprints fixos, clientes sem sprints estariam presos.

"If you build in a Lego way... the system works for you. If not, the system works against you."

## Implicação para arquitetura de produto
A distinção bricks vs. boxes não é só go-to-market — ela afeta como você constrói:

- **Bricks-first**: cada feature é uma primitiva independente que compõe com outras; mais complexo de construir, mas cada adição multiplica o valor de todas as existentes
- **Boxes-first**: cada feature é uma solução específica; mais simples de construir, mas cada adição compete por espaço e atenção

Notion escolheu bricks-first. O custo: anos de "lost years" antes de PMF. O benefício: uma vez que o modelo composable pegou, cada novo bloco multiplicava o valor de todos os outros.

## Analogia com o Unix
A visão de pipes composáveis do Unix é o antecedente histórico. Um sistema onde ferramentas simples se compõem em fluxos complexos é mais poderoso a longo prazo do que sistemas monolíticos — mas exige que o usuário entenda composição, o que levanta a barreira de entrada.

## Insights por autor
### [[Ivan Zhao]]
- "Lego is the only toy I ever wanted, and I want the same feeling of creativity and playfulness to the toy that people can use every day."
- "If you build in a Lego way... the system works for you. If not, the system works against you."
- O risco de upmarket: "se você hard-code sprints, clientes que não usam sprints estão presos."
> 🎧 [Notion's lost years (00:16:36)](https://www.youtube.com/watch?v=IIPKMixTMfE)

## Conceitos relacionados
[[Sugar-Coated Broccoli — Embrulhar a Visão no Familiar]] · [[Bundling vs Unbundling — O Ciclo Histórico]] · [[Democratização do software via IA]] · [[Software opinionado]]
