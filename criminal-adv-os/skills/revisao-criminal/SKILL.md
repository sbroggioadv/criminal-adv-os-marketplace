---
name: revisao-criminal
description: "Revisao criminal para desconstituir condenacao ja transitada em julgado, so em favor do reu (CPP arts. 621-631). Use para revisao criminal, desconstituir condenacao, prova nova, erro judiciario, rever a condenacao transitada em julgado, indenizacao por erro judiciario, ou citacao do art. 621 do CPP."
---

# REVISAO-CRIMINAL

> Camada 7 (recursos criminais). Acao autonoma de impugnacao que ataca a coisa julgada penal: desconstitui condenacao transitada SO PRO REO, a qualquer tempo. Foco: DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — grep os arts. 621-631 (hipoteses, prazo, competencia, procedimento, efeitos, indenizacao) e ler a faixa.
- `context/jurisprudencia-criminal.md` — so itens ✅ (ex.: Tema 1.016 art. 226 CPP pode lastrear prova nova/erro de reconhecimento).
- `context/penal-especial.md` — reformas 2024-2026 se a tese envolver lei especial.

## Objetivo
Reabrir processo findo quando a condenacao for injusta, com prova solida de uma das hipoteses do CPP art. 621, para absolver, desclassificar, reduzir a pena ou anular — sempre em beneficio do condenado.

## Quando ativar
Houve **transito em julgado** e surge: prova nova de inocencia, prova de que a condenacao se fundou em prova falsa, ou contrariedade ao texto da lei / evidencia dos autos. Tambem "prova nova", "erro judiciario", "rever condenacao", "621".

## Metodologia
1. **Hipoteses de cabimento — CPP art. 621** (taxativas):
   - **I** — sentenca condenatoria **contraria ao texto expresso da lei penal ou a evidencia dos autos**;
   - **II** — sentenca **fundada em depoimentos, exames ou documentos comprovadamente falsos**;
   - **III** — **prova nova** descoberta apos a sentenca, de inocencia do condenado ou de circunstancia que determine/autorize diminuicao especial da pena.
2. **So pro reo e a qualquer tempo — CPP art. 622.** Cabe em qualquer tempo, antes ou apos extinta a pena; vedada a reiteracao do pedido **salvo com nova prova** (art. 622, paragrafo unico). Persiste apos a morte do reu — `art. 631` manda nomear curador para a defesa.
3. **Legitimidade — CPP art. 623.** O proprio reu, procurador habilitado ou, **morto o reu**, conjuge, ascendente, descendente ou irmao.
4. **Competencia — CPP art. 624.** Julgam a revisao o STF (condenacoes por ele proferidas) e os Tribunais de Justica / TRFs nos demais casos, conforme regimento — nunca o juizo que sentenciou.
5. **Procedimento — CPP arts. 625-628.** Requerimento instruido com **certidao do transito em julgado** + pecas que comprovem os fatos (art. 625, § 1); relator nao pode ter decidido o caso (art. 625 caput); vista ao Procurador-Geral (art. 625, § 5).
6. **Efeitos — CPP art. 626.** Procedente, o tribunal pode **alterar a classificacao, absolver, modificar a pena ou anular o processo**; **vedada a reformatio in pejus** — nunca agravar a pena (art. 626, paragrafo unico). Absolvicao restabelece os direitos perdidos (art. 627).
7. **Indenizacao por erro judiciario — CPP art. 630.** Requerida na revisao, o tribunal pode reconhecer o direito a justa indenizacao (liquidada no civel), salvo as exclusoes do § 2 (erro imputavel ao proprio condenado; acusacao meramente privada).
8. **Prova nova de verdade.** Demonstrar que a prova e superveniente e idonea — nao mera reavaliacao do que ja estava nos autos.

## Entrega obrigatoria final
- Enquadramento na hipotese do art. 621 (I, II ou III) + comprovacao do transito em julgado + prova nova/documental anexada + competencia indicada (art. 624) + pedido coerente (absolver/desclassificar/reduzir/anular, art. 626) + pedido de indenizacao (art. 630) se cabivel.

## Guard
Fecha em `suprema-corte-criminal` (R1-R4); jurisprudencia so via `validador-criminal` e apenas itens ✅. Conferir a redacao vigente dos arts. 621-631 em `context/cpp-3689-41.md` antes de citar. Jamais propor revisao que agrave a situacao do reu (vedacao do art. 626, paragrafo unico). Sem prova nova idonea ou sem transito em julgado, bloquear.

revisao-criminal -> CPP art. 621 (I/II/III), 622, 623, 624, 625, 626 (e paragrafo unico — veda reformatio in pejus), 627, 630, 631.
