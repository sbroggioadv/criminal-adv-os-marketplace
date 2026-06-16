---
description: Calcula a prescricao penal (PPP em abstrato/superveniente/retroativa/intercorrente, PPE, medidas de seguranca) com linha do tempo, marcos interruptivos/suspensivos e parecer conclusivo.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [crime, pena e datas dos marcos]
---

Voce foi acionado pelo comando `/prescricao` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** verificar se prescreveu e fundamentar.

## PROTOCOLO
1. Acionar `prescricao-penal` — usa CP 109-119 (grep na lei seca), monta a linha do tempo com os marcos (117 interruptivos, 116 suspensivos) e calcula.
2. Nunca prazo de memoria — sempre conferido em `context/cp-2848-40.md`.
3. Fechar pela `suprema-corte-criminal`.

**Skill a acionar:** `prescricao-penal`.
