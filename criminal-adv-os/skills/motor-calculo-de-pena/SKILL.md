---
name: motor-calculo-de-pena
description: "Subsistema AUTONOMO que calcula a PENA COMPLETA de ponta a ponta — NUNCA numero de cabeca: recebe crimes/dispositivos/datas/circunstancias, aciona dosimetria-da-pena (3 fases) -> concurso-de-crimes-e-penas (se +1 crime) -> regime (33) -> substituicao (44)/sursis (77) -> prescricao-penal -> progressao-de-regime/livramento-condicional, e devolve pena final, regime, beneficios, fracoes, prescricao e a LINHA DO TEMPO PENAL. Use quando o operador disser calcular pena completa, motor de calculo, quanto vai pegar, pena final e beneficios, simular a pena."
---

# MOTOR-CALCULO-DE-PENA

> Camada 3 (subsistema autonomo — o §22 do PRD). Orquestra TODO o motor penal temporal numa entrega so: da dosimetria a linha do tempo da execucao. NENHUM numero de cabeca — o limite do art. 75 e os percentuais de progressao vem do `grep` na lei seca.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep** os artigos que cada subskill usa (59, 61-67, 68, 69-71, 33, 44, 77, 109-119). O numero pode quebrar de linha — ler o paragrafo inteiro.
- `context/lep-7210-84.md` — **art. 112 da LEP** (percentuais de PROGRESSAO) e **arts. 131-146 da LEP** (livramento condicional — procedimento). ⚠️ **Ler a redacao NAO-tachada VIGENTE** (art. 112 reescrito pela **Lei 15.402/2026** — base 1/6 + excecoes graduadas; camada hediondos **Lei 15.358/2026** Antifaccao V=70%/VI=75%/VII=80%/VIII=85%). **NAO usar os 16-70% de 2019 (tachados).**
- `context/penal-especial.md` — drogas (art. 42 Lei 11.343), hediondos, rol atualizado (Lei 15.159/2025).
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Responder "quanto vai pegar e quais beneficios" com calculo unico e auditavel: pena final, regime inicial, substituicao/sursis, prescricao e a linha do tempo penal (quando progride, quando alcanca livramento) — tudo fundamentado artigo a artigo.

## Quando ativar
- "Calcular pena completa" / "motor de calculo" / "quanto vai pegar" / "simular a pena".
- "Pena final e beneficios" / "monta a linha do tempo penal do reu".
- Sempre que a tarefa exigir DOSIMETRIA + CONCURSO + REGIME + PRESCRICAO + EXECUCAO numa entrega so.

