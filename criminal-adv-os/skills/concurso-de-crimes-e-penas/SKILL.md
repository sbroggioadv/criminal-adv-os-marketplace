---
name: concurso-de-crimes-e-penas
description: "Aplica o concurso de crimes — NUNCA numero de cabeca: concurso MATERIAL (art. 69, penas somadas), FORMAL (art. 70, mais grave + 1/6 a 1/2, ou soma se desigios autonomos), crime CONTINUADO (art. 71, pena de um + 1/6 a 2/3; par. unico continuidade especifica ate o triplo), LIMITE de cumprimento (art. 75 — confira o valor vigente no anexo) e unificacao, mais concurso de PESSOAS (arts. 29-31, autoria/participacao). Use quando o operador disser concurso de crimes, varios crimes, crime continuado, concurso formal, concurso material, limite da pena, concurso de agentes."
---

# CONCURSO-DE-CRIMES-E-PENAS

> Camada 3 (motor penal temporal). Como somar/aumentar penas de varios crimes e ate onde o reu cumpre. TODA fracao e o limite vem de `grep` na lei seca — zero numero de memoria. Foco DEFESA: enquadrar no concurso mais brando.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep CADA artigo** (29, 30, 31, 69, 70, 71, 75, 76) e ler a faixa. O numero pode quebrar de linha — ler o paragrafo inteiro. ⚠️ **O LIMITE do art. 75 NAO se decora — ler o valor VIGENTE no anexo** (esta na redacao da Lei 13.964/2019).
- `context/jurisprudencia-criminal.md` — so citar item ✅ (Sumula 443 STJ ✅ exige fundamentacao concreta no aumento; Sumula 711 STF ✅ lei mais grave no crime continuado/permanente). Sumula 715 STF (limite nao serve de base p/ beneficios) = 🟡 conferir antes de citar — nao consta como ✅ no anexo.

## Objetivo
Definir o tipo de concurso, calcular a soma/aumento de pena auditavel, somar o total e aplicar o limite de cumprimento do art. 75 — sempre com a tese defensiva do concurso mais favoravel.

## Quando ativar
- "Varios crimes" / "concurso de crimes" / "qual o total da pena".
- Tese de crime CONTINUADO (art. 71) em vez de concurso MATERIAL (art. 69) — defesa quer continuado (aumento de fracao << soma).
- "Limite da pena" / unificacao / ate onde cumpre.
- Concurso de PESSOAS (autoria, participacao, cooperacao dolosamente distinta).

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Classificar o concurso ANTES de calcular** — muda tudo:
   - **MATERIAL (art. 69):** mais de uma acao/omissao, dois ou mais crimes -> **penas SOMADAS (cumulativas)**. Reclusao executa-se antes da detencao. §1: aplicada PPL nao suspensa por um crime, e incabivel a substituicao (art. 44) nos demais.
   - **FORMAL (art. 70):** **uma so** acao/omissao, dois ou mais crimes -> aplica-se a **pena mais grave (ou uma se iguais) aumentada de 1/6 ate 1/2** (concurso formal proprio). ⚠️ **Exceto desigios autonomos** (acao dolosa + crimes de desigios autonomos) -> **somam-se** como no art. 69 (concurso formal improprio). Paragrafo unico: o aumento do formal proprio **nao pode exceder** o que daria a soma do art. 69 (concurso formal nao pode ser pior que o material).
   - **CONTINUADO (art. 71):** mais de uma acao/omissao, dois ou mais crimes **da mesma especie** + mesmas condicoes de tempo, lugar, modo (devem os seguintes ser tidos como continuacao) -> **pena de UM so dos crimes (se iguais) ou a mais grave (se diversas), aumentada de 1/6 a 2/3**. **Paragrafo unico — continuidade ESPECIFICA** (dolosos, vitimas diferentes, com violencia/grave ameaca): o juiz pode aumentar **ate o TRIPLO**, observados o par. unico do art. 70 e o art. 75.
