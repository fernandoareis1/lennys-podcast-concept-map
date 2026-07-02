---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Nikita Bier]
---
# Seed Controlado — Eliminar Variáveis Confusas no Teste

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Nikita Bier]]

## Ideia central
Em produtos com efeitos de rede, o principal obstáculo para testar se algo funciona é a **variável confusa da densidade**: se poucos usuários estão no app ao mesmo tempo, você não sabe se o produto falhou porque a ideia é ruim ou porque não havia críticos suficientes para o flywheel girar.

A solução de Nikita Bier: **seed controlado** — semente artificial de usuários em um espaço geográfico ou social fechado (ex: uma escola) para atingir densidade suficiente e observar se o produto funciona **como se já tivesse rede**. Isso é para **testar**, não para crescer.

Distinção crítica que a maioria confunde:
- **Seeding** = criar condições experimentais controladas para observar comportamento orgânico (para validação)
- **Growth** = como o produto cresce realmente depois de validado (deve ser orgânico)

Em tbh e Gas, Nikita semeava em escolas via follow em contas de Instagram (identificando alunos pelo bio) para testar. Depois que o produto provava que funcionava, o crescimento acontecia sozinho. **"Nunca fomos de escola em escola manualmente. Assim foi como testamos, não como crescemos."**

## Como aplicar
1. **Identifique o ambiente de teste mínimo**: qual é o espaço social fechado onde você pode criar densidade artificial? (escola, universidade, empresa, prédio residencial, comunidade online)
2. **Semeie manualmente os primeiros 100–500 usuários**: use qualquer método ético (follow, DM, flyer, presença física) para ter densidade naquele ambiente.
3. **Remova a variável confusa**: com densidade criada artificialmente, qualquer falha no produto é de produto — não de falta de usuários.
4. **Observe o orgânico antes de escalar**: se depois do seed o produto não cresce dentro daquele ambiente sem mais intervenção sua, a ideia provavelmente não funciona.
5. **Não confunda processo de teste com estratégia de crescimento**: nunca apresente o seeding como "nossa estratégia de go-to-market".

## Insights por autor
### [[Nikita Bier]]
- "This is not the way we grew the app. This is how we tested apps."
- "For the first 100 users, yes, that's how we got them. And that allowed us to know whether the product was working or not."
- "We wanted to eliminate all those potentially confounding variables so you can know immediately whether something's working or not."
- "You never want to walk away from an experiment and say, 'Well, maybe the execution was bad.' You really want to make sure your tests actually provide signal."
> 🎧 [Driving alignment within teams, work-life balance, and the changing PM landscape (59:20)](https://www.youtube.com/watch?v=4PhfAbRQpbI)

## Conceitos relacionados
[[Demanda Latente — Sinal de Produto no App Store]] · [[Adolescentes como Audiência de Crescimento Viral]] · [[Experimentos Wizard of Oz]] · [[Falha Conclusiva — Design de Experimento Definitivo]]
