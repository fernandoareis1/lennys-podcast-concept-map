---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores:
  - Aishwarya Naresh Reganti
  - Kiriti Badam
---
# Trade-off Agência-Controle em IA

Produtos de IA diferem do software tradicional em dois aspectos fundamentais que mudam como se constrói e testa um produto.

## Os dois diferenciais

### 1. Não-determinismo
Em software tradicional, o fluxo de decisão é mapeado: o usuário clica em botões, preenche formulários, e o sistema responde de forma previsível. Em produtos de IA, essa camada foi substituída por uma interface fluida — a linguagem natural.

Isso cria dupla incerteza:
- **Input**: o usuário pode expressar a mesma intenção de infinitas formas; não dá para prever como ele vai interagir
- **Output**: o LLM é uma API probabilística, sensível a frasings de prompt e essencialmente uma caixa preta

Resultado: você não sabe como o usuário vai se comportar *nem* como o LLM vai responder. Você está tentando antecipar comportamento de uma entrada e saída que não entende completamente.

### 2. Trade-off Agência-Controle
Toda vez que você delega capacidade de decisão a um sistema agêntico, você abre mão de uma parcela de controle. A proporção não é grátis — ela precisa ser *conquistada* pelo agente ao longo do tempo.

O princípio: agentes precisam ganhar confiança antes de receber autonomia. Não comece colocando um agente para fazer ações de alto impacto desde o dia 1. Comece com alto controle humano e baixa agência do agente; aumente progressivamente à medida que o sistema demonstra comportamento confiável.

## Por que isso importa na prática

A maioria das falhas em produtos de IA acontece quando times:
1. Ignoram o não-determinismo — testam o sistema uma vez e assumem que sempre funcionará igual
2. Pulam para o "V3 autônomo" antes de construir confiança — e descobrem que não conseguem depurar um agente com múltiplas decisões interdependentes

A solução é o framework [[CC/CD para Produtos de IA]].

## Exemplos
- **Booking.com** (software tradicional): intenção → ação via fluxo determinístico de botões e formulários
- **Agente de suporte** (AI): mesma intenção pode gerar centenas de variações de input, e o LLM pode gerar outputs diferentes a cada vez
- **IA em pré-autorização médica (seguros)**: MRIs e exames de sangue = baixo risco, alta agência OK; cirurgias invasivas = alto risco, humano no loop obrigatório

## Aplicação direta
Antes de construir qualquer produto de IA, mapeie:
1. Quais partes do fluxo são não-determinísticas (input e output)
2. Qual o nível atual de confiança que o agente ganhou — e portanto, quanta agência ele pode receber
3. Onde humanos devem permanecer no loop

### [[Aishwarya Naresh Reganti]]
"Você não sabe como o usuário vai se comportar com seu produto, e você também não sabe como o LLM vai responder. Então você está trabalhando com input, output e processo — e não entende bem nenhum dos três."

### [[Kiriti Badam]]
"Você precisa deliberadamente começar em lugares onde há impacto mínimo e mais controle humano, para ter uma boa percepção das capacidades atuais. Depois, aos poucos, você inclina para mais agência."
