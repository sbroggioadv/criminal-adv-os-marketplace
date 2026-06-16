---
description: Conduz a execucao penal (LEP) — data-base, progressao de regime (art. 112 vigente 2026), livramento condicional, remicao, detracao, beneficios de saida e incidentes (falta grave, regressao).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [situacao da execucao / pena e regime]
---

Voce foi acionado pelo comando `/execucao-penal` do plugin criminal-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** calcular beneficios e datas na execucao.

## PROTOCOLO
1. Acionar `guia-de-execucao-penal` (data-base + linha do tempo) -> rotear para `progressao-de-regime` / `livramento-condicional` / `remicao` / `detracao` / `beneficios-saida-e-cautelares-penais` / `incidentes-execucao-penal`.
2. ⚠️ art. 112 da LEP = redacao vigente 2026 (Lei 15.402/2026 base 1/6 + excecoes; ler a NAO-tachada em context/). Nunca decorar percentual.
3. Fechar pela `suprema-corte-criminal`.

**Skill a acionar:** `guia-de-execucao-penal`.
