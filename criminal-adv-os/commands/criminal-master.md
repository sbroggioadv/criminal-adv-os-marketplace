---
description: Porta unica da defesa penal — descreva o caso em linguagem natural e o criminal-master dirime todas as skills pertinentes (gestao processual, motor temporal, peca/recurso) e fecha pela suprema-corte-criminal.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descreva o caso ou a tarefa penal]
---

Voce foi acionado pelo comando `/criminal-master` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** conduzir a tarefa penal de ponta a ponta, sem esquecer nada.

## PROTOCOLO
1. Acionar a skill `criminal-master` — le a metodologia, classifica via `triagem-criminal`, carrega `memoria-de-caso-criminal`.
2. Gestao processual transversal (competencia/prazos/nulidades/estrategia) SEMPRE antes de peca/calculo.
3. Motor Penal Temporal quando cabivel (prescricao/dosimetria/calculo de pena/progressao) com a lei seca aberta.
4. Fechar pela `suprema-corte-criminal` (R1-R4) e atualizar a memoria do caso.

**Skill a acionar:** `criminal-master`.
