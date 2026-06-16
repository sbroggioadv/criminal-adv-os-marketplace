---
name: flagrante-e-audiencia-custodia
description: "Atacar a prisao em flagrante e municiar a audiencia de custodia (CPP 301-310) — vicios do auto, nota de culpa, comunicacao em 24h, e o trinomio do art. 310 (relaxar a prisao ilegal · converter em preventiva · conceder liberdade). Use quando o operador disser flagrante, audiencia de custodia, preso em flagrante, relaxamento de prisao, auto de prisao em flagrante."
---

# FLAGRANTE-E-AUDIENCIA-CUSTODIA

> Camada 6 (defesa, liberdade & investigacao). Primeira porta da liberdade: o flagrante e o filtro do art. 310. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (301-310) e ler a faixa. Atencao: art. 310 caput tem redacao da Lei 15.358/2026 (videoconferencia).
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Diagnosticar o flagrante (especie e vicios), checar prazos e comunicacoes obrigatorias e estruturar o pleito na custodia: relaxamento do flagrante ilegal ou liberdade, em vez da conversao em preventiva.

## Quando ativar
- Cliente preso em flagrante (agora ou nas ultimas horas); custodia designada ou nao realizada no prazo.
- Auto de prisao em flagrante com vicio formal/material; conversao do flagrante em preventiva ja decretada e a atacar.

## Metodologia
1. **Especie de flagrante — CPP 302.** Enquadrar: I esta cometendo · II acaba de cometer · III perseguido logo apos (presumido) · IV encontrado logo depois com instrumentos/objetos. Atacar o flagrante forjado/provocado/esperado e o "logo apos/depois" alargado (III/IV) sem situacao que presuma a autoria.
2. **Auto de prisao em flagrante — CPP 304.** Conferir a ordem dos atos (condutor, testemunhas, interrogatorio, lavratura) e as formalidades; §2 (duas pessoas que testemunharam a apresentacao, se faltam testemunhas do fato). Vicio de forma = base de relaxamento.
3. **Comunicacao e prazos — CPP 306.** A prisao e o local sao comunicados imediatamente ao juiz competente, ao MP e a familia/pessoa indicada. §1: em ate 24h o auto e encaminhado ao juiz e, sem advogado informado, copia integral a Defensoria. §2: nota de culpa entregue ao preso, com o motivo da prisao e o nome do condutor e das testemunhas. Falta de nota ou estouro das 24h = materia de relaxamento.
4. **AUDIENCIA DE CUSTODIA — CPP 310 (caput, Lei 15.358/2026).** Recebido o auto, no prazo maximo de 24h apos a prisao, o juiz realiza a custodia (videoconferencia em tempo real, com acusado, defensor/Defensoria e MP) e, fundamentadamente, decide o trinomio: **I — relaxa a prisao ILEGAL** (especie nao configurada, auto viciado, 306 descumprido); **II — converte em PREVENTIVA** so se presentes os requisitos do 312 e as hipoteses do 313, e inadequadas/insuficientes as cautelares do 319 (a defesa sustenta insuficiencia da fundamentacao 315 e cabimento de cautelares); **III — concede LIBERDADE PROVISORIA**, com ou sem fianca.
5. **Liberdade por excludente — CPP 310 §1.** Verificada pelo auto qualquer das condicoes do art. 23, I-III do CP, o juiz pode conceder liberdade mediante termo de comparecimento. Levantar excludente desde a custodia.
6. **Nao realizacao no prazo — CPP 310 §4.** Transcorridas 24h apos o decurso do prazo do caput, a nao realizacao da custodia sem motivacao idonea enseja a ilegalidade da prisao, a ser relaxada (sem prejuizo da §3 — responsabilidade da autoridade omissa).
7. **Garantias do ato — CPP 310 §§9-11.** Entrevista previa reservada e inviolavel com o defensor (§9), privacidade do preso (§10), repeticao integral em falha de comunicacao do tribunal (§11) — vicio dessas garantias contamina o ato.
8. Flagrante apoiado em **reconhecimento sem o rito do art. 226 CPP** -> somar **STJ Tema 1.016** (✅).

## Entrega obrigatoria final
Diagnostico do flagrante (especie 302 + vicios 304/306) + pleito na custodia pelo trinomio do 310 (I relaxamento / III liberdade, afastando a conversao 310-II) + excludente (310 §1) e/ou omissao do ato (310 §4) quando cabivel + handoff ao `criminal-master`; cross-link com `liberdade-provisoria-e-preventiva`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo entra sem `validador-criminal` (cruza `context/cpp-3689-41.md` — ler a redacao NAO-tachada do art. 310). Jurisprudencia so se ✅. Foco DEFESA: a custodia e oportunidade de liberdade, nao de validacao do flagrante. Gate final `suprema-corte-criminal`.

flagrante-e-audiencia-custodia -> arts. citados: CPP 301, 302 (I-IV), 304 (§2), 306 (§§1-2), 310 (caput, I-III, §§1, 4, 9-11), 312, 313, 319; CP 23 (I-III); STJ Tema 1.016 (✅).
