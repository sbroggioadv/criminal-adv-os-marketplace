---
description: Faz a dosimetria trifasica da pena (CP 68) — 1a fase circunstancias judiciais (art. 59), 2a agravantes/atenuantes, 3a majorantes/minorantes — com regime inicial e substituicao.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [crime + circunstancias]
---

Voce foi acionado pelo comando `/dosimetria` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** calcular a pena nas 3 fases.

## PROTOCOLO
1. Acionar `dosimetria-da-pena` — 1a fase (art. 59), 2a (61-67, Sumula 231 atenuante nao abaixo do minimo), 3a (majorantes/minorantes); regime (CP 33), substituicao (CP 44), sursis (CP 77). Drogas: art. 42 da Lei 11.343.
2. Tudo grounded; fechar pela `suprema-corte-criminal`.

**Skill a acionar:** `dosimetria-da-pena`.
