---
tipo: modelo
nivel: 3
fluxo: Estratégia & Visão
autores: [Sander Schulhoff]
---
# Espaço de Ataque Infinito — Por Que 99% de Defesa é Ilusão

**Tema:** [[Estratégia — Estratégia de produto]] · **Fluxo:** [[02 - Estratégia & Visão]]

Empresas de guardrails frequentemente afirmam "bloqueamos 99% dos ataques". Esse número é estatisticamente sem sentido porque o espaço de ataque de um LLM moderno é essencialmente infinito — cada prompt possível é um potencial ataque.

## A matemática da ilusão

Para um modelo como GPT-5, o número de prompts possíveis é **1 seguido de 1 milhão de zeros**. Para referência: um googol (10^100) tem apenas 100 zeros. O espaço de ataque é maior do que isso por ordens de magnitude enormes.

99% de 1 seguido de 1 milhão de zeros = ainda basicamente infinito. O número de ataques não bloqueados é tão grande que "99% de cobertura" não tem significado defensivo real.

A amostra que as empresas de guardrails testam para chegar ao número de 99% é estatisticamente irrelevante frente ao espaço total.

## Atacantes adaptativos tornam a situação pior

Um attacker estático tentando um conjunto fixo de prompts seria gerenciável. O problema: humanos são **atacantes adaptativos** — testam, veem o que funciona, iteram. A pesquisa de Sander com OpenAI, Google DeepMind e Anthropic mostrou que humanos quebram 100% das defesas em 10-30 tentativas.

Sistemas automatizados de ataque precisam de ordens de magnitude mais tentativas para o mesmo resultado — mas ainda chegam lá.

## Problema adicional: não dissuadem atacantes

Guardrails também falham em outro objetivo potencial — dissuasão. Se um atacante está determinado a quebrar GPT-5, ele vai contornar o guardrail sem dificuldade. A barreira adicionada é trivial para qualquer atacante motivado.

## Por que empresas compram mesmo assim

O ciclo é psicológico, não técnico:
1. CISO descobre que o modelo pode gerar conteúdo malicioso (o que é verdade para todos os modelos)
2. Empresa de guardrail vende a solução
3. CISO compra — parece responsável, parece que resolveu o problema
4. Resultado real: falsa sensação de segurança que pode ser **mais perigosa** do que não ter guardrail

A confiança excessiva na proteção faz empresas implantarem agentes com poderes maiores do que implantariam sem guardrail — aumentando o dano potencial de um breach.

## O que fazer no lugar

Ver [[CAMEL — Permissão Mínima em Sistemas Agênticos]] e [[Você Não Pode Patchear um Cérebro — Segurança em IA Agêntica]]. A resposta real está em minimizar a superfície de ação dos agentes e na interseção de segurança clássica com AI security — não em guardrails.
