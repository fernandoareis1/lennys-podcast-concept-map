# ROUTINE — instruções para processar um lote de episódios (modelo de 5 camadas)

Você é um agente autônomo. Objetivo: **expandir o mapa de conceitos** do Lenny's Podcast no vault Obsidian, no **modelo de profundidade progressiva (5 camadas)**, processando um lote de episódios e fazendo commit **após cada convidado**.

## Parâmetros
- **TAMANHO DO LOTE:** até 20 convidados por execução.
- **Transcrições-fonte:** `lennys-podcast-transcripts-main/lennys-podcast-transcripts-main/episodes/{slug}/transcript.md`
- **Vault:** `obsidian-vault/`
- **Manifesto de progresso:** `obsidian-vault/_meta/processed.txt` (um slug por linha = já processado)

## Modelo de 5 camadas (densidade cresce ao descer)
| Camada | Pasta | `nivel` | Densidade-alvo | Papel |
|---|---|---|---|---|
| L1 · Fluxo | `Fluxos/` | 1 | ~100 palavras | hub da fase; lista os Temas |
| L2 · Tema | `Temas/` | 2 | ~130 palavras | agrupa conceitos afins do fluxo |
| L3 · Conceito | `Conceitos/` | 3 | ~300 palavras | card: ideia central + como aplicar |
| L4 · Aprofundamento | `Aprofundamento/` | 4 | 600+ palavras | citações longas, debate, casos, playbook |

**Regra de ouro:** todo conceito (L3) pertence a um **Tema (L2)**, e todo Tema pertence a um **Fluxo (L1)**. Conteúdo denso (citações longas/casos) vai para **L4**, nunca incha o L3.

## Taxonomia de Temas (L2) por fluxo
Use esta tabela para arquivar cada conceito sob o Tema certo. **Se a nota do Tema ainda não existir em `Temas/`, crie-a** (schema abaixo). Pode criar um Tema novo se nenhum servir, mas prefira reusar.

- **01 Discovery & Pesquisa** → `Discovery — Jobs to be Done (teoria da demanda)` · `Discovery — Entrevistar usuários` · `Discovery — Descoberta contínua & validação`
- **02 Estratégia & Visão** → `Estratégia — Posicionamento & diferenciação` · `Estratégia — Estratégia de produto` · `Estratégia — Visão, missão & narrativa`
- **03 Priorização & Roadmap** → `Priorização — Outcomes & metas` · `Priorização — Priorização & foco` · `Priorização — Estratégia vs execução`
- **04 Design & UX** → `Design — Cultura & papel do design` · `Design — Experiência & fricção`
- **05 Experimentação & Dados** → `Experimentação — A/B testing & cultura` · `Experimentação — Aprender com pouco/qualitativo`
- **06 Growth & Aquisição** → `Growth — Modelos de crescimento` · `Growth — Distribuição & canais` · `Growth — Anti-táticas`
- **07 Ativação & Retenção** → `Retenção — Ativação & onboarding` · `Retenção — Retenção & churn`
- **08 Monetização & Pricing** → `Monetização — Estratégia de monetização` · `Monetização — Modelos & poder de pricing`
- **09 Liderança & Times** → `Liderança — Modelos de time` · `Liderança — Liderança & founder` · `Liderança — Colaboração & comunicação`
- **10 Founder & Carreira** → `Founder — Mentalidade de founder` · `Founder — Carreira & progresso`

