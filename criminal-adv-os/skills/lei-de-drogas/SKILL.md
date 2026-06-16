---
name: lei-de-drogas
description: "Defesa em crimes da Lei 11.343/2006 — porte para uso (art. 28, maconha NAO e infracao penal: Tema 506 STF, ate 40g/6 plantas, presuncao relativa), trafico (art. 33, pena 5-15 anos), trafico privilegiado (art. 33 §4, reducao 1/6 a 2/3, NAO hediondo), dosimetria especial (art. 42) e vedacoes (art. 44 lidas a luz do STF). Use quando o operador disser trafico, lei de drogas, 11.343, trafico privilegiado, porte para uso, art. 28, art. 33, desclassificacao de trafico, atipicidade de drogas."
---

# LEI-DE-DROGAS

> Camada 9 (leis penais especiais). Defesa em crimes da Lei 11.343/2006. NAO calcula pena sozinha — handoff a dosimetria-da-pena; foco em desclassificar, privilegiar e atipicar.

## Anexos obrigatorios (context/)
- `context/penal-especial.md` secao 1 (Lei 11.343/2006) — **grep "art. 28", "art. 33", "§4", "art. 42", "art. 44"** e ler o bloco + o status ✅/🟡. Conferir antes de citar.
- `context/jurisprudencia-criminal.md` — Tema 506 STF (maconha) e demais teses; so citar item ✅.

## Objetivo
Entregar a tese de defesa correta em crime de drogas — desclassificacao trafico->uso, reconhecimento do privilegiado, atipicidade — com o dispositivo lido do anexo, nunca de memoria.

## Quando ativar
- Imputacao de trafico (art. 33) ou porte para uso (art. 28).
- Tese de desclassificacao, trafico privilegiado, atipicidade ou minoracao por natureza/quantidade.
- Discussao de hediondez (privilegiado) ou vedacoes do art. 44.

## Metodologia (ARTIGOS REAIS do penal-especial.md — grep antes de afirmar)
1. **Tipicidade — uso x trafico (art. 28):** pune o porte **para consumo pessoal** (I advertencia · II prestacao de servicos · III medida educativa). O **§2º** manda olhar **natureza e quantidade**, local, condicoes da acao e antecedentes para decidir se era uso. Tese central: **desclassificar art. 33 -> art. 28**.
2. **Maconha — Tema 506 STF (RE 635.659) ✅:** porte de **maconha para consumo pessoal NAO e infracao penal** (ilicito administrativo) — so incisos I e III do art. 28. **Presuncao RELATIVA: ate 40 gramas OU 6 plantas femeas** = usuario. ⚠️ Relativa (afastavel por prova de trafico) e so para maconha (sem criterio fixo para outras drogas). Tese de atipicidade/desclassificacao.
3. **Trafico (art. 33):** tipo base, **pena reclusao 5 a 15 anos + 500-1.500 dias-multa**. A defesa ataca a prova do comercio/destinacao e busca desclassificacao ou privilegiado.
4. **Trafico privilegiado (art. 33, §4º):** pena **reduzida de 1/6 a 2/3** se o agente for, CUMULATIVAMENTE, **(a) primario, (b) bons antecedentes, (c) nao se dedicar a atividades criminosas, (d) nao integrar orcrim**. ✅ **NAO e equiparado a hediondo** (Sumula 512 STJ cancelada / STF HC 118.533) — chave para progressao e beneficios. Vedacao a restritivas superada (Resolucao SF 5/2012). Provar os 4 requisitos.
5. **Dosimetria especial (art. 42):** **natureza e quantidade** da substancia (+ personalidade/conduta social) **preponderam SOBRE o art. 59 do CP**. Na defesa, quantidade pequena milita pela pena no minimo e maior fracao do §4º. Calculo = handoff `dosimetria-da-pena`.
6. **Vedacoes (art. 44) a luz do STF:** veda fianca, sursis, graca, indulto, anistia e conversao em restritivas (art. 33 caput/§1º e 34-37); livramento apos **2/3** (vedado ao reincidente especifico). ⚠️ A vedacao **abstrata** a liberdade provisoria foi afastada pelo STF (HC 104.339) — cabe analise concreta do **art. 312 do CPP** para pleitear liberdade.

## Entrega obrigatoria final
- Tese identificada (desclassificacao / privilegiado / atipicidade / liberdade) + dispositivo transcrito do anexo + status de hediondez do privilegiado (NAO hediondo ✅) + handoff a `dosimetria-da-pena` se houver calculo. Cross-link `progressao-de-regime` / `livramento-condicional` para os beneficios. Fecha pela `suprema-corte-criminal`.

## Guard
Nenhum tipo, pena, fracao ou tese entra em peca sem `validador-criminal` (cruza `context/`). Tema 506 e demais teses so se ✅ no anexo; o parametro 40g/6 plantas e presuncao RELATIVA e so para maconha. Na duvida de vigencia/status (privilegiado nao hediondo, vedacao do art. 44), BLOQUEAR e reler o anexo. Gate final `suprema-corte-criminal` (R2 lei vigente · R3 jurisprudencia real).

lei-de-drogas -> arts. citados: Lei 11.343/2006 art. 28 (+§2º), 33, 33 §4º (privilegiado, NAO hediondo ✅), 42, 44; CPP 312; Tema 506 STF / RE 635.659 (✅ maconha ate 40g/6 plantas); Sumula 512 STJ (❌ cancelada) / STF HC 118.533 + HC 104.339. Fonte: penal-especial.md secao 1 + jurisprudencia-criminal.md.
