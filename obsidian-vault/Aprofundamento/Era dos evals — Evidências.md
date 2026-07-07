---
tipo: aprofundamento
nivel: 4
fluxo: Estratégia & Visão
conceito_pai: Era dos evals — o eval é o PRD do modelo
autores: [Brendan Foody, Hamel Husain, Shreya Shankar, Karina Nguyen, Kevin Weil, Nick Turley]
---
# 📜 Era dos evals — Evidências
**↑ Card:** [[Era dos evals — o eval é o PRD do modelo]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L4
**Fontes:** [[Brendan Foody]] (1:07:08) · [[Hamel Husain]] (1:46:33) · [[Shreya Shankar]] (1:46:33) · [[Karina Nguyen]] (1:14:34) · [[Kevin Weil]] · [[Nick Turley]] (01:14:00)

---

## [[Brendan Foody]] — A camada de negócio dos evals (2025-09-18)

> "Se o modelo é o produto, o eval é o PRD — mas também é o material de vendas. Os labs usam evals para demonstrar as capacidades dos seus modelos."

> "O gargalo primário dos labs para melhorar modelos é como eles podem medir efetivamente o que parece sucesso para o modelo. Toda capacidade que você quer que o modelo execute precisa de um eval primeiro."

> "A barreira para aplicar agentes em toda a economia para automatizar qualquer workflow é: como medimos sucesso? Como fazemos o eval?"

> "Os modelos são apenas tão bons quanto seus evals. Toda a economia vai provavelmente se tornar uma máquina de ambiente de evals, construindo mundos e contextos para que haja rubrics ou verificadores."

**Mecanismo:** Evals funcionam como "rubricas" que permitem ao modelo ser avaliado de forma objetiva — análogo a uma prova com gabarito. Sem eval, não há como recompensar os comportamentos certos no RL, nem validar que uma capacidade foi adquirida. Isso torna evals o ativo estratégico central de qualquer lab ou empresa construindo em cima de IA.

**Mercado:** Há uma nova categoria de trabalho humano especializado em escrever evals — mais bem-paga que crowdsourcing tradicional porque requer expertise real. Top 10% dos contribuidores geram maioria do impacto de melhoria de modelos.

🎧 [Why experts writing AI evals is creating the fastest-growing companies in history | Brendan Foody (1:07:08)](https://www.youtube.com/watch?v=ja6fWTDPQl4) · 2025-09-18

---

## [[Hamel Husain]] & [[Shreya Shankar]] — A metodologia prática de evals para builders (2025-09-25)

> "Evals é uma forma de medir e melhorar sistematicamente uma aplicação de IA. No fundo é análise de dados do seu aplicativo de LLM — data analytics — com uma forma sistemática de olhar esses dados, criar métricas e iterar com confiança." — Hamel

> "Evals é um grande espectro de formas de medir a qualidade da aplicação. Unit tests são só uma pequena parte desse grande quebra-cabeça." — Shreya

**O processo completo (demonstrado ao vivo com caso real da Nurture Boss):**

### Fase 1 — Error Analysis / Open Coding
Amostrar ~100 traces (logs de interação), anotar o primeiro erro visível em cada um de forma livre e descritiva. Não tentar categorizar ainda — apenas capturar. O objetivo é desenvolvimento de intuição sobre o que está errado.

> "Quando as pessoas fazem esse processo de olhar os dados, ficam imediatamente viciadas. Você aprende muito sobre sua aplicação em muito pouco tempo." — Hamel

> "Não há nenhum LLM que consiga fazer essa parte da análise pelo humano. Eu apostaria dinheiro nisso. Se você colocar uma alucinação sobre tour virtual no ChatGPT e perguntar 'tem algum erro?', ele vai dizer 'não, fez ótimo trabalho'. Mas Hamel tinha o contexto de que a empresa não oferece tour virtual." — Shreya

**Conceito do "benevolent dictator":** Não use um comitê para decidir o que é erro. Designe uma pessoa com expertise de domínio como a "ditadora benevolente" — ela define o que é certo e errado. Processo por comitê torna o eval caro demais para manter.

### Fase 2 — Axial Coding (LLM para organizar)
Exportar as notas como CSV e pedir a um LLM para agrupar em categorias de falha (axial codes). Revisar as categorias e torná-las específicas e acionáveis (não genéricas como "capability limitations").

> "O que as pessoas geralmente fazem é pular direto para os testes. Isso é onde as coisas saem dos trilhos. Você precisa primeiro fazer análise de dados para saber o que realmente merece um eval." — Hamel

> "Os termos open coding e axial coding vêm das ciências sociais — não é algo que inventamos. Se alguém te traz uma forma de fazer algo inteiramente nova sem embasamento em centenas de anos de teoria, você devia ser um pouco cético." — Shreya

### Fase 3 — Contagem (pivot table)
Usar a planilha para contar frequência de cada categoria de falha. A técnica de contagem simples é subestimada — é poderosa porque vai do caos a prioridades claras em minutos.

> "Basic counting is the most powerful analytical technique in data science because it's so simple and it's undervalued." — Hamel

### Fase 4 — LLM como Juiz (para falhas subjetivas)
Para modos de falha que não são capturáveis com código simples (ex.: "deveria ter transferido para um humano?"), criar um LLM judge com output binário true/false. Validar o juiz contra as anotações humanas via **matriz de confusão** — não apenas % de concordância.

> "Você não quer escrever um eval com escala de 1 a 5. Isso é uma forma covarde de não tomar uma decisão. Você precisa decidir: isso é bom o suficiente ou não? Quando você reporta as métricas, ninguém sabe o que 3.2 versus 3.7 significa." — Hamel

> "Quando as pessoas perdem confiança nos seus evals, perdem confiança em você. É crítico que você valide seu juiz." — Hamel

**Erros comuns identificados:**
- Criar o prompt de juiz e confiar nele sem validar contra humano.
- Usar apenas % de concordância (enganoso quando erros são raros).
- Escala Likert ao invés de binário.
- Pular a análise de erros e ir direto para os testes.

**Sobre o debate "evals vs. vibe checks":**
> "Dogfooding é perigoso só porque muitas pessoas dizem que estão dogfooding mas não estão de verdade — não estão com aquela viscosidade necessária para fechar o loop de feedback." — Hamel

> "Coding agents como Claude Code estão de pé nos ombros dos evals que os colegas fizeram para os modelos de coding. Não existe mundo em que eles estão sendo como, 'fiz o Claude Code, nunca vou olhar nada'." — Shreya

**Sobre o debate "evals vs. A/B tests":**
> "A/B tests são mais uma forma de eval — você tem uma métrica que quantifica sucesso de algo e está comparando. Não dá para fazer A/B test sem um eval para comparar. Talvez só tenhamos um jeito diferente de ver isso." — Shreya

**Tempo investido:**
- Setup inicial: 3–4 dias para rodar o processo completo e criar os primeiros LLM judges.
- Manutenção: ~30 minutos por semana depois do setup.
- Quantidade de LLM judges necessários: 4 a 7 por produto típico.

🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

---

---

## [[Karina Nguyen]] — Evals de dentro do lab: treinar comportamentos de produto (2025-02-09)

> "O eval mais robusto é o que faz o baseline promtado receber a pontuação mais baixa. Porque então você sabe que, se treinou um bom modelo, ele vai subir nesse eval continuamente sem regredir em outros evals de inteligência."

> "Às vezes peço aos product managers para criar uma planilha dupla com diferentes abas: qual é o comportamento atual, qual é o comportamento ideal e por quê, e algumas notas. Às vezes usamos com evals, às vezes usamos para treinamento. Porque se você der a planilha ao modelo o1, ele provavelmente vai descobrir como ensinar a si mesmo um bom comportamento."

**A perspectiva do modelo para treinar produtos:**

Enquanto Hamel/Shreya ensinam evals para melhorar *aplicações de LLM já deployadas*, Karina ensina evals para *treinar comportamentos novos no modelo*. A diferença é de nível: produto vs. fundação. Na prática de Karina:

1. **Evals determinísticos** (pass/fail): para comportamentos de decisão clara. Exemplo de Tasks: "Se o usuário diz 7PM, o modelo deve dizer 7PM." Binário, auditável, mensurável.

2. **Win-rate humano**: para qualidade de output subjetiva. Dada uma conversa e dois completions, qual modelo produziu melhor resultado? Percentual de vitória sobre o modelo anterior = sinal de progresso.

3. **Evals como especificação de treinamento**: a planilha com "comportamento atual / ideal / por quê" é passada ao o1, que usa para inferir como sintetizar dados de treinamento.

**Ensinar PMs e model designers a escrever evals:**

> "Uma parte do meu tempo na OpenAI foi trabalho de IC de pesquisa — rodar código, treinar modelos, escrever evals, trabalhar com PMs e designers para ensiná-los a pensar em avaliação. Acho que foi uma adoção de 'como fazemos product management de feature de IA para nossos modelos de IA'."

O processo criou uma nova função: *model designer* — alguém que pensa nos comportamentos do modelo como produto, escreve evals para esses comportamentos e define o que "correto" significa para cada interação.

**Prompting como nova prototipagem:**

> "Prompting é uma nova forma de desenvolvimento de produto ou prototipagem para designers e product managers."

O demo de 100K context com file uploads foi construído inteiramente como protótipo em browser local via prompting — sem treinamento. A capacidade existia; o form factor foi validado com prompts antes de qualquer investimento em engenharia.

🎧 [OpenAI researcher on why soft skills are the future of work](https://www.youtube.com/watch?v=DeskgjrLxxs) · 2025-02-09

---

## [[Kevin Weil]] — Evals como habilidade central do CPO (2025-04-10)

> "Escrever evals está se tornando uma habilidade central de PMs em empresas de IA, da mesma forma que análise de dados se tornou no ciclo anterior."

> "Entender se o modelo é 60% ou 99,5% confiável determina qual produto você pode construir. Evals são o gate de cada feature."

**Evals como gating de produto:**

Kevin Weil, como CPO da OpenAI, descreve o ciclo completo de como evals determinam o que é construível:

1. O PM escreve o eval que define o comportamento esperado para uma nova capacidade.
2. O time de treino usa esse eval como sinal de hill-climbing — o modelo melhora iterativamente nessa direção.
3. Quando o eval atinge o threshold de confiabilidade necessário, a feature pode ser lançada.
4. A distinção entre "o modelo *sabe* fazer" (demonstra em prompts específicos) e "o modelo faz *de forma confiável*" (passa no eval em escala) é capturada exclusivamente pelos evals.

**Caso concreto — Deep Research:**

> "Para Deep Research, usamos evals para definir o que é uma boa pesquisa. Depois usamos isso para hill-climbing durante o treinamento. O eval define a direção do treino."

Esse ciclo é análogo ao que Brendan Foody descreve para labs — evals como motor de RL — mas descrito da perspectiva do PM que precisa *especificar* o critério antes de qualquer treinamento acontecer.

**Por que evals são agora requisito de PM:**

> "Análise de dados se tornou uma habilidade esperada de PMs no ciclo anterior. Evals estão fazendo o mesmo no ciclo atual."

Kevin compara a evolução: antes, um PM sem SQL ou Amplitude era "cego". Hoje, um PM que não escreve evals para produtos de IA trabalha igualmente cego — sem capacidade de medir se o modelo evoluiu na direção correta.

🎧 [OpenAI's CPO on why ChatGPT is the worst AI you'll ever use | Kevin Weil](https://www.youtube.com/watch?v=scsW6_2SPC4) · 2025-04-10

---

## [[Nick Turley]] — O eval como instinto de PM formalizado (2025-08-09)

> "I started writing evals before I knew what an eval was — I was just outlining very clearly specified ideal behavior for various use cases until someone told me 'Hey, you should make an eval.'"

> "It's not some technical magic you have to understand. It's really just articulating success in a way that is maximally useful for training bots."

> "At the end of the day, it's not different from the wisdom of: you ought to articulate success before you do anything else. It's just a new mechanism for doing that."

**O eval como instinto de produto formalizado em linguagem de ML:**

Nick Turley, Head of Product do ChatGPT, traz talvez a perspectiva mais reveladora sobre evals: ele os descobriu por acidente enquanto fazia o que qualquer bom PM faz — definir claramente o que seria sucesso.

O que é notável no seu relato:
- Antes de saber o que era um "eval", ele já fazia o equivalente: documentava com precisão o comportamento ideal para cada use case do ChatGPT.
- Alguém do time de pesquisa reconheceu o padrão e disse: "isso que você está fazendo — é um eval."
- Isso revela que evals não são uma construção artificial de ML — são a formalização, em linguagem compatível com sistemas de treino, de algo que bons PMs já fazem intuitivamente.

**A desmistificação:**

> "It's not some technical magic you have to understand."

Essa frase é importante para adoção: um dos maiores obstáculos à escrita de evals é a percepção de que é uma tarefa técnica — de engenheiro ou pesquisador. Nick desconstruiu isso: é articular sucesso, que é fundamentalmente uma responsabilidade de produto.

**O loop que ele descobriu:**

Usou evals para definir o comportamento ideal do ChatGPT antes de qualquer treinamento; o processo o ensinou que "eval" era simplesmente a forma ML de especificar produto. Isso fechou o loop entre:

- PM define comportamento ideal (eval) →
- Treino usa eval para hill-climbing →
- Comportamento do modelo converge para o especificado →
- PM valida com o eval que o comportamento chegou ao target

O que é um loop de product development — apenas com o "código" substituído pelo "modelo".

🎧 [Inside ChatGPT: The fastest growing product in history | Nick Turley (OpenAI) (01:14:00–01:16:00)](https://www.youtube.com/watch?v=ixY2PvQJ0To) · 2025-08-09

---

## Síntese — Por que evals se tornaram a habilidade mais importante

Seis perspectivas convergentes revelando camadas complementares do mesmo fenômeno:

1. **Nível de modelo/lab** (Brendan Foody): evals são o gargalo para melhorar fundação de modelos; sem eval, não há RL, não há validação de capacidade. São também o "material de vendas" com que labs demonstram capacidades objetivamente.
2. **Nível de produto de IA** (Hamel + Shreya): evals são a forma sistemática de entender o que está errado com sua aplicação de LLM, priorizar melhorias e testar regressões. O processo correto: error analysis → axial coding → contagem → LLM judge.
3. **Nível de PRD** (Hamel + Shreya): "evals são os novos PRDs" — o prompt do LLM judge captura as expectativas do PM de forma explícita, verificável e que melhora iterativamente com os dados reais.
4. **Nível de treinamento de produto** (Karina Nguyen): evals definem o que "correto" significa para comportamentos específicos de produto, e essa definição alimenta diretamente a geração de dados sintéticos para pós-treinamento — fechando o loop entre produto e modelo.
5. **Nível de gating de features** (Kevin Weil): evals determinam o que é construível — a confiabilidade do modelo em cada tarefa só pode ser conhecida através de evals em escala. O PM sem evals trabalha cego, como o PM sem análise de dados na era anterior.
6. **Nível de instinto de PM** (Nick Turley): evals não são magia técnica — são a formalização do que bons PMs já fazem: articular sucesso de forma clara e mensurável. A única diferença é que a articulação deve ser compatível com sistemas de treino de ML.

**O que unifica todas as perspectivas:** em sistemas estocásticos (como LLMs), não há garantia de comportamento — só medição sistemática. Evals são a infraestrutura de qualidade do desenvolvimento de produtos de IA, análoga a testes unitários + analytics + QA no desenvolvimento de software tradicional — mas com técnicas adaptadas ao não-determinismo. Quem define o eval define o produto; quem não evaleia não sabe o que tem.
