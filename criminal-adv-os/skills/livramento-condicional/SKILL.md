---
name: livramento-condicional
description: "Calcula o livramento condicional pelos requisitos do CP arts. 83-90 (fracoes 1/3, 1/2 e 2/3; reparacao do dano; requisitos subjetivos) + procedimento da LEP arts. 131-146 (condicoes, revogacao, prorrogacao). Use quando o operador disser livramento condicional, quando sai em livramento, requisitos do livramento, ou pedir para calcular se o apenado pode ser liberado condicionalmente."
---

# LIVRAMENTO-CONDICIONAL

> Camada 4 (execucao penal — LEP). Liberdade antecipada sob condicoes apos cumprir fracao da pena. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep** arts. 83 (requisitos), 84 (soma), 85-90 (condicoes/revogacao/extincao).
- `context/lep-7210-84.md` — arts. 66 (competencia), 131-146 (procedimento, condicoes, revogacao, prorrogacao).
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Dizer se o livramento cabe, com a **fracao aplicavel + data**, as condicoes impostas e o parecer — fundamentado artigo a artigo, com a lei seca aberta.

## Quando ativar
- Saber se/quando o apenado tem direito a livramento condicional.
- Calcular a fracao e a data do livramento.
- Conferir requisitos subjetivos, reparacao do dano ou risco de revogacao.

## Metodologia
1. **Cabimento (CP art. 83, caput).** Pena privativa de liberdade **igual ou superior a 2 anos**. Somam-se penas de infracoes diversas (art. 84).
2. **Fracao OBJETIVA (CP art. 83, I, II e V — ler no arquivo):**
   - **+1/3** (mais de um terco) se **primario** e **bons antecedentes** (I).
   - **+1/2** (mais da metade) se **reincidente em crime doloso** (II).
   - **+2/3** (mais de dois tercos) nos **hediondos/equiparados, tortura, trafico, trafico de pessoas e terrorismo**, **vedado ao reincidente especifico** nessa natureza (V).
   - ⚠️ Alem das fracoes, ha **vedacao expressa de livramento** em hipoteses do art. 112 LEP (VI-a, VI-b, VI-d e VIII) — conferir antes de afirmar cabimento.
3. **Requisitos SUBJETIVOS (CP art. 83, III — red. Lei 13.964/2019):** comprovar bom comportamento na execucao, **nao cometimento de falta grave nos ultimos 12 meses**, bom desempenho no trabalho e aptidao para prover a propria subsistencia. Crime doloso com violencia/grave ameaca: tambem condicoes pessoais que facam presumir nao reincidencia (par. unico).
4. **Reparacao do dano (CP art. 83, IV).** Ter reparado o dano, salvo efetiva impossibilidade.
5. **Procedimento (LEP arts. 131-146).** Concedido pelo **Juiz da Execucao**, presentes os requisitos do CP 83, ouvidos MP e Conselho Penitenciario (131). O juiz especifica as **condicoes** (132). Cerimonia de concessao (137). **Revogacao** obrigatoria (CP 86; LEP 140) por nova condenacao a PPL; **facultativa** (CP 87) por descumprimento de condicao ou condenacao a pena nao privativa. Revogado, em regra **nao se desconta** o tempo solto e nao pode ser novamente concedido (CP 88), salvo crime anterior.
6. **Extincao (CP 89-90; LEP 145-146).** Nao revogado ate o termo, a pena privativa de liberdade considera-se **extinta** (CP 90). O juiz nao declara extinta enquanto pender processo por crime cometido na vigencia (CP 89) — pode haver **prorrogacao**.
7. **Calcular:** pena total (apos detracao/remicao) x fracao -> tempo exigido -> data do livramento, a partir da data-base.

## Saida obrigatoria (calculo + data + parecer)
**Cabe? + fracao aplicavel (citando o inciso do CP 83) + data** + condicoes (LEP 132) + alerta de vedacao do art. 112 LEP se aplicavel + parecer + handoff. Passa pela `suprema-corte-criminal`.

## Guard
Nenhuma fracao/data sai sem `validador-criminal` (cruza `context/`). Conferir a fracao no CP 83 e a eventual vedacao de livramento no art. 112 LEP (redacao vigente NAO-tachada — 15.358/2026), nunca de memoria. Reincidente especifico em hediondo NAO tem o +2/3. Jurisprudencia so se ✅. Na duvida, bloquear e reler a lei seca. Gate final `suprema-corte-criminal`.

livramento-condicional -> arts. citados: CP 83 (I=+1/3 primario+bons antecedentes, II=+1/2 reincidente doloso, V=+2/3 hediondos/equiparados vedado reincidente especifico, III subjetivos, IV reparacao, par. unico), 84, 85, 86, 87, 88, 89, 90; LEP 66, 131, 132, 140, 145, 146 — vedacao de livramento conferida no art. 112 LEP vigente (VI-a, VI-b orcrim ultraviolenta, VI-d feminicidio, VIII reincidente+hediondo+morte).
