---
name: dosimetria-da-pena
description: "Calcula a pena pelo metodo TRIFASICO do art. 68 do CP — NUNCA numero de cabeca: 1a fase pena-base (8 circunstancias do art. 59), 2a fase agravantes/atenuantes (61-67, com Sumula 231 STJ a atenuante nao baixa do minimo), 3a fase causas de aumento/diminuicao (fracoes fixas), regime (33), substituicao (44), sursis (77), e dosimetria especial de drogas (art. 42 da Lei 11.343). Use quando o operador disser dosimetria, calcular a pena, pena-base, primeira fase, agravantes atenuantes, majorante minorante."
---

# DOSIMETRIA-DA-PENA

> Camada 3 (motor penal temporal). O calculo da pena propriamente dito. TODA faixa e fracao vem de `grep` na lei seca — zero numero de memoria. Foco DEFESA: puxar a pena para o minimo.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep CADA artigo** (59, 61, 62, 63, 64, 65, 66, 67, 68, 33, 44, 77) e ler a faixa. O numero pode quebrar de linha — ler o paragrafo inteiro. As fracoes das causas de aumento/diminuicao estao na **parte especial** (no tipo) — grep o artigo do crime.
- `context/penal-especial.md` — dosimetria ESPECIAL de drogas (art. 42 da Lei 11.343 — preponderancia sobre o art. 59 + natureza/quantidade). Ler antes de calcular crime de drogas.
- `context/jurisprudencia-criminal.md` — so citar item ✅ (Sumula 231 STJ ✅; Sumula 440 STJ ✅; Tema 585/Sumula 444 STJ ✅).

## Objetivo
Entregar a pena final auditavel pelo metodo trifasico: as 3 fases passo a passo, com fundamento legal artigo a artigo, mais regime inicial, substituicao/sursis e parecer — sempre defendendo a fixacao no minimo.

## Quando ativar
- "Dosimetria" / "calcular a pena" / "qual a pena que vai dar".
- Tese de pena-base no minimo, afastamento de agravante, reconhecimento de atenuante, reducao por minorante.
- Defesa em alegacoes finais/apelacao impugnando a dosimetria da sentenca.
- Dosimetria especial de drogas (art. 42 da Lei 11.343).

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Ponto de partida:** localizar o tipo penal e ler a **pena cominada (minimo e maximo)**. A pena-base parte do minimo e so sobe com fundamentacao concreta.
2. **1a FASE — pena-base (art. 68 c/c art. 59):** valorar as **8 circunstancias judiciais** do art. 59 — culpabilidade · antecedentes · conduta social · personalidade do agente · motivos · circunstancias · consequencias do crime · comportamento da vitima. Cada uma desfavoravel pode elevar; favoraveis/neutras mantem no minimo. ⚠️ **Inquerito/acao penal em curso NAO agrava** antecedentes/personalidade/conduta social (Tema 585 STJ / Sumula 444 STJ — ✅). Pena-base fica **entre o minimo e o maximo do tipo** (nunca extrapola nesta fase).
3. **2a FASE — agravantes e atenuantes:** sobre a pena-base aplicar **agravantes** (art. 61, rol; art. 62 no concurso de pessoas — quem promove/organiza, coage, instiga subordinado, paga) e **atenuantes** (art. 65, rol — menor de 21 ao fato/maior de 70 na sentenca, confissao, etc.; art. 66 atenuante inominada). **Reincidencia (art. 61, I; def. arts. 63-64)** agrava. ⚠️ **Sumula 231 STJ ✅: a atenuante NAO reduz a pena abaixo do minimo legal** (no mesmo sentido STF Tema 158/RE 597.270 ✅) — se a pena-base ja esta no minimo, a atenuante nao baixa mais; a agravante pode subir. **Concurso de circunstancias (art. 67):** a pena aproxima-se das **preponderantes** (motivos determinantes, personalidade, reincidencia). Sem fracao legal fixa — praxe ~1/6, sempre com fundamentacao concreta.
4. **3a FASE — causas de aumento e de diminuicao (majorantes/minorantes):** aplicar as **fracoes FIXAS previstas no tipo/parte geral** (ex.: tentativa art. 14, II = reduz de 1/3 a 2/3; participacao de menor importancia art. 29, §1 = reduz 1/6 a 1/3). ⚠️ Esta e a UNICA fase que **pode ultrapassar o minimo ou o maximo** do tipo. **Concurso de causas (art. 68, paragrafo unico):** havendo varias causas da parte especial, o juiz pode limitar-se a uma so, prevalecendo a que mais aumente/diminua. Grep a fracao no anexo — nunca decorar.
5. **DOSIMETRIA ESPECIAL DE DROGAS (art. 42 da Lei 11.343):** na 1a fase, a **natureza e a quantidade** da substancia preponderam SOBRE o art. 59 do CP (alem de personalidade e conduta social). **Trafico privilegiado (art. 33, §4 Lei 11.343)** = minorante de 1/6 a 2/3 (3a fase) — ler em `penal-especial.md`; **nao e hediondo** (Sumula 512 STJ cancelada — ❌, nao citar como vigente).
6. **REGIME INICIAL (art. 33, §2-§3):** pela pena FINAL + art. 59 — >8 anos = fechado; nao reincidente >4 a 8 = pode semiaberto; nao reincidente ate 4 = pode aberto. ⚠️ **Sumula 440 STJ ✅: minimo veda regime mais gravoso so pela gravidade abstrata.** SV 56 STF (falta de vaga nao mantem em regime mais gravoso) ✅.
7. **SUBSTITUICAO por restritivas (art. 44):** pena ate 4 anos + crime sem violencia/grave ameaca (ou culposo) + nao reincidente doloso + circunstancias favoraveis. Ate 1 ano = 1 restritiva ou multa; acima = 2 restritivas ou 1 + multa (§2).
8. **SURSIS (art. 77):** pena ate 2 anos (ate 4 se >70/saude — §2), nao reincidente doloso, circunstancias favoraveis, substituicao (art. 44) nao indicada/cabivel (III). Suspende por 2 a 4 anos.

