---
description: Avalia e estrutura acordos penais — ANPP (CPP 28-A), transacao penal e suspensao condicional do processo (Lei 9.099) — verificando cabimento e negociando as melhores condicoes para o cliente.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [crime e situacao do cliente]
---

Voce foi acionado pelo comando `/anpp` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** buscar o acordo penal cabivel mais favoravel.

## PROTOCOLO
1. Classificar o cabimento: pena minima < 4 anos sem violencia/grave ameaca -> `anpp` (CPP 28-A); menor potencial ofensivo (pena max 2 anos) -> `transacao-penal`; pena minima <= 1 ano -> `suspensao-condicional-processo`. Pena ja aplicada <= 2 anos -> `sursis-penal`.
2. Conferir requisitos e vedacoes na lei seca; itens da Lei 9.099 -> validar ao vivo.
3. Fechar pela `suprema-corte-criminal`.

**Skill a acionar:** `anpp` (ou a skill de acordo correspondente).
