---
name: incidentes-execucao-penal
description: "Classifica e defende incidentes da execucao penal (LEP) — faltas disciplinares (49-52), regressao de regime (118), efeitos da falta grave sobre progressao/livramento, conversoes de pena (180-184) e unificacao. Use quando o operador disser falta grave, PAD, processo administrativo disciplinar, regressao de regime, incidente de execucao, perdeu a progressao, converteu a pena, ou apurar consequencia de falta no curso da pena."
---

# INCIDENTES DE EXECUCAO PENAL — Falta grave, regressao e conversoes

> Camada 4 (execucao penal — LEP). Skill de classificacao e defesa: enquadra o incidente, mede a consequencia temporal e arma a tese defensiva. O `criminal-master` acopla a peca (defesa no incidente / agravo em execucao) e o gate `suprema-corte-criminal`.

## Anexos obrigatorios (context/)
- `context/lep-7210-84.md` — buscar `Art. 49` a `Art. 52` (faltas), `Art. 118` (regressao), `Art. 57` (sancoes), `Art. 180` a `Art. 184` (conversoes) e `Art. 112` (progressao); ler so a faixa, **a redacao NAO-tachada**.
- `context/jurisprudencia-criminal.md` — so itens marcados ✅; Sumulas 533/534/535 do STJ sao 🟡, remeter a validacao antes de citar.

## Objetivo
Classificar o incidente (qual falta, hipotese de regressao ou conversao), apontar a consequencia temporal sobre os beneficios e devolver a defesa cabivel artigo a artigo — sem afirmar efeito de sumula nao confirmada.

## Quando ativar
- Apuracao ou defesa de falta grave / PAD na execucao.
- Risco ou decreto de regressao de regime.
- Impacto da falta grave sobre data-base de progressao, livramento ou comutacao.
- Conversao de pena (PPL em PRD ou PRD em PPL) ou unificacao.

## Metodologia
1. **Abrir a lei seca** e identificar o fato com a `memoria-de-caso-criminal` (regime, comportamento, fato imputado).
2. **Faltas — arts. 49-52:** classificam-se em **leves, medias e graves** (art. 49 — leves/medias e sancao a cargo da legislacao local). Faltas **GRAVES** do condenado a PPL no **art. 50** (I a IX — ex.: fuga, posse de celular no VII, recusa a identificacao genetica no VIII, aproximacao da vitima sob medida protetiva no IX, Lei 15.410/2026); para PRD, no **art. 51**. **Art. 52:** crime doloso e falta grave e, com subversao da ordem, sujeita ao RDD (Lei 13.964/2019). Sancoes observam o **art. 57**.
3. **Defesa tecnica no PAD:** apuracao de falta grave exige PAD com **defesa tecnica** — **Sumula 533 do STJ (🟡)**, so apos `validador-criminal` + `anti-alucinacao-juridica`. Frentes: nulidade do PAD sem defesa, falta de tipificacao no art. 50/51, atipicidade, ausencia de subversao da ordem (art. 52).
4. **Regressao — art. 118:** ocorre quando o condenado (I) pratica fato definido como crime doloso ou falta grave; (II) sofre condenacao por crime anterior cuja pena somada torne incabivel o regime (art. 111). No regime aberto, regride tambem por frustrar a execucao ou nao pagar a multa (§ 1). **Nas hipoteses do inciso I e do § 1 o condenado deve ser ouvido previamente** (art. 118 § 2) — contraditorio, com tese de nulidade se ausente.
5. **Efeitos temporais da falta grave:**
   - **Interrompe a data-base da progressao** (recomeca a contagem) — **Sumula 534 STJ (🟡)**.
   - **NAO interrompe** o prazo de livramento condicional nem de comutacao/indulto — **Sumula 535 STJ (🟡)**.
   - **Remicao:** pode revogar **ate 1/3** dos dias remidos (art. 127) — remeter a `remicao`.
   - ⚠️ Conferir teor/vigencia das Sumulas 533/534/535 no `validador-criminal` antes de afirmar o efeito; a fracao recalculada de progressao vem de `progressao-de-regime` (art. 112, redacao 2026).
6. **Conversoes — arts. 180-184:** PPL nao superior a 2 anos pode ser **convertida em restritiva de direitos** (art. 180 — regime aberto, 1/4 cumprido, antecedentes/personalidade favoraveis); a **PRD converte-se em PPL** nas hipoteses do art. 181 (falta grave, nao comparecimento, recusa injustificada). ⚠️ Art. 182 (multa em detencao) esta **revogado** (Lei 9.268/1996) — nao citar. Art. 183: medida de seguranca por doenca mental superveniente.
7. **Unificacao:** havendo mais de um titulo, unificar penas e recalcular saldo e marcos dos beneficios (cruza `motor-calculo-de-pena` e `progressao-de-regime`).
8. Em divergencia entre memoria e texto, vence o texto do arquivo.

## Saida obrigatoria
- **Classificacao do incidente:** qual falta (art. 50/51/52), qual hipotese de regressao (art. 118) ou de conversao (180-184), com o dispositivo.
- **Consequencia temporal:** o que interrompe (progressao — Sum. 534) e o que NAO interrompe (livramento/comutacao — Sum. 535), efeito na remicao (ate 1/3), nova data-base — tudo condicionado a validacao das sumulas.
- **Defesa cabivel:** nulidade do PAD sem defesa tecnica (Sum. 533, se validada), ausencia de contraditorio na regressao (art. 118 § 2), atipicidade, descabimento da conversao.
- **Parecer** com fundamento artigo a artigo + ressalva sobre sumulas 🟡 pendentes de validacao + proximo passo (defesa no incidente / agravo em execucao).

## Guard
Nenhum dispositivo, sumula ou efeito temporal entra sem `validador-criminal` (cruza `context/`). Sumulas 533/534/535 do STJ e SV 9 sao 🟡: bloquear ate confirmar teor/vigencia via `validador-criminal` + `anti-alucinacao-juridica` — nao afirmar efeito de memoria. Art. 182 (conversao de multa) esta revogado — nao citar. Percentual de progressao vem de `progressao-de-regime`. Toda entrega fecha pela `suprema-corte-criminal`.
