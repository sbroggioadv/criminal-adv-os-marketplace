---
name: lavagem-e-financeiros
description: "Defesa em lavagem de dinheiro (Lei 9.613/1998) — art. 1 (ocultar/dissimular natureza, origem, localizacao, movimentacao ou propriedade de bens provenientes de infracao penal; AUTONOMIA da lavagem; qualquer infracao antecedente apos Lei 12.683/2012; pena 3-10 anos + multa). Defesa: ausencia de dolo/ciencia da origem ilicita, atipicidade, exaurimento/consuncao no crime antecedente. Itens nao confirmados no anexo = 🟡. Use quando o operador disser lavagem de dinheiro, 9.613, ocultacao de bens, branqueamento, crime antecedente, dissimulacao."
---

# LAVAGEM-E-FINANCEIROS

> Camada 9 (leis penais especiais). Defesa em lavagem de capitais (Lei 9.613/1998). Foco: quebrar o dolo/ciencia da origem ilicita e atacar a autonomia da imputacao. Itens nao confirmados no anexo = 🟡.

## Anexos obrigatorios (context/)
- `context/penal-especial.md` secao 5 (Lei 9.613/1998) — **grep "art. 1", "lavagem", "antecedente", "12.683"** e ler o bloco + status ✅/🟡. Conferir antes de citar.
- `context/jurisprudencia-criminal.md` — teses correlatas (so citar ✅); na ausencia de tese confirmada para um ponto, marcar 🟡.

## Objetivo
Construir a tese de defesa em lavagem — atipicidade, ausencia de dolo/ciencia da origem, ou absorcao pelo crime antecedente — com o tipo e a regra de autonomia lidos do anexo, nunca de memoria.

## Quando ativar
- Imputacao de ocultacao/dissimulacao de bens, direitos ou valores de origem ilicita.
- Tese de ausencia de dolo, desconhecimento da origem, atipicidade ou consuncao no crime antecedente.
- Discussao sobre a autonomia do processo de lavagem frente a infracao antecedente.

## Metodologia (ARTIGOS REAIS do penal-especial.md — grep antes de afirmar)
1. **Tipo do art. 1º:** **ocultar ou dissimular** a natureza, origem, localizacao, disposicao, movimentacao ou propriedade de bens, direitos ou valores **provenientes, direta ou indiretamente, de infracao penal**. **Pena reclusao de 3 a 10 anos e multa.** Conduta nuclear = ocultar/dissimular — a defesa ataca a ausencia do verbo (mera fruicao/gasto do proveito, sem ato de ocultacao, e atipica).
2. **Antecedente — qualquer um (apos Lei 12.683/2012):** deixou de ser rol taxativo, passou a ser **qualquer infracao penal**. A defesa pode atacar a existencia/idoneidade do antecedente (sem indicios suficientes dele, nao ha lavagem).
3. **Autonomia (art. 2º, II) — dois gumes:** o processo da lavagem e **autonomo** e independe de processo/condenacao pelo antecedente, **bastando indicios suficientes** de sua existencia. Defesa: cobrar que existam ESSES indicios — sem eles, a imputacao autonoma nao se sustenta.
4. **TESE — dolo e ciencia:** lavagem exige **dolo** e **ciencia da origem ilicita**. Sustentar desconhecimento da procedencia (ausencia de elemento subjetivo) = tese central de absolvicao/atipicidade. Negar tambem **dolo eventual** quando o cenario nao permitia presumir ciencia.
5. **TESE — consuncao/exaurimento:** quando o agente so usufrui/esconde o proveito do proprio crime antecedente sem ato autonomo de reciclagem, sustentar **mero exaurimento** (post factum impunivel), nao lavagem autonoma. ⚠️ Controverso — sem tese ✅ no anexo, tratar como argumento doutrinario 🟡 e validar.
6. **Calculo de pena:** handoff `dosimetria-da-pena`. Cross-link `organizacao-criminosa-e-colaboracao` (lavagem frequente em orcrim) e `crimes-hediondos-e-equiparados` (status).

## Entrega obrigatoria final
- Tese identificada (atipicidade do verbo / ausencia de dolo-ciencia / ataque ao antecedente / consuncao) + art. 1º e regra de autonomia transcritos do anexo + alerta dos pontos 🟡 (consuncao, teses nao confirmadas) + handoff `dosimetria-da-pena` se houver calculo. Fecha pela `suprema-corte-criminal`.

## Guard
Nenhum tipo, pena, regra de autonomia ou tese entra em peca sem `validador-criminal` (cruza `context/`). So citar como ✅ o que estiver ✅ no anexo; teses controversas (consuncao, dolo eventual) e o que nao constar = 🟡, BLOQUEAR e checar. Na duvida de vigencia/teor, reler o anexo. Gate final `suprema-corte-criminal` (R2 lei vigente · R3 jurisprudencia real).

lavagem-e-financeiros -> arts. citados: Lei 9.613/1998 art. 1º (ocultar/dissimular bens de infracao penal; pena 3-10 anos + multa), art. 2º, II (autonomia — basta indicios do antecedente); Lei 12.683/2012 (antecedente = qualquer infracao penal). Teses de dolo/ciencia e consuncao = 🟡 (validar). Fonte: penal-especial.md secao 5 + jurisprudencia-criminal.md.
