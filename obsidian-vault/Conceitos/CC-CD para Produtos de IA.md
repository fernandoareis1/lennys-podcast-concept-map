---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores:
  - Aishwarya Naresh Reganti
  - Kiriti Badam
---
# CC/CD para Produtos de IA

Framework de ciclo de vida iterativo para produtos de IA, análogo ao CI/CD do desenvolvimento de software tradicional. Nome completo: **Calibração Contínua / Desenvolvimento Contínuo**.

Motivação: como o comportamento de sistemas de IA não pode ser previsto antes do deployment, a única forma de construir com segurança é criar um loop de aprendizado que cresce progressivamente em autonomia sem destruir a experiência do usuário.

## O ciclo

### Loop de Desenvolvimento Contínuo (construção)
1. **Definir escopo de capacidade** — o que o sistema vai fazer e não vai fazer
2. **Curar dados** — montar um dataset de inputs esperados e seus outputs ideais; este exercício força o time a alinhar como o produto deve se comportar (PMs e especialistas do domínio são essenciais aqui)
3. **Configurar a aplicação** — construir o sistema
4. **Definir métricas de avaliação** — não "fazer evals", mas escolher *dimensões* que importam (ex: taxa de routing correto, erros de ferramenta, verbosidade)
5. **Deploy**

### Loop de Calibração Contínua (aprendizado em produção)
1. **Analisar comportamento** — observar o que usuários reais fazem; muitos padrões não são antecipáveis antes do deploy
2. **Identificar padrões de erro** — agrupar falhas por tipo
3. **Aplicar correções** — corrigir problemas identificados (alguns erros pontuais não precisam de nova métrica; basta corrigir e seguir)
4. **Criar novas métricas de avaliação** — quando surgem padrões novos que as métricas existentes não detectam
5. **Atualizar o dataset** — alimentar o flywheel com o que foi aprendido

## Eixo de progressão: agência vs. controle
Cada iteração deve aumentar a agência do agente e reduzir o controle humano — mas apenas quando confiança for demonstrada.

Exemplo com agente de suporte ao cliente:
- **V1** (alta controle, baixa agência): agente classifica e roteia tickets para o departamento certo; humanos fazem tudo o mais. Aprende: qualidade dos dados de routing, estrutura de contexto necessária.
- **V2** (controle médio): agente sugere draft de resposta ao agente humano; humano decide o que usar. Aprende: quais partes do draft são aproveitadas, onde o sistema erra. Este log *é análise de erro grátis*.
- **V3** (baixa controle, alta agência): agente resolve ticket de ponta a ponta de forma autônoma.

## Diferença entre evals e monitoramento de produção
- **Evals** detectam erros que você já conhecia (dataset de problemas mapeados)
- **Monitoramento de produção** detecta padrões emergentes que você *não* antecipou

Ambos são necessários. Evals não são substitutos do monitoramento, e vice-versa. A falácia comum é escolher um dos dois como suficiente.

## Quando avançar para a próxima versão?
Não há regra rígida. O sinal principal: quando as calibrações diárias deixam de revelar novos padrões de comportamento — o sistema está estável o suficiente para receber mais agência.

Atenção: eventos externos (troca de modelo de base, mudança de comportamento de usuário, alterações no produto) podem "descalibrar" o sistema e exigir reiniciar o ciclo.

## Nota sobre o nome
CC/CD é uma referência intencional ao CI/CD de engenharia de software. Assim como CI/CD automatiza integração e deployment, CC/CD torna contínuos a avaliação de comportamento e o desenvolvimento do produto de IA.

### [[Aishwarya Naresh Reganti]]
"A ideia é a calibração de comportamento — e não perder a confiança do usuário enquanto faz essa calibração."

### [[Kiriti Badam]]
"Se você começa no lugar errado, vai ter muita dificuldade em corrigir as coisas de lá. Começar pequeno te força a pensar: qual é o problema que estou resolvendo?"
