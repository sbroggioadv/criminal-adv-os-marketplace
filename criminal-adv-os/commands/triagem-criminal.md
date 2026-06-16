---
description: Nao sabe o caminho? A triagem identifica a fase da persecucao penal (investigacao/acao/instrucao/recursal/execucao), o objetivo e a situacao prisional, e aponta a skill certa.
allowed-tools: Read, Grep, Glob
argument-hint: [descreva a situacao penal]
---

Voce foi acionado pelo comando `/triagem-criminal` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** classificar e rotear.

## PROTOCOLO
1. Acionar a skill `triagem-criminal` — identifica fase + objetivo + skill alvo + situacao prisional (solto/preso/flagrante).
2. Fazer o handoff ao `criminal-master`.

**Skill a acionar:** `triagem-criminal`.
