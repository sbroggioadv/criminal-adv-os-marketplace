---
name: rese
description: "Recurso em sentido estrito (RESE) — recurso contra as decisoes do ROL TAXATIVO do CPP 581 (rejeicao da denuncia/queixa, pronuncia, extincao da punibilidade e demais incisos). Use quando o operador disser recurso em sentido estrito, RESE, recorri da pronuncia, rejeicao da denuncia, recorrer do 581, ou descrever decisao interlocutoria criminal recorrivel por instrumento."
---

# RESE — Recurso em Sentido Estrito

> Camada 7 (recursos criminais). Foco DEFESA. Recurso de ROL TAXATIVO — so cabe nas hipoteses do CPP 581; fora delas, ou nao cabe RESE ou e caso de apelacao (581 nao serve onde cabe apelacao — 593 §4).

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (581 + 582-592 + 589) e ler a faixa. Confirmar a hipotese-chave (581 I rejeicao, 581 IV pronuncia) ANTES de afirmar cabimento.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Identificar se a decisao esta no rol do CPP 581, interpor RESE tempestivo, redigir razoes e aproveitar o juizo de retratacao (589).

## Quando ativar
- Decisao que **nao recebe** a denuncia ou a queixa (581, I).
- Decisao que **pronuncia** o reu (581, IV) — leva o reu a juri.
- Decisao que decreta prescricao ou extingue a punibilidade (581, VIII).
- Decisao que denega a apelacao ou a julga deserta (581, XV) — conferir tambem carta-testemunhavel-e-residuais.
- Qualquer outra hipotese do rol taxativo do CPP 581.

## Metodologia
1. **Confirmar o cabimento no rol (CPP 581).** Localizar a hipotese exata: I (rejeicao da denuncia/queixa), IV (pronuncia), VIII (extincao da punibilidade), XV (denegacao de apelacao), etc. Se a decisao nao estiver no rol e couber apelacao, **NAO e RESE** (CPP 593 §4 — apelacao afasta o RESE, ainda que so de parte).
2. **Tempestividade — CPP 586: 5 dias para interpor** (no caso do 581 XIV, 20 dias). ⚠️ Prazo PROCESSUAL conta pelo CPP 798 §1 (EXCLUI o dia do comeco) — cross-link `prazos-processuais-penais` para a data fatal. Nunca contar de cabeca.
3. **Razoes — CPP 588: 2 dias** apos a interposicao (ou da vista do traslado), com vista ao recorrido por igual prazo.
4. **Forma de subida (CPP 583).** Subem nos proprios autos os casos do 581 I, III, IV, VI, VIII e X; os demais por instrumento (traslado — CPP 587), indicando as pecas a trasladar.
5. **Juizo de retratacao — CPP 589: o juiz pode reformar ou sustentar** o despacho em 2 dias. ✅ Alavanca da defesa: razoes que convencam o proprio juiz a se retratar (ex.: receber a denuncia rejeitada nao interessa a defesa; ja a impronuncia/extincao em retratacao, sim). Se reformar, a parte contraria recorre por simples peticao (589 par. unico).
6. **Efeito (CPP 584).** Em regra so devolutivo; efeito suspensivo nas hipoteses do 584 (perda de fianca, livramento, 581 XV/XVII/XXIV). Recurso da pronuncia suspende so o julgamento (584 §2). Para o 581 V, pedido de efeito suspensivo/ativo ao ad quem (584 §4).
7. **Conteudo das razoes (DEFESA):** error in procedendo/in judicando + nulidades (cross-link `nulidades-penais`) + tese de fundo. Na pronuncia, atacar o juizo de admissibilidade (materialidade + indicios de autoria) e excessos de linguagem.

## Entrega obrigatoria final
Peticao de interposicao + razoes (combatendo a decisao do rol 581) + linha do tempo de tempestividade (CPP 586/588 via `prazos-processuais-penais`) + indicacao da forma de subida (583/587) + estrategia de retratacao (589) + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo/jurisprudencia/percentual sem `validador-criminal` (cruza `context/`). Confirmar a hipotese no rol do CPP 581 — RESE fora do rol e inadmissivel; onde cabe apelacao, usar apelacao (593 §4). Prazo SEMPRE pelo CPP 798 via `prazos-processuais-penais`, nunca de memoria. Jurisprudencia so se ✅. Gate final `suprema-corte-criminal`.

rese -> arts. citados: CPP 581 (I, IV, VIII, XV), 582, 583, 584 (§§2, 4), 586, 587, 588, 589, 593 §4; + CPP 798 (via prazos-processuais-penais).
