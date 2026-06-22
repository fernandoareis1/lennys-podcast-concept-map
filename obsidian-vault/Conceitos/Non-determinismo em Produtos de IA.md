---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Non-determinismo em Produtos de IA
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Produtos de IA diferem do software tradicional em uma propriedade fundamental: são **não-determinísticos nos dois extremos**. No input, a interface em linguagem natural permite infinitas formas de expressar a mesma intenção — o usuário não segue um fluxo previsível de botões. No output, o LLM é uma API probabilística sensível ao fraseado do prompt. Resultado: o builder não controla completamente input, processo nem output — e precisa construir produto sabendo disso.

## Como aplicar
1. Não projete para o "caminho feliz" único. Mapeie a diversidade de formas como usuários expressarão intenções similares e teste variações de prompt para as mesmas.
2. Não prometa determinismo para stakeholders. Comunique que o comportamento do sistema é probabilístico e que vai ser calibrado iterativamente (veja [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]]).
3. Invista em logging de comportamento desde o dia 1: sem observabilidade, não há calibração possível.
4. Use o não-determinismo como vantagem: a interface natural reduz o atrito de uso (barreira mais baixa que fluxos clicáveis), mas exija que a intenção seja capturada corretamente antes de agir.

## Insights por autor
### [[Aishwarya Naresh Reganti]] e [[Kiriti Badam]]
- Software tradicional: usuário tem intenção → produto converte em ação via fluxo determinístico (ex: Booking.com, seleção de filtros → reserva). Com IA, a camada intermediária é linguagem natural fluida — o mapa intenção→ação deixa de ser mapeado de antemão.
- "Você não sabe como o usuário vai se comportar com seu produto, e também não sabe como o LLM vai responder. Você está trabalhando com input, output e processo que não entende completamente."
- Com sistemas agênticos, a não-determinismo se amplifica: o agente pode encadear erros ao longo de múltiplos passos.

> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Trade-off Agência-Controle]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]] · [[Humans in the Loop (algoritmos)]] · [[Experimentação — AB testing & cultura]]