2. **Calcular cada pena isolada PRIMEIRO** (cada crime passa pela `dosimetria-da-pena` — 3 fases), depois aplicar a regra do concurso. **Fracao** (formal/continuado) pela quantidade de crimes, com fundamentacao concreta: ⚠️ **Sumula 443 STJ ✅ — exige fundamentacao concreta quanto ao numero de crimes; nao se admite o patamar maximo sem justificativa.** Praxe (defesa): 2 crimes ~1/6, sobe com o numero. Grep o intervalo legal do artigo.
3. **Aplicar conforme o tipo:** material = somar todas; formal proprio = mais grave + 1/6 a 1/2; continuado = uma + 1/6 a 2/3 (ou ate o triplo no especifico).
4. **LIMITE de cumprimento (art. 75):** **ler o valor VIGENTE no anexo** — PPL **nao pode ser superior a 40 (quarenta) anos** (redacao Lei 13.964/2019). §1: somadas as penas alem do limite, **unificam-se**. §2: condenacao por fato POSTERIOR ao inicio do cumprimento -> **nova unificacao**, desprezado o periodo ja cumprido. **Conferir no `grep` — nunca decorar.**
5. **Limite x beneficios:** o art. 75 e teto de CUMPRIMENTO; a base dos beneficios de execucao discute-se a parte. **Sumula 715 STF (limite nao serve de base p/ beneficios) = 🟡 conferir** — nao consta como ✅ no anexo; remeter a `progressao-de-regime`/`livramento-condicional`. Multas: aplicadas distinta e integralmente (art. 72).
6. **CONCURSO DE PESSOAS (arts. 29-31):** **art. 29** — quem concorre responde na **medida da sua culpabilidade**; **§1 participacao de menor importancia** = reducao de **1/6 a 1/3**; **§2 cooperacao dolosamente distinta** (quis crime menos grave) = pena do menos grave, **aumentada ate metade** se previsivel o resultado mais grave. **Art. 30** — condicoes de carater pessoal nao se comunicam, salvo elementares. **Art. 31** — ajuste/determinacao/instigacao/auxilio nao sao puniveis se o crime nao chega a ser tentado. Distinguir **autor** (executa/domina) de **participe** — defesa busca o §1.

## Saida obrigatoria
1. **Tipo de concurso identificado** (material 69 / formal proprio ou improprio 70 / continuado 71 / continuidade especifica) com o fundamento factual (uma acao? mesma especie? desigios autonomos?).
2. **Calculo do aumento/soma:** penas isoladas (cada uma ja dosada) -> regra aplicada -> fracao (1/6 a 1/2, 1/6 a 2/3, ou ate o triplo) com fundamentacao concreta (Sumula 443 STJ) -> **total**.
3. **Limite do art. 75** aplicado: total bruto x limite VIGENTE lido no anexo (40 anos — Lei 13.964/2019); unificacao se ultrapassar (§1/§2).
4. **Concurso de pessoas** (se houver): autoria x participacao, §1/§2 do art. 29, e o reflexo na pena.
5. **Parecer:** concurso mais favoravel cabivel + total final + handoff ao `criminal-master`; passa pela `suprema-corte-criminal`.

## Guard
Nenhuma fracao/limite sai sem `validador-criminal` (cruza `context/`) — toda fracao e **o limite do art. 75** vem de `grep` no CP, nunca de memoria (⚠️ confira o valor vigente do art. 75 no anexo a cada uso). Jurisprudencia so se ✅ (Sumula 443 STJ ✅; Sumula 711 STF ✅; Sumula 715 STF = 🟡, conferir). Tipo de concurso ou fracao em duvida: bloquear e reler a lei seca. Calculo penal sob OAB = catastrofe se errado. Gate final `suprema-corte-criminal` (R4 refaz a soma e reconfere o limite).

concurso-de-crimes-e-penas -> arts. citados: CP 29 (caput, §1, §2), 30, 31, 69 (caput, §1, §2), 70 (caput, par. unico), 71 (caput, par. unico), 72, 75 (caput, §1, §2 — **limite lido do anexo: 40 anos, Lei 13.964/2019**), 76; Sumula 443 STJ (✅), Sumula 711 STF (✅), Sumula 715 STF (🟡 conferir).
