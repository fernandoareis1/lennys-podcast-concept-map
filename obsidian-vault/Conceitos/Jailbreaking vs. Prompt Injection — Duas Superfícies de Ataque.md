---
tipo: modelo
nivel: 3
fluxo: Estratégia & Visão
autores: [Sander Schulhoff]
---
# Jailbreaking vs. Prompt Injection — Duas Superfícies de Ataque

**Tema:** [[Estratégia — Estratégia de produto]] · **Fluxo:** [[02 - Estratégia & Visão]]

Jailbreaking e prompt injection são frequentemente confundidos, mas são ataques fundamentalmente diferentes com superfícies de risco distintas. Confundi-los leva a defesas erradas.

## A distinção

**Jailbreaking:** usuário malicioso + modelo. Não há system prompt. O usuário tenta convencer o modelo diretamente a fazer algo que não deveria — "como construir uma bomba", discurso de ódio, etc. É o cenário "eu e o ChatGPT".

**Prompt Injection:** usuário malicioso + modelo + system prompt de um desenvolvedor. O desenvolvedor construiu uma aplicação (ex: "escreva uma história") e o usuário malicioso tenta fazer o modelo ignorar essas instruções do desenvolvedor. O ataque tem como alvo o sistema de outro desenvolvedor.

**Indirect Prompt Injection:** variação mais perigosa para agentes. O ataque não vem do usuário — vem de dados externos que o agente consome (e-mails, páginas web, APIs). Quando o agente lê uma página maliciosa, essa página contém instruções que sequestram o agente.

## Por que a distinção importa para produtos

A superfície de ataque diferente exige mitigações diferentes:

| Tipo | Quem ataca | Onde mora o risco | Mitigação primária |
|------|-----------|-------------------|-------------------|
| Jailbreaking | Usuário do seu produto | Reputação + CBRN | Safety-tuning do modelo |
| Prompt injection | Usuário manipulando seu sistema | Integridade da aplicação | Validação de input + permissões |
| Indirect prompt injection | Internet/dados externos | Agente tomando ações não autorizadas | CAMEL + isolamento de contexto |

## Implicação estratégica

Chatbots que não tomam ações externas têm dano de prompt injection limitado — no pior caso, output malicioso que o usuário poderia obter no ChatGPT de qualquer forma. O risco real está em **agentes com ações**: se um agente pode ler e enviar e-mails, qualquer e-mail malicioso pode sequestrar suas próximas ações.

"Qualquer dado que o AI tem acesso, o usuário pode fazer vazar. Qualquer ação que ele pode tomar, o usuário pode fazer tomar." — Sander Schulhoff

O primeiro passo de segurança: mapear quais ações e dados cada componente agêntico do seu produto realmente precisa.
