---
tipo: tática
nivel: 3
fluxo: Experimentação & Dados
autores: [Upasna Gautam]
---
# Ensaio de Breaking News — Stress Test em Contexto Real

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Tática · **Fontes:** [[Upasna Gautam]]

## Ideia central
Antes de lançar qualquer funcionalidade crítica da plataforma, a CNN roda "breaking news dress rehearsals" — ensaios roteirizados que simulam um cenário de breaking news do início ao fim, no ritmo real de uma notícia urgente.

A lógica é simples: se o produto não consegue servir às necessidades de breaking news, é inútil. E o único jeito de saber isso com certeza *antes* da notícia real chegar é simular o contexto com a mesma pressão, os mesmos atores e o mesmo ritmo.

## Como funciona o ensaio
**Roteiro completo**: a equipe define o cenário (tipo de notícia, times envolvidos, sequência de eventos), e o ensaio começa com o disparo de um email da equipe de news-gathering — exatamente como acontece numa notícia real.

**Atores corretos**: jornalistas, editores, time de foto, suporte editorial, engenheiros e a PM estão todos presentes ou monitorando.

**Sequência real**: do email de breaking news → escrita do artigo → seleção de fotos → edição → publicação. Cada parte do workflow é executada no novo sistema, não descrita ou debatida.

**Observação paralela**: enquanto os jornalistas executam o workflow, engenheiros e time de suporte editorial observam, registram friction points e capturam feedback em tempo real.

**Objetivo declarado**: stress-testar o sistema, identificar pontos de atrito, entender até onde é possível ir com novas funcionalidades — tudo no ritmo de breaking news, não no ritmo de um meeting de product review.

## Por que isso é diferente de user testing convencional
| User testing convencional | Breaking news dress rehearsal |
|---|---|
| Usuário responde perguntas sobre o produto | Usuário *usa* o produto para fazer seu trabalho real |
| Ambiente artificial, ritmo da pesquisa | Ambiente simulado, ritmo da notícia |
| Feedback explícito e articulado | Friction revelada pelo comportamento, não pela fala |
| Duração: 45-60 min com pausas para reflexão | Duração: 3-5 min sem pausas — velocidade real |
| Difícil de agendar em locações globais | Mais fácil: é um evento com propósito claro |

## O princípio generalizável
O ensaio de breaking news é a implementação de um princípio mais amplo: **teste nas condições mais extremas do uso real, não nas condições médias**. Isso vale para qualquer produto que:
- Tem picos de uso imprevisíveis (elections, lançamentos, campanhas)
- Serve usuários que não podem parar suas tarefas para testar
- Exige zero tolerância a falha num momento crítico

A ideia de "dress rehearsal" como método de descoberta pode ser adaptada: uma startup fazendo ensaio de lançamento, um time de suporte fazendo simulação de incidente, um time de ML simulando anomalias.

## Insights por autor
### [[Upasna Gautam]]
- "You create a script and do a simulation of a breaking news scenario to stress test our platform, because all breaking news scenarios are definitely not the same either."
- "This gives us a lot of great feedback in that short amount of time at the speed of breaking news."
- "If it cannot serve the needs of breaking news, then it's useless."
- "It's a crazy amount of stuff and information you can gather in such a short span of time. It's a lot of work that goes into it for this three-minute event."
- "We have engineers and our editorial support team on hand as well — observing what's happening while it's usually me and one of our editorial stakeholders and leads facilitating the actual rehearsal part."

> 🎧 [An inside look at how CNN builds product | Upasna Gautam](https://www.youtube.com/watch?v=gRiCzfFEd7c) · 2023-02-23

## Conceitos relacionados
[[Descoberta assíncrona]] · [[Sistema de 4 Touch Points — Gestão de Usuários Indisponíveis]] · [[Engenheiros no Loop Criativo]] · [[Priming em Reuniões — Antes de Decidir, Alinhar]]
