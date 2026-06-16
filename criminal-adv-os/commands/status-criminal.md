---
description: Mostra o status do caso criminal ativo (reu, vitima, MP, tipo penal, fase da persecucao, situacao prisional, prazos e proxima providencia).
allowed-tools: Read, Grep, Glob
argument-hint: [nome do caso, opcional]
---

Voce foi acionado pelo comando `/status-criminal` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dar o panorama do caso.

## PROTOCOLO
1. Acionar `memoria-de-caso-criminal` — le `criminal/casos/<caso>.md` e resume: partes, imputacao, fase, situacao prisional, prazos e proximo passo.
2. Se houver mais de um caso, listar e perguntar qual.

**Skill a acionar:** `memoria-de-caso-criminal`.
