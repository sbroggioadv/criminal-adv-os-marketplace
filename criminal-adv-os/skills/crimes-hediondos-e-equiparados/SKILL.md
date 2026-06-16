---
name: crimes-hediondos-e-equiparados
description: "Defesa em crimes hediondos e equiparados (Lei 8.072/1990) — le o ROL VIGENTE do art. 1 (atualizado ate 2024-2026: homicidio qualificado, feminicidio I-B Lei 14.994/2024, vicaricidio I-C Lei 15.384/2026, estupro, etc.) e as consequencias do art. 2 (insuscetibilidade de graca/anistia/indulto/fianca; progressao e livramento). Tese de defesa: AFASTAR a hediondez (ex.: trafico privilegiado NAO e hediondo). Use quando o operador disser crime hediondo, 8.072, rol de hediondos, equiparado a hediondo, progressao em hediondo, afastar hediondez."
---

# CRIMES-HEDIONDOS-E-EQUIPARADOS

> Camada 9 (leis penais especiais). Status de hediondez e seus efeitos pela Lei 8.072/1990. Foco DEFESA: afastar a hediondez e seus regimes mais gravosos. Calculo de progressao/livramento = cross-link.

## Anexos obrigatorios (context/)
- `context/penal-especial.md` secao 2 (Lei 8.072/1990) — **grep "art. 1", "art. 2", "I-B", "I-C", "Antifaccao"**, ler o ROL VIGENTE + status. ⚠️ A redacao mudou em 2024-2026 — usar SEMPRE a do anexo.
- `context/jurisprudencia-criminal.md` — SV 26, SV 56, status do trafico privilegiado; so citar item ✅.

## Objetivo
Dizer se o crime e (ou nao e) hediondo/equiparado pela redacao vigente, declarar as consequencias e construir a tese de afastamento da hediondez — tudo lido do anexo.

## Quando ativar
- Saber se um crime e hediondo/equiparado e qual o regime de beneficios.
- Tese de afastar a hediondez (ex.: trafico privilegiado nao hediondo; desclassificacao para tipo fora do rol).
- Discussao de progressao/livramento em hediondo, regime inicial, vedacao de graca/fianca.

## Metodologia (ARTIGOS REAIS do penal-especial.md — grep antes de afirmar)
1. **Ler o ROL VIGENTE do art. 1º (conferido no anexo 2026-06-15):** **I** homicidio em grupo de exterminio e **qualificado (121, §2º)** (Lei 15.159/2025); **I-A** lesao gravissima/seguida de morte contra autoridades e em instituicao de ensino; **I-B feminicidio (121-A)** (Lei 14.994/2024 — crime AUTONOMO, nao mais qualificadora); **I-C vicaricidio (121-B)** (Lei 15.384/2026); roubo e extorsao qualificados; **estupro (213)** e **de vulneravel (217-A)**; **paragrafo unico** (genocidio, armas de uso proibido, orcrim direcionada a hediondo, e — Lei 15.358/2026 Antifaccao — **dominio social estruturado**). ⚠️ Conferir o inciso exato no anexo; o rol foi reescrito.
2. **Consequencias do art. 2º:** hediondos/tortura/trafico/terrorismo sao **insuscetiveis de I anistia, graca e indulto; II fianca**. **§1º** — pena cumprida **inicialmente em regime fechado** (STF afastou a obrigatoriedade absoluta — HC 111.840 — mas e a regra inicial). ⚠️ **O §2º (2/5 e 3/5) foi REVOGADO pela Lei 13.964/2019** — NAO citar.
3. **SV 26 e SV 56 ✅:** o regime integralmente fechado e a vedacao generica de progressao sao inconstitucionais — **SV 26** permite progressao (juiz pode exigir exame criminologico por decisao fundamentada); **SV 56** (falta de vaga nao mantem em regime mais gravoso).
4. **Progressao e livramento (cross-link, nao decorar):** progressao segue o **art. 112 da LEP** (VIGENTE: Lei 15.402/2026 base 1/6 + excecoes; fracoes da Lei 15.358/2026 — V=70%, VI=75%, VII=80%, VIII=85% reincidente+hediondo+morte). ⚠️ Os 16-70% de 2019 estao TACHADOS — NAO usar. Calculo = `progressao-de-regime`. Livramento apos **2/3** (art. 5º Lei 8.072 + art. 83, V, CP), vedado ao reincidente especifico = `livramento-condicional`.
5. **TESE — afastar a hediondez:** mostrar que o crime NAO esta no rol vigente, desclassifica-lo para tipo fora do rol, ou reconhecer o **trafico privilegiado (art. 33, §4º), que NAO e equiparado a hediondo** ✅ (Sumula 512 STJ cancelada / STF HC 118.533), destravando progressao pelas fracoes comuns. Cross-link `lei-de-drogas`.

## Entrega obrigatoria final
- Status de hediondez pelo rol vigente do art. 1º + consequencias do art. 2º (graca/fianca/regime) + tese de afastamento (se cabivel) + cross-link `progressao-de-regime` e `livramento-condicional`. Fecha pela `suprema-corte-criminal`.

## Guard
Nenhum enquadramento no rol, consequencia ou tese entra em peca sem `validador-criminal` (cruza `context/`). ⚠️ O rol e as fracoes mudaram em 2024-2026 — usar SO a redacao do anexo. §2º da Lei 8.072 = ❌; equiparacao do privilegiado a hediondo = ❌. Na duvida, BLOQUEAR e reler o anexo. Gate final `suprema-corte-criminal` (R2 lei vigente · R3 jurisprudencia real).

crimes-hediondos-e-equiparados -> arts.: Lei 8.072/1990 art. 1º (rol: I, I-A, I-B feminicidio, I-C vicaricidio, estupro, dominio social estruturado), art. 2º (graca/anistia/indulto/fianca; §1º regime inicial fechado; §2º ❌), art. 5º (livramento 2/3); CP 121-A, 121-B, 33 §4º (privilegiado NAO hediondo ✅); LEP 112 + CP 83 V (cross-link); SV 26 ✅, SV 56 ✅. Fonte: penal-especial.md secao 2 + jurisprudencia.
