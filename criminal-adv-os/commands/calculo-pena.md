---
description: Motor de calculo de pena — recebe crime(s), datas, circunstancias e devolve pena final, regime, beneficios, fracoes de progressao/livramento, prescricao e a linha do tempo penal, tudo fundamentado na lei seca.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [crime + dados do caso]
---

Voce foi acionado pelo comando `/calculo-pena` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** calcular a pena completa, de forma auditavel.

## PROTOCOLO
1. Acionar `motor-calculo-de-pena` — ele aciona `dosimetria-da-pena` (3 fases), `concurso-de-crimes-e-penas` (se +1 crime), regime (CP 33), substituicao (CP 44)/sursis (CP 77), `prescricao-penal` e `progressao-de-regime`/`livramento-condicional`.
2. Tudo grounded em `context/` (CP/LEP) — nenhum numero de cabeca; lei vigente 2026.
3. Fechar pela `suprema-corte-criminal`.

**Skill a acionar:** `motor-calculo-de-pena`.
