---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Troca Agência-Controle em IA

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Toda vez que você dá a um sistema de AI mais **agência** (capacidade de tomar decisões autonomamente), você abre mão de **controle**. Não existe almoço grátis: agência e controle são inversamente proporcionais. O erro mais comum é ir direto para alta agência (agentes totalmente autônomos) antes de o sistema ter **ganhado confiança**. A abordagem correta é construir em versões progressivas, cada uma aumentando agência apenas quando a versão anterior demonstrou confiabilidade suficiente.

## Como aplicar

### Escada de agência (exemplo: customer support)
| Versão | Agência | Controle | O que o sistema faz |
|--------|---------|----------|---------------------|
| V1 | Baixa | Alta | Classifica e roteia tickets para o departamento certo — humano mantém controle total |
| V2 | Média | Média | Sugere rascunhos de resposta; humano edita e envia (copilot) |
| V3 | Alta | Baixa | Resolve tickets de ponta a ponta autonomamente |

### Critério para subir de nível
- Você **não está mais descobrindo novas distribuições de comportamento do usuário** — as iterações recentes não surpreendem.
- Os humanos no loop estão usando os rascunhos/sugestões com poucas alterações.
- Métricas de confiabilidade estão estáveis e seus padrões de falha são compreendidos.
- Sensação de "não estou mais aprendendo muito aqui" = hora de aumentar agência.

### Como constrainar agência
- **Por número de ações:** agente pode tomar até N ações antes de pedir confirmação humana.
- **Por domínio/tópico:** autorizar autonomia em domínios de baixo risco (FAQ, roteamento) antes de domínios de alto risco (reembolsos, mudanças de conta).
- **Por complexidade:** casos simples autônomos; casos com múltiplos critérios ou histórico ambíguo precisam de humano.
- Exemplo médico: AI aprovando exames de sangue e MRI de rotina (baixo risco) vs. cirurgias invasivas (humano obrigatório).

### O flywheel implícito
Cada versão com mais controle humano é também uma coleta de dados gratuita: você está **logando o que os humanos fariam** que o AI não faria corretamente. Esse dado alimenta as melhorias para a próxima versão. Não pule versões: você perde essa observação estruturada.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Every time you hand over decision-making capabilities to agentic systems, you're kind of relinquishing some amount of control on your end. And you want to make sure that the agent has gained your trust or is reliable enough that you can allow it to make decisions."
- "It's not about being the first company to have an agent among your competitors. It's about: have you built the right flywheels in place so that you can improve over time?"
- Aprendeu da forma difícil: construiu um agente de customer support end-to-end que teve que ser desligado por excesso de hotfixes incontroláveis.

### [[Kiriti Badam]]
- "When you start small and with high human control and low agency, it also forces you to think about what is the problem that I'm going to solve."
- "74-75% of enterprises have reliability as their biggest problem — that's why they're not comfortable deploying AI products to end users."

> 🎧 [Why most AI products fail | Aishwarya & Kiriti (00:09)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Não-determinismo em Produtos de IA]] · [[CC-CD (Calibração e Desenvolvimento Contínuos)]] · [[Humano no Loop Algorítmico]] · [[A-B Testing (Ronny Kohavi)]]