## Saida obrigatoria
1. **Calculo fundamentado nas 3 fases, passo a passo:**
   - 1a fase: pena cominada (min/max), as 8 circunstancias do art. 59 valoradas uma a uma, pena-base fixada (e por que no minimo, na defesa).
   - 2a fase: agravantes (61-62) e atenuantes (65-66) reconhecidas, concurso (67), Sumula 231 STJ aplicada (nao baixa do minimo), pena intermediaria.
   - 3a fase: causas de aumento/diminuicao com a fracao do tipo (grep), art. 68 paragrafo unico se concorrerem, **pena definitiva**.
2. **Resultado:** pena privativa final (anos/meses/dias) + multa se houver + **regime inicial (33)** + **substituicao (44) / sursis (77)** cabiveis ou nao, com fundamento.
3. Handoff ao `criminal-master`; se houver +1 crime, acionar `concurso-de-crimes-e-penas`; passa pela `suprema-corte-criminal`.

## Guard
Nenhuma faixa/fracao sai sem `validador-criminal` (cruza `context/`) — toda pena cominada e toda fracao vem de `grep` no CP/tipo penal, nunca de memoria. Jurisprudencia so se ✅ (Sumula 231 STJ ✅ a atenuante nao baixa do minimo; Sumula 512 STJ = ❌, nao citar). Fase, base ou regime em duvida: bloquear e reler a lei seca. Calculo penal sob OAB = catastrofe se errado. Gate final `suprema-corte-criminal` (R4 refaz a dosimetria).

dosimetria-da-pena -> arts. citados: CP 59 (8 circunstancias), 61, 62, 63, 64, 65, 66, 67, 68 (caput + par. unico), 33 (§2-§3), 44, 77; Lei 11.343 art. 42 + art. 33 §4; Sumula 231 STJ (✅), Sumula 440 STJ (✅), Tema 585/Sumula 444 STJ (✅), STF Tema 158/RE 597.270 (✅).
