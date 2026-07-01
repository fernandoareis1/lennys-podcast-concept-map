---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Nikita Bier]
---
# Processo Reprodutível de Testes — Muitas Apostas com Sinal Limpo
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fonte:** [[Nikita Bier]]

## Ideia central
O erro do fundador de consumer app não é escolher a ideia errada — é não ter um processo reprodutível para testar muitas ideias. A qualidade do processo reduz o risco mais do que qualquer insight de produto.

**A lição dos 15 apps:**
Nikita e sua equipe construíram 15 apps em 5 anos antes de tbh. O primeiro app mobile levou 1 ano para construir; o último levou 2 semanas. A velocidade de iteração não veio de preguiça ou de atalhos — veio de um processo cada vez mais afiado de: seed, observe, decide, next.

**Os dois erros de teste mais comuns:**
1. **Variáveis confusas:** você lança, não cresce, mas não sabe se foi a ideia, a execução, a audiência ou o produto. "Talvez as pessoas não tivessem amigos o suficiente." "Talvez não tivéssemos o aha moment certo." Não dá para aprender com isso.
2. **Testar a versão ruim:** você testa uma versão subótima e conclui que a ideia não funciona — mas na verdade a execução era ruim.

**A regra: elimine variáveis confusas**
- Sature a audiência-alvo com a presença do produto antes de lançar (follow Instagram accounts da escola-alvo, anúncios direcionados ao CEP)
- Garanta que usuários têm pessoas o suficiente na rede para experimentar valor
- Execute 100% na parte que você está testando; half-ass o resto
- Para consumer social: seed manual de uma escola inteira = sinal limpo de "o produto funciona com densidade adequada?"

**Validação em cascata:**
O processo de desenvolvimento 0-to-1 de Nikita segue afirmações condicionais:
1. As pessoas usarão o core flow? (testar apenas isso, perfeito)
2. Elas vão espalhar dentro do peer group? (só adicione spreading se 1 for verdade)
3. Vai cruzar peer groups? (só adicione hopping se 2 for verdade)
4. Pagarão? (só teste monetização se 3 for verdade)

Em cada estágio: 4 coisas que devem ser verdade. Quanto mais afirmações condicionais, mais alto o risco.

**Live chat como ferramenta de pesquisa:**
Adicione suporte via chat ao vivo 24h no app. Parece ineficiente, mas:
- Elimina a variável "o usuário saiu porque não recebeu suporte?"
- Usuários dizem exatamente qual problema têm (a melhor forma de user research)
- Feedback vai diretamente para o Slack do produto

## Como aplicar
1. **Construa a máquina de teste primeiro:** como você seed uma audiência-alvo de forma reprodutível?
2. **Liste suas variáveis confusas:** o que poderia explicar a não-adoção que NÃO é a ideia ruim?
3. **Elimine cada uma:** seed adequado, onboarding funcionando, rede suficiente
4. **Teste em sequência, não em paralelo:** valide core flow antes de adicionar spreading; spreading antes de hopping
5. **Execute 100% na coisa que você está validando agora;** tudo mais pode ser imperfeito
6. **Adicione chat ao vivo:** o custo marginal de ter feedback direto de usuário é baixo; o benefício de saber exatamente o que está quebrando é alto

## Insights por autor
### [[Nikita Bier]]
- "If you actually focus more on your process for taking many shots at bat, that's what actually reduces the risk more than anything."
- "We wanted to eliminate all those potentially confounding variables so you can know immediately whether something's working or not."
- "You never want to walk away from an experiment and say, 'Well, maybe the execution was bad.'"
- "Execute at 100% for the thing you're trying to validate at that specific stage. You can half-ass the rest."
- "If this is true, then what next needs to be true for this thing to work out? These layers of conditional statements — the more layers you have, the higher risk your product is."
- "Put live chat in your app 24 hours a day. Users will literally tell you the problem they're having."

## Conceitos relacionados
[[Demanda Latente — Cristalizar o que as Pessoas Já Querem]] · [[Experimentação com amostras pequenas]] · [[Taxa de Fracasso de 80% — A Realidade da Experimentação]] · [[A maioria das ideias falha no teste]] · [[Aha Moment Invertido — Valor Antes do Onboarding]]
