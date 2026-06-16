---
name: detracao
description: "Calcula a detracao penal — abate na pena (e na medida de seguranca) o tempo de prisao provisoria, prisao administrativa e internacao (CP art. 42) + impacto na unificacao (LEP art. 111) + na fixacao do regime inicial pelo juiz da condenacao (CPP art. 387 §2). Use quando o operador disser detracao, abater tempo preso, tempo de prisao provisoria, descontar a cautelar, ou pedir para computar o tempo ja cumprido."
---

# DETRACAO

> Camada 4 (execucao penal — LEP). Computa o tempo ja privado de liberdade na pena a cumprir. Fundacao da linha do tempo. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep "Art. 42"** (detracao).
- `context/lep-7210-84.md` — art. 111 (detracao na unificacao de penas), art. 66 (competencia do Juiz da Execucao — III-c).
- `context/cpp-3689-41.md` — art. 387 §2 (detracao na fixacao do regime inicial pelo juiz da condenacao — Lei 12.736/2012).
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Entregar o **tempo detraido** e o **impacto** dele na pena, no regime inicial e nos marcos (progressao, livramento) — fundamentado artigo a artigo.

## Quando ativar
- Apenado teve prisao provisoria, administrativa ou internacao a abater.
- Definir/conferir o regime inicial considerando o tempo ja preso.
- Antes de projetar progressao/livramento — a detracao desloca todas as datas.

## Metodologia
1. **Regra (CP art. 42).** Computam-se, na **pena privativa de liberdade** e na **medida de seguranca**, o tempo de **prisao provisoria** (no Brasil ou no estrangeiro), de **prisao administrativa** e de **internacao**. Identificar e somar todos os periodos de privacao de liberdade ja sofridos.
2. **Detracao na fixacao do regime inicial (CPP art. 387 §2 — Lei 12.736/2012).** O tempo de prisao provisoria/administrativa/internacao **e computado pelo juiz da condenacao para determinar o regime inicial**. Logo a detracao pode comecar ja na sentenca, nao so na execucao — conferir se o juiz aplicou; se nao, e tese de recurso/peticao.
3. **Detracao na unificacao (LEP art. 111).** Na soma/unificacao de penas, o regime sai do **resultado da soma observada a detracao** (e a remicao). Aplicar a detracao antes de definir o regime do conjunto.
4. **Competencia na execucao (LEP art. 66, III-c).** Na fase de execucao, a detracao e decidida pelo **Juiz da Execucao**.
5. **Impacto nos marcos.** Subtrair o tempo detraido do total -> obter o **saldo a cumprir** -> e SOBRE esse saldo que se projetam a progressao (`progressao-de-regime`) e o livramento (`livramento-condicional`). A detracao tambem pode **antecipar o regime inicial** (do fechado p/ semiaberto, p.ex.) via CPP 387 §2.
6. **Calcular:** somar periodos detraiveis -> abater da pena -> recalcular regime inicial (CPP 387 §2) e saldo -> reprojetar marcos -> entregar linha do tempo.

## Saida obrigatoria (calculo + data + parecer)
**Tempo detraido** (soma dos periodos, com datas) + **impacto** na pena/regime inicial/progressao/livramento (saldo a cumprir + datas reprojetadas) + fundamento (CP 42; CPP 387 §2; LEP 111, 66) + parecer + handoff. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum periodo/calculo sai sem `validador-criminal` (cruza `context/`). So e detraivel o tempo efetivo de prisao provisoria/administrativa/internacao (CP 42) — nao confundir com medidas cautelares diversas da prisao. Conferir se o regime inicial ja considerou a detracao (CPP 387 §2) antes de afirmar. Na duvida, bloquear e reler a lei seca. Gate final `suprema-corte-criminal`.

detracao -> arts. citados: CP 42; CPP 387 §2 (Lei 12.736/2012); LEP 111, 66 (III-c) — a detracao alimenta a linha do tempo do art. 112 LEP vigente (caput base 1/6, Lei 15.402/2026), cuja fracao/inciso e SEMPRE lida do arquivo, nunca decorada.
