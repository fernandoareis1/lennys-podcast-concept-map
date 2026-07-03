---
tipo: conceito
nivel: 3
fluxo: Founder & Carreira
autores: [Sander Schulhoff]
---
# IA Security como Campo Híbrido — Cybersegurança Encontra IA

**Fluxo:** [[10 - Founder & Carreira]] · **Tema:** [[Founder — Carreira & progresso]] · **Camada:** L3
**Tipo:** Conceito · **Fontes:** [[Sander Schulhoff]]

## Ideia central
A segurança de IA não é só cybersegurança clássica com um modelo novo, nem só pesquisa de AI safety. É um campo híbrido emergente que requer os dois — e a intersecção é onde o trabalho de maior valor acontece.

**O blind spot do profissional clássico de segurança:** ele olha para um sistema que usa LLM para executar código e faz todas as perguntas certas de cybersec — acesso de rede, permissões de sistema de arquivos, autenticação. Mas não pergunta: "e se alguém escrever algo no input que faça o LLM gerar código malicioso?" Para ele, a IA é um componente confiável. A ideia de que um texto pode redirecionar o comportamento de um componente de software é estranha ao paradigma clássico.

**O blind spot do pesquisador de IA:** ele entende que modelos podem ser enganados, conhece as técnicas de ataque, sabe que guardrails são frágeis. Mas não pensa em containerização, data permissioning, isolamento de processos. Consegue dizer "esse sistema é vulnerável a prompt injection" mas não resolve o problema de implantação.

**Onde as carreiras se cruzam:** o exemplo concreto — LLM que gera e executa código. Solução: containerizar a execução em ambiente isolado. O código gerado pelo LLM roda numa sandbox, não no servidor principal. Agora o pior caso de um prompt injection é código malicioso que roda em container descartável — não no servidor de produção. Isso é classical security + AI awareness.

**O futuro do trabalho de segurança:** profissionais no cruzamento dos dois campos são escassos e altamente demandados. O trabalho não é "AI red teaming puro" (qual empresa compraria?) nem "cybersec clássico" (sem AI awareness). É o novo CSO que pensa em threat modeling para sistemas agenticos.

**Implicação para builders de produto:** ao contratar segurança para um produto com agentes, não contrate só um ou outro. O profissional ideal entende tanto os vetores de ataque específicos de LLMs quanto os princípios de permissioning e containerização.

## Como aplicar
1. **Ao revisar segurança de sistema agentico:** faça as duas perguntas — (a) "qual é a pior ação que o agente comprometido poderia tomar?" (AI lens) e (b) "quais permissões mínimas esse agente precisa?" (classical security lens).
2. **Dockerize qualquer execução de código gerado por LLM:** se seu sistema faz o LLM escrever e executar código, isso é requisito não-negociável. Qualquer output de código deve rodar em sandbox isolada.
3. **Para contratar:** busque alguém que entenda tanto de adversarial robustness quanto de permissioning de dados e arquiteturas de serviços. Se não existe, contrate um de cada e force colaboração estreita.
4. **Threat modeling de IA:** adicione ao seu processo de threat modeling a pergunta "qual seria o pior comportamento possível se esse componente for comprometido por prompt injection?" — para cada componente que usa LLM.
5. **Monitore tudo:** logging de inputs e outputs de todos os componentes de LLM é infraestrutura mínima. Não é defesa em tempo real — é a única forma de detectar ataques pós-facto e melhorar o sistema.

## Insights por autor
### [[Sander Schulhoff]]
- "Os trabalhos de segurança do futuro estão na intersecção. Não é só fazer AI red teaming, e não é só cybersegurança clássica. É onde os dois se encontram que o trabalho importante acontece."
- "Um profissional de segurança clássico olha para o sistema e não pensa 'e se alguém enganar a IA?' Isso simplesmente não é como esperamos que IA funcione, mesmo de uma perspectiva de ficção científica."
- "Um pesquisador de IA pode dizer que seu sistema é vulnerável, mas é o profissional de cyberseg que vai dockerizar o código e garantir que o pior caso é um container descartável, não seu servidor de produção."
- "Pesquisadores de IA são os únicos que conseguem resolver isso no longo prazo, mas profissionais de cybersegurança clássica são os únicos que conseguem mitigar no curto prazo — garantindo que implantamos sistemas com permissões adequadas e sem a possibilidade de coisas muito ruins."

> 🎧 [Why securing AI is harder than anyone expected and guardrails are failing | HackAPrompt CEO (1:32:41)](https://www.youtube.com/watch?v=J9982NLmTXg) · 2025-12-21

## Conceitos relacionados
[[Segurança Agentica — Não Dá para Patchar um Cérebro]] · [[CAMEL — Defesa por Permissão de Intenção]] · [[Falsa Confiança de Guardrail — Proteção Ilusória que Amplifica o Risco]] · [[Mastery Técnica antes da Gestão]]
