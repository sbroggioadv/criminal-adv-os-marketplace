---
name: sursis-penal
description: "Pleiteia a suspensao condicional da PENA / sursis penal (CP arts. 77-82) — suspende a execucao da pena privativa ja aplicada (ate 2 anos, ou ate 4 no etario/humanitario), com periodo de prova e condicoes, ate a extincao da pena. Use quando o operador disser sursis, sursis penal, suspensao condicional da pena, suspender a pena, ou sursis etario/humanitario."
---

# SURSIS-PENAL

> Camada 5 (acordos & despenalizacao). Sursis PENAL — suspende a EXECUCAO da pena privativa de liberdade ja imposta na sentenca. Foco DEFESA. NAO confundir com sursis PROCESSUAL (Lei 9.099 art. 89 = `suspensao-condicional-processo`, que suspende o processo antes da condenacao).

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep** arts. 77 (caput, I-III, §§1-2), 78 (§§1-2), 79, 80, 81 (I-III, §§1-3), 82. O numero pode quebrar de linha — ler a faixa.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Verificar se a pena aplicada comporta sursis penal, obter a suspensao na modalidade mais favoravel (simples x especial; etario/humanitario quando cabivel) e conduzir ate a extincao da pena ao fim do periodo de prova sem revogacao — evitando o encarceramento.

## Quando ativar
- Sentenca com **pena privativa nao superior a 2 anos** (ou ate 4 no etario/humanitario) e substituicao por restritiva (art. 44) nao cabivel/indicada.
- "Suspende a pena?" / "sursis" / "cabe sursis pra esse reu?".
- Reu maior de 70 anos ou com razoes de saude (etario/humanitario); ou conferir/pleitear sursis em recurso.

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Requisitos (CP art. 77 caput, I-III):** pena privativa **nao superior a 2 anos**, suspensa por **2 a 4 anos**, desde que: **I** reu **nao reincidente em crime doloso** (§1: condenacao anterior so a multa NAO impede); **II** culpabilidade, antecedentes, conduta social, personalidade, motivos e circunstancias autorizem; **III** **nao seja cabivel/indicada a substituicao do art. 44** (restritivas de direitos). A substituicao do art. 44, quando cabivel, prefere o sursis.
2. **Etario e humanitario (art. 77 §2):** pena **nao superior a 4 anos** pode ser suspensa por **4 a 6 anos** quando o condenado for **maior de 70 anos** (etario) **ou razoes de saude** justifiquem (humanitario). Mesmo §2 cobre as duas hipoteses — conferir.
3. **Condicoes — SIMPLES x ESPECIAL (art. 78):** §1 (regra/**simples**) — no 1o ano, prestar servico a comunidade (art. 46) **ou** limitacao de fim de semana (art. 48). §2 (**especial**, mais brando) — se reparou o dano (salvo impossibilidade) **e** as circunstancias do art. 59 forem inteiramente favoraveis, o juiz pode substituir o §1 por: a) proibicao de frequentar lugares; b) proibicao de ausentar-se da comarca sem autorizacao; c) comparecimento pessoal mensal a juizo. **Defesa: pleitear a modalidade especial.** Art. 79: o juiz pode especificar outras condicoes adequadas. Art. 80: a suspensao **nao se estende as penas restritivas de direitos nem a multa**.
4. **Revogacao OBRIGATORIA (art. 81, I-III):** I condenacao irrecorrivel por **crime doloso**; II frustrar, embora solvente, a execucao da multa **ou** nao reparar o dano sem motivo justificado; III descumprir a condicao do §1 do art. 78.
5. **Revogacao FACULTATIVA (art. 81 §1):** descumprir qualquer outra condicao **ou** condenacao irrecorrivel por **crime culposo/contravencao** a pena privativa ou restritiva. **Prorrogacao:** §2 — se o beneficiario esta sendo processado por outro crime/contravencao, o prazo prorroga-se ate o julgamento definitivo; §3 — na revogacao facultativa o juiz pode, ao inves de revogar, prorrogar o periodo de prova ate o maximo.
6. **Extincao (art. 82):** expirado o prazo sem revogacao, considera-se **extinta a pena privativa de liberdade** — rotear `extincao-da-punibilidade` para registrar o efeito.

## Entrega obrigatoria final
Parecer de cabimento (pena + requisitos do art. 77) + modalidade pleiteada (simples/especial; etario/humanitario) + condicoes propostas + cronograma do periodo de prova + alerta sobre revogacao obrigatoria/facultativa + minuta do pedido/recurso + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo/prazo sai sem `validador-criminal` (cruza `context/`). Conferir limite de pena (2 anos / 4 no §2), periodo de prova e condicoes na lei seca, nunca de memoria. NAO confundir com sursis processual (Lei 9.099 art. 89 = `suspensao-condicional-processo`). Jurisprudencia so se ✅. Na duvida, bloquear e reler CP 77-82. Gate final `suprema-corte-criminal`.

sursis-penal -> arts. citados: CP 77 (caput; I-III; §§ 1, 2 etario/humanitario), 78 (§1 simples, §2 especial a/b/c), 79, 80, 81 (I-III; §§ 1 facultativa, 2 prorrogacao, 3), 82; CP 44 (substituicao), 46, 48, 59. Cross-link: suspensao-condicional-processo (Lei 9.099 art. 89 — NAO confundir).
