---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Agency-Control Trade-off
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Cada ponto de autonomia que você entrega a um agente de AI é um ponto de controle que você abre mão. Para que essa troca valha a pena, o agente precisa ter **ganho confiança** por evidências reais de comportamento confiável — não por promessa tecnológica. A implicação prática: comece com alta intervenção humana e baixa autonomia; aumente a agência gradualmente apenas quando o comportamento do sistema estiver calibrado e confiável.

## Como aplicar
1. **V1 — High control, low agency:** o agente sugere, o humano executa. Logging de tudo que o humano faz diferente da sugestão.
2. **V2 — Medium control, medium agency:** o agente age em casos simples; humano só revisa edge cases ou casos de alto risco.
3. **V3 — Low control, high agency:** o agente executa end-to-end em domínios que já demonstrou confiabilidade. Humano intervém só em exceções.
4. Determine a fronteira de risco explicitamente: quais ações têm impacto irreversível (disparar e-mail, emitir reembolso, fazer cirurgia) versus reversíveis (sugerir rota de ticket).
5. Use a progressão de versões como flywheel: o logging de V1 vira dataset de treino/calibração de V2.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- Exemplo de pre-authorization em seguros de saúde: MRI e exames de sangue são casos de baixo risco onde AI pode agir autonomamente; cirurgias invasivas exigem humano no loop.
- "Você quer ter certeza que o agente ganhou sua confiança antes de deixá-lo tomar decisões."
- 74–75% das enterprises entrevistadas numa pesquisa de Berkeley citaram **confiabilidade** como maior obstáculo para deploy em produção.

### [[Kiriti Badam]]
- Analogia da escalada: você não vai ao Half Dome no primeiro dia — você treina partes progressivas até ter confiança.
- Exemplo do Codex (OpenAI): começaram com customer support sugerindo respostas a agentes humanos → depois resposta direta ao cliente → depois emissão de reembolsos automáticos.
- "Quando você começa pequeno, você é forçado a pensar: qual é o problema que estou resolvendo?"

> 🎧 [Why most AI products fail (9:53–21:31)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Non-determinismo em Produtos AI]] · [[CC/CD Framework]] · [[Humans in the Loop (algoritmos)]] · [[Empowered Teams vs Feature Teams]]
