---
name: guia-de-execucao-penal
description: "Porta da execucao penal — abre a fase de cumprimento da pena e estabelece a LINHA DO TEMPO (data-base + marcos) que progressao, livramento, remicao e detracao usam. Use quando o operador disser execucao penal, guia de recolhimento, PEC, data-base, atestado de pena, calculo da execucao, unificacao de penas, ou pedir para iniciar/organizar a execucao de um condenado."
---

# GUIA-DE-EXECUCAO-PENAL

> Camada 4 (execucao penal — LEP). Porta de entrada da execucao: monta a linha do tempo e roteia para os beneficios. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/lep-7210-84.md` — **grep o artigo** (66, 105-107, 111, 112) e ler a faixa. ⚠️ art. 112 tem redacao 2026 — ler a NAO-tachada.
- `context/cp-2848-40.md` — art. 42 (detracao), 33 (regimes).
- `context/cpp-3689-41.md` — art. 387 §2 (detracao na fixacao do regime inicial).
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Abrir e organizar a execucao penal: fixar a data-base, montar a guia/PEC e o atestado de pena a cumprir, e entregar a linha do tempo dos marcos (progressao, livramento, etc.) que as demais skills da Camada 4 vao calcular.

## Quando ativar
- Transito em julgado e inicio do cumprimento — expedir/conferir guia de recolhimento.
- Pedido de atestado de pena a cumprir ou de calculo da execucao.
- Unificacao/soma de penas (condenacoes em processos distintos ou nova condenacao no curso).
- Definir/conferir a data-base de um beneficio.

## Metodologia
1. **Competencia (LEP art. 66).** Tudo na execucao corre perante o **Juiz da Execucao**: soma/unificacao (III-a), progressao/regressao (III-b), **detracao e remicao (III-c)**, livramento (III-e), incidentes (III-f), saidas temporarias (IV). Confirmar o juizo antes de peticionar.
2. **Guia de recolhimento (LEP arts. 105-107).** Transitada a sentenca e preso o reu, o juiz ordena a **expedicao da guia** (105). A guia (106) contem nome, qualificacao, inteiro teor da denuncia + sentenca + certidao de transito, antecedentes e **a data de terminacao da pena** (106, V). Sem guia, ninguem cumpre pena (107). A guia se **retifica** sempre que mudar o inicio ou o tempo da pena (106, §2).
3. **Data-base.** Marco zero de cada beneficio. Em regra e a **data do inicio do cumprimento** (prisao/transito). ⚠️ **Falta grave interrompe** o prazo da progressao e reinicia a contagem sobre a **pena remanescente** (LEP art. 112, §6) — recalcular a data-base apos cada falta grave reconhecida.
4. **Unificacao de penas (LEP art. 111).** Havendo condenacao por mais de um crime, o regime sai da **soma ou unificacao** das penas, observadas **detracao** e remicao. Sobrevindo condenacao no curso da execucao, soma-se ao **restante** da que esta sendo cumprida (111, par. unico).
5. **Detracao na fundacao da linha do tempo.** Abater o tempo de prisao provisoria (CP 42; CPP 387 §2) antes de projetar marcos — rotear para `detracao`.
6. **Atestado de pena a cumprir.** Pena total -> detracao -> remicao -> saldo a cumprir -> projecao dos marcos. Entregar a **linha do tempo** com cada beneficio datado.
7. **Rotear** os marcos: fracao/regime -> `progressao-de-regime`; +1/3, +1/2 ou +2/3 -> `livramento-condicional`; trabalho/estudo -> `remicao`; abatimento de cautelar -> `detracao`.

## Saida obrigatoria (calculo + data + parecer)
Linha do tempo da execucao: **data-base** + pena total + detracao/remicao + saldo + **datas projetadas** de cada marco (progressao, livramento) + fundamento (LEP 66, 105-107, 111; CP 42; CPP 387 §2) + parecer do que pedir primeiro + handoff. Passa pela `suprema-corte-criminal`.

## Guard
Nenhuma data/marco sai sem `validador-criminal` (cruza `context/`). Conferir SEMPRE a redacao vigente do art. 112 no `lep-7210-84.md` (a NAO-tachada — Lei 15.402/2026 + 15.358/2026); nunca decorar percentual. Na duvida de competencia/data-base, bloquear e reler a lei seca. Gate final `suprema-corte-criminal`.

guia-de-execucao-penal -> arts. citados: LEP 66, 105, 106, 107, 111, 112 (caput base 1/6 + §6 falta grave); CP 42; CPP 387 §2 — e a fracao do art. 112 que LI como vigente: caput base 1/6 (Lei 15.402/2026) com excecoes graduadas I-VIII (25/30/20/30/70/75/80/85), VI-A revogado.
