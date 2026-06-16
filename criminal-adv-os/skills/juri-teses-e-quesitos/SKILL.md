---
name: juri-teses-e-quesitos
description: "Coracao tecnico do juri: a quesitacao (CPP 482-491). Estrutura as teses defensivas e a ordem dos quesitos (CPP 483 — I materialidade, II autoria, III o quesito GENERICO o jurado absolve o acusado?, IV causa de diminuicao, V qualificadora/aumento), cuidando da votacao (CPP 487-490) e do quesito da desclassificacao/tentativa (483 §§4-5). Use quando o operador disser quesitos, quesitacao, teses do juri, terceiro quesito, absolvicao generica, perguntas aos jurados."
---

# JURI-TESES-E-QUESITOS

> Camada 8 (tribunal do juri) — CRITICA. O quesito mal formulado anula o julgamento ou condena o reu. O 3o quesito (absolvicao generica) e a arma defensiva mais forte do plenario. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (482-491) e ler a faixa. A numeracao quebra de linha — grepar tambem `^48[2-9]\.`, `^490\.`, `^491\.`.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Verter as teses defensivas em quesitos na ordem e redacao certas (CPP 483), preservar o 3o quesito (absolvicao generica) como porta de clemencia e impugnar quesitacao defeituosa para fundar nulidade (CPP 593 III "a", cross-link `juri-recursos`).

## Quando ativar
- Antes do plenario: definir a tese principal e as subsidiarias que viram quesito.
- No plenario, ao conferir o questionario lido pelo presidente (CPP 484).
- Apos o julgamento: detectar contradicao/defeito na quesitacao para o recurso.

## Metodologia
1. **O que se questiona — CPP 482.** O Conselho e questionado sobre **materia de fato** e **se o acusado deve ser absolvido**. Paragrafo unico: quesitos em **proposicoes afirmativas, simples e distintas**, claras e precisas, conforme pronuncia, interrogatorio e alegacoes.
2. **ORDEM DOS QUESITOS — CPP 483.** **I — materialidade do fato**; **II — autoria ou participacao**; **III — se o acusado deve ser absolvido**; **IV — causa de diminuicao de pena alegada pela defesa**; **V — qualificadora ou causa de aumento** reconhecida na pronuncia. §1: resposta negativa de **mais de 3 jurados** aos quesitos I ou II **encerra a votacao e absolve**. §2: respondidos afirmativamente I e II, formula-se **"O jurado absolve o acusado?"** — o **3o quesito GENERICO** (obrigatorio).
3. **⚠️ 3o QUESITO = ABSOLVICAO GENERICA / CLEMENCIA (CPP 483 III + §2).** Respondido **"sim"** por **mais de 3 jurados**, o reu e **absolvido** — por **qualquer fundamento, inclusive clemencia**, sem ancorar em tese juridica especifica. Arma defensiva central: mesmo com materialidade e autoria reconhecidas, a defesa sustenta a absolvicao pelo 3o quesito. (Amplitude da defesa/clemencia ligada a **ADPF 779** — citar so se ✅.)
4. **Fase de condenacao — CPP 483 §3.** Decidindo os jurados pela condenacao (3o quesito "nao"), seguem: **I — causa de diminuicao alegada pela defesa**; **II — qualificadora ou causa de aumento** da pronuncia.
5. **Desclassificacao e tentativa — CPP 483 §§4-6.** §4: sustentada a **desclassificacao** para crime do juiz singular, quesito proprio apos o 2o ou 3o. §5: sustentada a **forma tentada** ou divergencia de tipificacao (ainda do juri), quesito apos o 2o. §6: mais de um crime/acusado -> quesitos em **series distintas**.
6. **Conferencia e reclamacao — CPP 484.** O presidente le os quesitos e indaga sobre **requerimento ou reclamacao**, que constam da ata. **Reclamar na ata e essencial** — sem registro, preclui a nulidade da quesitacao no recurso.
7. **Votacao — CPP 487-490.** Sigilo do voto, apuracao por mais de 3 jurados. **CPP 490: contradicao nas respostas -> nova votacao** ou esclarecimento; persistindo, anota-se. Quesitacao contraditoria/defeituosa funda nulidade (CPP 593 III "a").
8. **Teses tipicas -> quesito:** negativa de autoria (II), atipicidade/excludentes e **clemencia** (3o quesito), privilegio/tentativa (IV / §5), desclassificacao para crime do juizo singular (§4). Mapear cada tese ao quesito antes do plenario.
9. **Gestao processual transversal.** Passar por `nulidades-penais`, `estrategia-penal` e `prazos-processuais-penais` antes de fechar.

## Entrega obrigatoria final
Mapa de teses -> quesitos na ordem do CPP 483 (com o 3o quesito generico destacado), redacao afirmativa simples de cada quesito, pontos de reclamacao a registrar em ata (CPP 484) e, se for o caso, minuta de impugnacao da quesitacao para recurso. Handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo/jurisprudencia entra sem `validador-criminal` (cruza `context/cpp-3689-41.md`). Jurisprudencia (ADPF 779 e afins) so se ✅. Respeitar a ordem legal dos quesitos (CPP 483 I-V) e a redacao afirmativa/simples (CPP 482 par. unico) — quesito fora de ordem ou complexo gera nulidade. Sempre preservar e explorar o 3o quesito (absolvicao generica). Foco DEFESA. Gate final `suprema-corte-criminal`.

juri-teses-e-quesitos -> arts. citados: CPP 482 (par. unico), 483 (I-V, §§1-6), 484, 485, 486, 487, 488, 489, 490, 491; ADPF 779 (so se ✅); CPP 593 III "a" (via juri-recursos).
