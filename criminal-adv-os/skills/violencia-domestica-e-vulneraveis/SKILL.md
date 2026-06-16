---
name: violencia-domestica-e-vulneraveis
description: "Defesa do ACUSADO em violencia domestica (Lei 11.340/2006 — Maria da Penha): medidas protetivas de urgencia (arts. 22-24), natureza da acao penal (lesao corporal = INCONDICIONADA, ADI 4.424 + Sumula 542 STJ; ameaca = condicionada a representacao), nao aplicacao da Lei 9.099 (art. 41). Lado defesa: contraditorio nas protetivas, proporcionalidade, atipicidade, prova; vitima vulneravel/crianca (ECA). Use quando o operador disser maria da penha, violencia domestica, medida protetiva, 11.340, defesa em violencia domestica, descumprimento de protetiva."
---

# VIOLENCIA-DOMESTICA-E-VULNERAVEIS

> Camada 9 (leis penais especiais) — lado DEFESA do acusado. Maria da Penha (Lei 11.340/2006) e protecao de vulneraveis. Foco: contraditorio nas protetivas, proporcionalidade, atipicidade e prova. Nao e advocacia da vitima.

## Anexos obrigatorios (context/)
- `context/penal-especial.md` secao 6 (Lei 11.340/2006) — **grep "art. 22", "art. 24-A", "art. 41", "acao penal"**, ler o bloco + status. Conferir antes de citar.
- `context/jurisprudencia-criminal.md` — Sumula 542 STJ (lesao incondicionada ✅) e Sumula 593 STJ (vulneravel ✅); so citar ✅.

## Objetivo
Construir a defesa do acusado em violencia domestica — atacar a protetiva no contraditorio, sustentar proporcionalidade/atipicidade e fixar a natureza da acao penal — com os dispositivos lidos do anexo.

## Quando ativar
- Cliente acusado/intimado em violencia domestica ou descumprimento de protetiva.
- Tese de revisao/revogacao de protetiva, atipicidade ou insuficiencia de prova.
- Duvida sobre a natureza da acao penal (lesao x ameaca) ou aplicabilidade da Lei 9.099.

## Metodologia (ARTIGOS REAIS do penal-especial.md — grep antes de afirmar)
1. **Medidas protetivas (arts. 22-24):** o **art. 22** (obrigam o agressor) — restricao do porte de armas, **afastamento do lar**, **proibicao de aproximacao e de contato** (distancia minima), proibicao de frequentar lugares, restricao de visitas, alimentos provisorios. **Art. 23** (favor da ofendida) e **art. 24** (patrimoniais). A defesa conhece o conteudo exato da protetiva para impugnar excesso/desproporcao.
2. **DEFESA nas protetivas — natureza cautelar ✅:** sao **cautelares** — exigem **fumus boni iuris e periculum**; cabem **contraditorio, revisao e revogacao** cessado o risco. Atacar a ausencia de fundamentacao concreta do risco e a desproporcao (ex.: afastamento sem suporte fatico).
3. **Descumprimento (art. 24-A):** crime de **reclusao de 3 meses a 2 anos**, mas **exige protetiva valida, devidamente intimada e ciencia inequivoca** do agressor. Ataque defensivo: protetiva irregular, ausencia de intimacao valida, falta de ciencia inequivoca = atipicidade.
4. **Natureza da acao penal:** **lesao corporal** em violencia domestica contra a mulher = **ACAO PENAL PUBLICA INCONDICIONADA** ✅ (STF ADI 4.424 + ADC 19; **Sumula 542 STJ**) — independe de representacao e nao comporta retratacao. Ja a **ameaca** segue **condicionada a representacao** — discutir falta/retratacao da representacao quando a acao for condicionada.
5. **Nao aplicacao da Lei 9.099 (art. 41):** aos crimes com violencia domestica contra a mulher **nao se aplica a Lei 9.099/1995** — afasta transacao penal e suspensao do processo. A defesa nao pleiteia despenalizadores incabiveis e redireciona a estrategia (atipicidade, prova, dosimetria).
6. **Vulneraveis (cross-link):** vitima crianca/adolescente — **estupro de vulneravel (art. 217-A, hediondo)** + **Sumula 593 STJ** ✅ (irrelevancia do consentimento de menor de 14) = `crimes-hediondos-e-equiparados`. Adolescente infrator = **ato infracional do ECA** (fronteira; nao e crime). Calculo = `dosimetria-da-pena`.

## Entrega obrigatoria final
- Tese defensiva (revisao/revogacao da protetiva / atipicidade do art. 24-A / acao penal / insuficiencia de prova) + dispositivos dos arts. 22-24, 24-A, 41 do anexo + fixacao da acao penal (lesao incondicionada ✅ / ameaca condicionada) + cross-link `crimes-hediondos-e-equiparados` e `dosimetria-da-pena`. Fecha pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo, natureza de acao penal ou tese entra em peca sem `validador-criminal` (cruza `context/`). Sumulas 542 e 593 STJ so se ✅ no anexo. Na duvida de teor/vigencia, BLOQUEAR e reler. Foco DEFESA do acusado — nao confundir com tutela da vitima. Gate final `suprema-corte-criminal` (R2 lei vigente · R3 jurisprudencia real).

violencia-domestica-e-vulneraveis -> arts.: Lei 11.340/2006 arts. 22-24 (protetivas), 24-A (descumprimento, reclusao 3 meses-2 anos), 41 (nao aplica Lei 9.099); lesao INCONDICIONADA (STF ADI 4.424 + ADC 19, Sumula 542 STJ ✅) x ameaca condicionada; CP 217-A + Sumula 593 STJ ✅ (cross-link); ECA (ato infracional). Fonte: penal-especial.md secao 6 + jurisprudencia.
