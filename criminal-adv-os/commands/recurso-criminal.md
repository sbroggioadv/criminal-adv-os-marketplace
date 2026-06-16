---
description: Escolhe e redige o recurso criminal correto (RESE, apelacao, embargos de declaracao/infringentes, REsp/RE, carta testemunhavel, revisao criminal) com admissibilidade e tempestividade.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [decisao a recorrer]
---

Voce foi acionado pelo comando `/recurso-criminal` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** recorrer da decisao certa, no recurso certo.

## PROTOCOLO
1. Identificar a decisao: rol do art. 581 (pronuncia, rejeicao) -> `rese`; sentenca/decisao do juri -> `apelacao-criminal`; vicio no acordao -> `embargos-criminais`; ultima instancia vs lei federal/CF -> `recursos-excepcionais-criminais`; denegacao de recurso -> `carta-testemunhavel-e-residuais`; condenacao transitada com prova nova/erro -> `revisao-criminal`.
2. SEMPRE `prazos-processuais-penais` (CPP 798 exclui o dia do comeco) + admissibilidade.
3. Fechar pela `suprema-corte-criminal`.

**Skill a acionar:** o recurso correspondente.
