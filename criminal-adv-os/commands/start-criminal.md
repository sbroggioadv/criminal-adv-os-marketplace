---
description: Onboarding do plugin criminal-adv-os — apresenta o que faz e os caminhos por botoes (calcular pena, prescricao, execucao, ANPP, habeas corpus, recurso, juri, defesa).
allowed-tools: Read, Grep, Glob
argument-hint: [opcional: o que voce precisa]
---

Voce foi acionado pelo comando `/start-criminal` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dar as boas-vindas e rotear por botoes.

## PROTOCOLO
1. Acionar a skill `criminal-onboarding` — apresenta o plugin e oferece os botoes pertinentes.
2. Ao escolher, entregar ao `criminal-master` com o objetivo identificado.

**Skill a acionar:** `criminal-onboarding`.
