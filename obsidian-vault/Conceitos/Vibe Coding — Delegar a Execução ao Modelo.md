---
tipo: prática
nivel: 3
fluxo: Estratégia & Visão
autores: [Kevin Weil]
---
# Vibe Coding — Delegar a Execução ao Modelo

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Prática · **Fontes:** [[Kevin Weil]]

## Ideia central
Vibe coding (termo cunhado por Andrej Karpathy) é o modo de programar onde você deixa a IA assumir o volante — aprovando rapidamente as sugestões em vez de escrever linha a linha. O foco humano muda de **execução** para **direção e aprovação**.

**O que muda com vibe coding:**
- Antes: programador decide sintaxe, estrutura, implementação linha a linha
- Com vibe coding: programador declara intenção → IA propõe implementação → humano aprova, rejeita ou redireciona
- A velocidade de prototipagem aumenta em ordens de magnitude
- Não-programadores podem criar ferramentas funcionais

**Exemplo prático na OpenAI:**
A Chief People Officer da OpenAI (Julia) fez vibe coding de uma ferramenta interna. O CPO (Kevin) ele mesmo usa vibe coding com Windsurf. Isso sinaliza que a prática não é nicho técnico — está se tornando habilidade de líderes de produto e executivos.

**Limitação importante:**
Vibe coding funciona melhor para protótipos, ferramentas internas, demos e experimentos. Para código de produção com requisitos de segurança, performance e manutenibilidade, é necessário revisão humana mais rigorosa. O output do vibe coding é ponto de partida, não entregável final em todos os contextos.

**Conexão com democratização:**
Vibe coding é uma manifestação de [[Democratização do software via IA]] — a barreira de entrada para criar software está caindo para quase zero em intencionalidade técnica.

## Como aplicar
1. Para protótipos e ferramentas internas: use Cursor, Windsurf ou ferramentas similares no modo de aprovação rápida. Foque em articular o que quer, não como implementar.
2. Para PMs não-técnicos: vibe coding é a nova habilidade de prototipagem. Substitui (em parte) depender de engenheiro para explorar hipóteses técnicas.
3. Para líderes: incentive times a usar vibe coding para validar ideias antes de sprint planejado — reduz o custo de exploração de soluções.
4. Avalie quando vibe coding é suficiente vs. quando código human-reviewed é necessário: considere criticidade, público, manutenibilidade futura.
5. Monitore qualidade: revise o código gerado antes de ir a produção. A IA pode funcionar mas gerar dívida técnica significativa.

## Insights por autor
### [[Kevin Weil]]
- Termo cunhado por Andrej Karpathy; Kevin o adota como prática pessoal com Windsurf.
- A Chief People Officer da OpenAI fez vibe coding de uma ferramenta interna — sinal de que a prática está se expandindo além de engenheiros.
- "Vibe coding com produtos como Windsurf é super divertido. Estou me divertindo muito fazendo isso."
- Citou também Cursor como produto de respeito no mesmo espaço.
- "Está mudando a forma como todo mundo constrói produto. Nada de mais."

> 🎧 [OpenAI's CPO on why ChatGPT is the worst AI you'll ever use | Kevin Weil](https://www.youtube.com/watch?v=scsW6_2SPC4) · 2025-04-10

## Conceitos relacionados
[[Democratização do software via IA]] · [[Código como Linguagem Universal dos Agentes]] · [[AI-Driven Testing — Fronteira Subvalorizada]] · [[O Pior Modelo que Você Já Usará — Modelo Maximalismo]] · [[Dívida Técnica como Alavanca Estratégica]]