## Passos (processe UM convidado de cada vez)
1. Liste `episodes/` e leia `_meta/processed.txt`. Selecione os próximos slugs em ordem alfabética **não presentes** no manifesto (até 20). **Crie uma branch de trabalho** e NÃO trabalhe na `main`: `git checkout -b routine/lote-$(date +%Y%m%d-%H%M)`.
2. Para CADA convidado:
   a. Leia o `transcript.md`. **Confirme o convidado pelo CORPO do texto** (alguns frontmatters estão trocados).
   b. Extraia 3–6 **frameworks/mindsets/insights**.
   c. **L3 — Conceito:** crie/atualize a nota em `Conceitos/` (schema abaixo, `nivel: 3`). **Se o conceito já existir, NÃO sobrescreva** — adicione `### [[Autor]]` em "Insights por autor" e inclua o autor no frontmatter `autores`.
   d. **L2 — Tema:** garanta que o conceito referencia seu Tema (`**Tema:** [[...]]`) e que o Tema lista o conceito. Crie a nota do Tema se faltar.
   e. **L1 — Fluxo:** garanta que o Tema está listado no hub do fluxo em `Fluxos/`.
   f. **L4 — Aprofundamento (regra ≥3 autores):** quando um conceito acumular **3 ou mais autores**, crie (ou expanda) a nota `Aprofundamento/{Conceito} — Evidências.md` (`nivel: 4`) com as citações longas + timestamps de cada autor, e ligue-a no card L3 (seção "## Aprofundamento ⬇"). Para frameworks centrais muito ricos, pode criar também `— Debate` e `— Casos`.
   g. **Autor:** crie/atualize a nota leve em `Autores/`.
   h. Anexe o slug a `_meta/processed.txt`.
   i. Valide que os `[[links]]` criados têm arquivo correspondente em `Conceitos`/`Fluxos`/`Autores`/`Temas`/`Aprofundamento`/raiz (corrija órfãos).
   j. **COMMIT + PUSH NA BRANCH (NÃO na main):** `git add -A && git commit -m "routine: +1 (slug)"` e `git push -u origin HEAD`. NÃO tente **assinar** o commit — se um hook reclamar de assinatura, ignore (o commit já foi feito); nunca use `--amend` para isso.
3. Repita até 20 ou até a sessão estar acabando.
   ⚠️ **NUNCA acumule.** Cada convidado é commitado/pushed na branch ANTES do próximo, para sobreviver a qualquer interrupção.

## Publicação via Pull Request (NUNCA push na main)
- Na **primeira** publicação da branch, abra um PR para a `main`:
  `gh pr create --base main --head "$(git branch --show-current)" --title "routine: lote de convidados" --body "Processados: <slugs>"`
- Nos pushes seguintes o PR **atualiza sozinho** — não abra outro.
- **NUNCA** faça `git push origin main` nem `git merge` na main. O merge é feito pelo dono do repo após revisar o PR.
- Se o `git push` falhar com **403/permissão**, PARE e reporte (é credencial do ambiente; repetir não resolve).

## Schemas

### L2 — Tema
```markdown
---
tipo: tema
nivel: 2
fluxo: <Nome do Fluxo>
---
# 🧩 Tema · <Nome>
**Fluxo:** [[NN - Nome do Fluxo]] · **Camada:** L2 (Tema)

<2–3 linhas conectando os conceitos do tema.>

## Conceitos (L3)
- [[Conceito A]] — <gancho>
- [[Conceito B]] — <gancho>

## Descer mais (L4) ⬇
[[Conceito A — Evidências]]   (quando existir)
```

### L3 — Conceito
```markdown
---
tipo: framework | mindset | tecnica | insight
nivel: 3
fluxo: <Nome do Fluxo>
autores: [Nome]
---
# <Nome do Conceito>
**Fluxo:** [[NN - Nome do Fluxo]] · **Tema:** [[<Tema>]] · **Camada:** L3
**Tipo:** ... · **Fontes:** [[Autor]]

## Ideia central
2–4 linhas.

## Como aplicar
passos práticos.

## Insights por autor
### [[Autor]]
- ponto + citação curta
> 🎧 [Título (duração)](youtube_url)

## Aprofundamento ⬇   (só se houver L4)
- [[<Conceito> — Evidências]]

## Conceitos relacionados
[[...]] · [[...]]
```

### L4 — Aprofundamento
```markdown
---
tipo: aprofundamento
nivel: 4
fluxo: <Nome do Fluxo>
conceito_pai: <Conceito>
autores: [Nome, ...]
---
# 📜 <Conceito> — Evidências
**↑ Card:** [[<Conceito>]] · **Tema:** [[<Tema>]] · **Camada:** L4
**Fontes:** [[Autor]] (duração)

> citações LONGAS com timestamps, mecânica completa, casos. 600+ palavras.
```

## Os 10 fluxos (taxonomia fixa de topo)
01 Discovery & Pesquisa · 02 Estratégia & Visão · 03 Priorização & Roadmap · 04 Design & UX · 05 Experimentação & Dados · 06 Growth & Aquisição · 07 Ativação & Retenção · 08 Monetização & Pricing · 09 Liderança & Times · 10 Founder & Carreira

## Princípios
- **Eixo = conceito, não autor.** O autor é fonte/citação.
- Tudo em **PT-BR**. Não invente citações; baseie-se na transcrição.
- **Mescle** conceitos repetidos (acumular autores) em vez de duplicar.
- Densidade cresce ao descer: L3 enxuto, L4 denso.
