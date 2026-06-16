---
name: carta-testemunhavel-e-residuais
description: "Carta testemunhavel (CPP 639-646) contra a decisao que DENEGA o recurso ou obsta seu seguimento/expedicao, e recursos residuais (correicao parcial). Use quando o operador disser carta testemunhavel, denegaram o recurso, obstaram o recurso, nao deixaram o recurso subir, correicao parcial, ou 639."
---

# CARTA-TESTEMUNHAVEL-E-RESIDUAIS

> Camada 7 (recursos criminais). Foco DEFESA. Recurso-instrumento de destrancamento: nao discute o merito do recurso denegado — forca o seu seguimento ao juizo ad quem.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (639, 640, 643, 646) e ler a faixa.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Destrancar recurso indevidamente denegado/obstado via carta testemunhavel, e mapear o residual (correicao parcial) quando o vicio for de procedimento, nao de denegacao de recurso.

## Quando ativar
- Decisao que **denega** o recurso (CPP 639, I).
- Decisao que, admitindo o recurso, **obsta sua expedicao/seguimento** ao ad quem (CPP 639, II).
- ⚠️ Se a denegacao for de APELACAO, ha via propria pelo RESE (CPP 581, XV — cross-link `rese`); a carta cobre o que nao tem recurso especifico.
- Error in procedendo / inversao tumultuaria sem recurso proprio -> correicao parcial (residual).

## Metodologia
1. **CARTA TESTEMUNHAVEL — cabimento (CPP 639):** I = decisao que denega o recurso; II = decisao que, admitindo o recurso, obsta sua expedicao e seguimento ao ad quem. Nao se discute o merito do recurso trancado — discute-se o trancamento.
2. **Prazo e forma — CPP 640: 48 HORAS** seguintes ao despacho que denegar, requerida **ao escrivao** (ou secretario do tribunal), indicando as pecas a trasladar. ⚠️ Prazo PROCESSUAL conta pelo CPP 798 — cross-link `prazos-processuais-penais` para confirmar o termo inicial e a fatal; nunca de cabeca.
3. **Processamento.** O escrivao da recibo e extrai a carta (CPP 641); recusa = sancao + avocacao pelo ad quem (642). Extraido o instrumento, observa-se o disposto nos CPP 588-592 (643). O tribunal manda processar o recurso ou ja decide o merito se instruido (644); na superior, segue o rito do recurso denegado (645).
4. **Efeito — CPP 646: a carta testemunhavel NAO tem efeito suspensivo.** Se houver risco de execucao no intervalo, ponderar HC/medida cautelar em paralelo (cross-link `habeas-corpus`).
5. **RESIDUAL — correicao parcial (descritivo):** reclamacao contra error in procedendo / inversao tumultuaria do processo, quando NAO houver recurso especifico. **Base legal nao e do CPP** — vem das leis de organizacao judiciaria estaduais e dos regimentos internos dos tribunais. ⚠️ NAO afirmar artigo de CPP; descrever a natureza e remeter ao regimento/lei local — confirmar no `validador-criminal` antes de citar dispositivo.
6. **Conteudo (DEFESA):** carta = demonstrar que o recurso era cabivel/tempestivo e foi indevidamente trancado. Correicao = demonstrar o tumulto/inversao procedimental e o prejuizo.

## Entrega obrigatoria final
Identificacao do instrumento (carta testemunhavel x correicao parcial) + peca/requerimento redigido (carta = ataca o trancamento, indica pecas a trasladar) + linha do tempo de tempestividade (carta = 48 horas, CPP 640, via `prazos-processuais-penais`) + alerta de ausencia de efeito suspensivo (646) + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo/jurisprudencia sem `validador-criminal` (cruza `context/`). Carta testemunhavel so contra denegacao/obstrucao de recurso (CPP 639) — nao e via de merito. Correicao parcial: base legal ESTADUAL/REGIMENTAL, NUNCA atribuir artigo do CPP de cabeca. Prazo de 48 horas (CPP 640) pelo CPP 798 via `prazos-processuais-penais`, nunca de memoria. Jurisprudencia so se ✅. Gate final `suprema-corte-criminal`.

carta-testemunhavel-e-residuais -> arts. citados: CPP 639 (I, II), 640 (48 horas), 641, 642, 643 (remete 588-592), 644, 645, 646 (sem efeito suspensivo), 581 XV (cross RESE); correicao parcial = base estadual/regimental (descritivo, sem artigo CPP); + CPP 798 (via prazos-processuais-penais).
