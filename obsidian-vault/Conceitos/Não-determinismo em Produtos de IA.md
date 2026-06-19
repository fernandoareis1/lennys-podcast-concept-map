---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Não-determinismo em Produtos de IA

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Produtos de AI diferem do software tradicional em uma dimensão fundamental: **não-determinismo em ambos os extremos do sistema**. No software clássico, você tem um motor de decisão bem mapeado — o usuário clica por um fluxo previsível e obtém um resultado previsível. Em produtos de AI, (1) a entrada é não-determinística (usuários expressam intenções em linguagem natural de infinitas formas imprevisíveis) e (2) a saída é não-determinística (LLMs são APIs probabilísticas, caixas-pretas sensíveis a variações de prompt). Você está construindo sem saber como o usuário se comportará **nem** como o modelo responderá.

## Como aplicar

### O que muda na prática
- **Teste e observação contínuos são obrigatórios:** você não pode mapear o comportamento do produto antecipadamente como faria com software tradicional. Comportamento tem que ser **calibrado** ao longo do tempo.
- **Cobertura de edge cases é diferente:** em software clássico, você pode enumerar os estados. Com LLMs, o espaço de inputs/outputs é essencialmente infinito. A abordagem é estatística e iterativa, não exaustiva.
- **Logging é produto de primeira classe:** como você não consegue prever falhas upfront, você precisa de sistemas de monitoramento de produção robustos que captem sinais implícitos (usuário regenerou a resposta? saiu do fluxo?) além de feedback explícito.
- **Não-determinismo = oportunidade:** a mesma característica que cria imprevisibilidade também baixa a barra para o usuário — linguagem natural é mais natural do que clicar em botões. O desafio é capturar a intenção e traduzi-la em ação confiável.

### Sinal de alerta
Equipes que ignoram o não-determinismo tendem a construir sistemas muito complexos (V3 de cara) e depois descobrem que "não tem como contar todos os problemas emergentes" — Aishwarya teve que **desligar um produto** de customer support por isso: hotfixes infinitos em sistema autônomo que ninguém entendia mais.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Most people tend to ignore the non-determinism. You don't know how the user might behave with your product, and you also don't know how the LLM might respond to that."
- "You don't know how the user might behave with your product, and you also don't know how the LLM might respond to that. So you're working with an input, output, and a process — you don't understand all three very well."
- "With AI systems, it's all about behavior calibration. It's incredibly impossible to predict upfront how your system behaves."

### [[Kiriti Badam]]
- "When you start small, it forces you to think about what is the problem I'm going to solve. In all these advancements of AI, one easy slippery slope is to keep thinking about complexities of the solution and forget the problem."

> 🎧 [Why most AI products fail | Aishwarya & Kiriti (00:07)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Troca Agência-Controle em IA]] · [[CC-CD (Calibração e Desenvolvimento Contínuos)]] · [[Humano no Loop Algorítmico]] · [[DHM Model]]
