---
name: recursos-excepcionais-criminais
description: "Recurso Especial (REsp) ao STJ e Recurso Extraordinario (RE) ao STF na materia criminal, na perspectiva da defesa. Use para recurso especial, REsp, recurso extraordinario, RE, prequestionamento, repercussao geral, recurso aos tribunais superiores, agravo em REsp ou em RE, e juizo de admissibilidade de recurso excepcional."
---

# RECURSOS-EXCEPCIONAIS-CRIMINAIS

> Camada 7 (recursos criminais). REsp ao STJ e RE ao STF: vias de estreito cabimento, so apos esgotada a instancia ordinaria. Foco: DEFESA. Errar admissibilidade = nao conhecimento.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — grep o artigo do procedimento recursal (ex.: art. 637 — RE sem efeito suspensivo).
- `context/jurisprudencia-criminal.md` — so itens ✅ (Sumulas de admissibilidade citadas abaixo estao 🟡 — remeter ao validador).
- `context/penal-especial.md` — reformas 2024-2026 e regime recursal vigente.

## Objetivo
Levar a tese de defesa ao STJ (lei federal) ou ao STF (questao constitucional) com admissibilidade blindada: cabimento, prequestionamento e nao reexame de prova checados ANTES de redigir, para o recurso ser conhecido e julgado no merito.

## Quando ativar
Acordao de tribunal (apelacao/RESE) que contraria lei federal ou diverge de outro tribunal -> REsp; ou ofende a CF -> RE. Tambem "prequestionar", "repercussao geral", "negaram seguimento ao REsp/RE".

## Metodologia
1. **Esgotamento da instancia.** REsp e RE so cabem contra acordao de ultima/unica instancia; checar transito da via ordinaria e se cabem embargos de declaracao antes.
2. **Identificar a via:**
   - **REsp ao STJ — CF art. 105, III:** "a" contrariar/negar vigencia a lei federal; "b" validar ato local contestado em face de lei federal; "c" interpretacao divergente de outro tribunal (comprovar com cotejo analitico).
   - **RE ao STF — CF art. 102, III:** "a" contrariar a CF; "b" declarar inconstitucional tratado/lei federal. Exige **REPERCUSSAO GERAL** (CF art. 102, § 3) — preliminar formal e fundamentada, sob pena de nao conhecimento.
3. **PREQUESTIONAMENTO (requisito-chave).** A materia tem de ter sido decidida no acordao recorrido. Sumulas **282 e 356 do STF** e **211 do STJ** (🟡 validador). Se o ponto nao foi enfrentado, opor embargos de declaracao para prequestionar ANTES do REsp/RE.
4. **Nao reexame de prova.** REsp/RE nao reabrem fatos. **Sumula 7 do STJ** e **Sumula 279 do STF** (🟡) vedam revolvimento factico. Enquadrar a tese como **questao de direito** (valoracao juridica, nao reavaliacao de prova).
5. **Prazo e forma.** Prazo de **15 dias** (contagem penal/recursal — confirmar na `prazos-processuais-penais`); RE **nao tem efeito suspensivo** (CPP art. 637). Interposicao + razoes ao tribunal superior, demonstrando cada requisito de admissibilidade.
6. **Negado seguimento -> agravo.** Inadmitido o REsp/RE pela presidencia do tribunal a quo, cabe **agravo** para destrancar (regime atual — CPC art. 1.042 subsidiario; Lei 8.038/1990 disciplina o rito; o antigo art. 28 da Lei 8.038 foi superado pelo CPC). ⚠️ **Confirmar regime e prazo no `validador-criminal`** — nao afirmar dispositivo revogado como vigente.
7. **Defesa:** pedido alinhado a reversao favoravel (absolvicao, desclassificacao, anulacao, refazimento da dosimetria); jamais agravar a situacao do reu.

## Entrega obrigatoria final
- Identificacao da via (REsp art. 105, III / RE art. 102, III) + checklist de admissibilidade (esgotamento · prequestionamento · nao reexame de prova · repercussao geral se RE · prazo) + peca de interposicao e razoes redigidas + alerta de cada requisito que precise de embargos previos.

## Guard
Toda Sumula/tese/numeracao passa por `validador-criminal` e fecha em `suprema-corte-criminal` (R1-R4). Dispositivos da CF (105, III; 102, III e § 3) sao constitucionais — citar como CF, sem inventar. Regime do agravo (1.042 CPC / Lei 8.038) e teor das Sumulas 282/356/211/7/279: validador antes de afirmar. Na duvida de admissibilidade, bloquear.

recursos-excepcionais-criminais -> CF art. 105, III ("a"/"b"/"c"); CF art. 102, III e § 3 (repercussao geral); CPP art. 637 (RE sem efeito suspensivo); CPC art. 1.042 (agravo, subsidiario — remeter ao validador); Lei 8.038/1990 (rito — remeter ao validador); Sumulas STF 282, 356, 279 e STJ 211, 7 (🟡 validador).
