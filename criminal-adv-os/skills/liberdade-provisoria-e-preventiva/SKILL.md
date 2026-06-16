---
name: liberdade-provisoria-e-preventiva
description: "Peca central da liberdade: revogar a prisao preventiva e obter liberdade provisoria (CPP 311-316, 319, 321-350) — contemporaneidade, fundamentacao concreta, cautelares diversas e fianca. Use quando o operador disser prisao preventiva, liberdade provisoria, revogar a preventiva, medidas cautelares, fianca, relaxar prisao, excesso de prazo."
---

# LIBERDADE-PROVISORIA-E-PREVENTIVA

> Camada 6 (defesa, liberdade & investigacao) — CENTRAL para a defesa. A prisao e a excecao; a liberdade, a regra. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (311-316, 319, 321-350) e ler a faixa.
- `context/jurisprudencia-criminal.md` — so item ✅.

## Objetivo
Demonstrar a ausencia ou o desaparecimento dos requisitos da preventiva e construir o pedido de liberdade provisoria (cautelares diversas e/ou fianca), com fundamentacao concreta.

## Quando ativar
- Cliente sob preventiva a revogar; pedido de liberdade provisoria com ou sem fianca.
- Preventiva por fundamentacao generica/gravidade abstrata; excesso de prazo; fato nao contemporaneo; cabimento de cautelar.

## Metodologia
1. **Cabimento e requisitos — CPP 311 e 312.** Preventiva decretada pelo juiz a requerimento do MP/querelante/assistente ou por representacao policial — nunca de oficio (311; oficio = ilegalidade). Requisitos (312): garantia da ordem publica/economica, conveniencia da instrucao ou aplicacao da lei penal, COM prova da existencia do crime + indicio de autoria + perigo do estado de liberdade. §2: motivacao em fatos NOVOS ou CONTEMPORANEOS; §4: incabivel por gravidade abstrata. Atacar cada pilar ausente.
2. **Hipoteses — CPP 313.** So em crime doloso com pena maxima superior a 4 anos (I), condenacao irrecorrivel por outro crime doloso em sentenca transitada em julgado — ressalvado CP 64 I (quinquenio depurador) (II), violencia domestica/familiar para garantir protetivas (III) ou integrante de orcrim ultraviolenta/milicia (V, Lei 15.358/2026). Fora delas, nao cabe. CPP 314: vedada se as provas indicarem excludente do art. 23 CP.
3. **Fundamentacao — CPP 315.** Decisao que decreta/substitui/denega e sempre motivada; §1 exige fatos novos ou contemporaneos; §2 (I-VI) lista 6 hipoteses de decisao NAO fundamentada (parafrase de ato normativo, conceito indeterminado, motivo generico, nao enfrentar argumentos, precedente/sumula sem fundamentos, ignorar precedente da parte). Incidencia em qualquer inciso = nulidade.
4. **Revogacao e REVISAO a cada 90 dias — CPP 316.** Caput: revoga se faltar motivo para subsistir. Par. un.: o orgao emissor revisa a manutencao **a cada 90 dias**, por decisao fundamentada, de oficio, **sob pena de tornar a prisao ilegal**. ⚠️ Conferir a redacao vigente no anexo. Falta de revisao = relaxamento.
5. **Cautelares DIVERSAS — CPP 319 (I-IX).** Comparecimento periodico, proibicoes (lugares/contato/ausentar-se da comarca), recolhimento domiciliar noturno, suspensao de funcao, internacao provisoria, fianca, monitoracao eletronica. Sempre oferecer a cautelar adequada e suficiente como alternativa (CPP 282).
6. **LIBERDADE PROVISORIA e fianca — CPP 321-350.** 321: ausentes os requisitos da preventiva, o juiz DEVE conceder liberdade, impondo cautelares se for o caso. 322: autoridade policial concede fianca ate 4 anos; nos demais, o juiz decide em 48h. 323-324: nao se concede fianca (racismo; tortura/trafico/terrorismo/hediondos; crimes contra o Estado Democratico; presentes os motivos da preventiva). Liberdade SEM fianca cabe quando esta for incabivel mas a preventiva nao se justificar.
7. **Teses recorrentes:** falta de contemporaneidade (312 §2 / 315 §1); fundamentacao generica (312 §4 / 315 §2); cautelares 319 menos gravosas; ausencia das hipoteses do 313; excesso de prazo; falta de revisao trimestral (316). Regime/vaga -> **SV 56** ✅.

## Entrega obrigatoria final
Requisito ausente (312/313/315) + tese principal (entre as do item 7) + pedido de liberdade provisoria com cautelares 319 e/ou fianca (321-350) + handoff ao `criminal-master`; se a prisao vier de flagrante, cross-link com `flagrante-e-audiencia-custodia`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo entra sem `validador-criminal` (cruza `context/cpp-3689-41.md` — conferir a redacao vigente do prazo de revisao do 316 par. un.). Jurisprudencia so se ✅. Foco DEFESA: a regra e a liberdade, a prisao e onus do Estado. Gate final `suprema-corte-criminal`.

liberdade-provisoria-e-preventiva -> arts. citados: CPP 282, 311, 312 (§§2,4), 313 (I-III,V), 314, 315 (§§1-2), 316 (par. un. — revisao 90 dias), 319 (I-IX), 321-325; CP 23; STF SV 56 (✅).