## Metodologia (ORQUESTRA as subskills — cada numero vem da subskill, que grep a lei seca)
1. **ENTRADAS — coletar e travar antes de calcular:** crime(s) + dispositivo(s) legal(is) · datas (fato, recebimento da denuncia, sentenca, transito) · circunstancias judiciais do art. 59 (para a pena-base) · agravantes/atenuantes · majorantes/minorantes (fracoes do tipo) · reincidencia (e datas, p/ art. 64) · situacao prisional/detracao se houver. Faltou dado essencial -> **bloquear e pedir** (nao presumir numero).
2. **DOSIMETRIA (aciona `dosimetria-da-pena`):** roda as 3 fases do art. 68 para CADA crime — 1a pena-base (art. 59), 2a agravantes/atenuantes (61-67, Sumula 231 STJ a atenuante nao baixa do minimo), 3a causas de aumento/diminuicao (fracoes do tipo). Drogas -> dosimetria especial art. 42 da Lei 11.343.
3. **CONCURSO (aciona `concurso-de-crimes-e-penas` se +1 crime):** classifica material (69, soma) / formal (70, 1/6-1/2) / continuado (71, 1/6-2/3 ou ate o triplo), aplica e soma. **LIMITE de cumprimento — art. 75: ler o valor VIGENTE no anexo (40 anos, Lei 13.964/2019); NAO decorar.** Unifica se ultrapassar.
4. **REGIME INICIAL (art. 33, §2-§3):** pela pena final + art. 59 — >8 fechado; nao reincidente >4 a 8 semiaberto; nao reincidente ate 4 aberto (Sumula 440 STJ ✅: minimo veda regime mais gravoso so pela gravidade abstrata; SV 56 STF ✅).
5. **SUBSTITUICAO / SURSIS:** substituicao por restritivas (art. 44 — ate 4 anos, sem violencia/grave ameaca, nao reincidente doloso) OU sursis (art. 77 — ate 2 anos, ou 4 se >70/saude). Se cabe substituicao, em regra nao cabe sursis (art. 77, III).
6. **PRESCRICAO (aciona `prescricao-penal`):** verifica PPP (abstrata art. 109 pela pena maxima; retroativa/superveniente art. 110 pela pena aplicada) e PPE — com termos iniciais (111/112), interruptivas (117), suspensivas (116), reducao do art. 115. Se prescreveu, a punibilidade esta extinta — anotar na linha do tempo.
7. **EXECUCAO — Camada 4 (aciona `progressao-de-regime` e `livramento-condicional`):** sobre a pena final, calcular as **fracoes de progressao** do **art. 112 da LEP** (⚠️ **percentuais lidos da redacao VIGENTE no anexo** — base 1/6 + excecoes graduadas da Lei 15.402/2026; hediondos pela Lei 15.358/2026 V=70%/VI=75%/VII=80%/VIII=85%; **nunca os 16-70% de 2019, tachados**) e o **livramento condicional** (CP 83 + LEP arts. 131-146 — grep). Detracao (tempo de prisao provisoria) e remicao abatem da base, se houver.
8. **MONTAR A LINHA DO TEMPO PENAL:** inicio do cumprimento -> data prevista de cada progressao (% lido da LEP sobre a pena) -> data do livramento -> termino; cruzar com a prescricao executoria. Tudo datado e fundamentado.

## Saida obrigatoria
1. **Pena final** (anos/meses/dias) com o resumo das 3 fases por crime e o concurso aplicado.
2. **Regime inicial** (33) + **substituicao (44) / sursis (77)** cabiveis ou nao, fundamentados.
3. **Beneficios cabiveis** + **fracoes de progressao (art. 112 LEP, % VIGENTE do anexo)** e de **livramento (CP 83 / LEP 131-146)**, com a base de calculo.
4. **Prescricao** (prescreveu? qual especie? faltam quantos anos?).
5. **LINHA DO TEMPO PENAL completa** — inicio · progressoes datadas · livramento · termino · marcos de prescricao — tudo grounded.
6. Handoff ao `criminal-master`; passa pela `suprema-corte-criminal` (R4 refaz o calculo).

## Guard
⚠️ Tudo grounded — **nenhum numero de cabeca.** O **limite do art. 75 (40 anos)** e os **percentuais de progressao do art. 112 da LEP (redacao Lei 15.402/2026 + Lei 15.358/2026)** vem do `grep` no anexo, **lendo a redacao NAO-tachada VIGENTE** (jamais os 16-70% de 2019). Cada subskill passa pelo `validador-criminal` (cruza `context/`). Jurisprudencia so se ✅. Entrada incompleta, especie de prescricao, fracao ou percentual em duvida: bloquear e reler a lei seca. Calculo penal sob OAB = catastrofe se errado. Gate final `suprema-corte-criminal`.

motor-calculo-de-pena -> arts. citados: CP 59, 61-67, 68, 69-71, 33 (§2-§3), 44, 77, 83, 109-119; LEP art. 112 (progressao — **% lido do anexo, Lei 15.402/2026 + Lei 15.358/2026**) e arts. 131-146 (livramento condicional — procedimento); **limite art. 75 do CP lido do anexo: 40 anos (Lei 13.964/2019)**; Sumula 231 STJ (✅), Sumula 440 STJ (✅).
