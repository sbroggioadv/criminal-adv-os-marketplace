---
name: extincao-da-punibilidade
description: "Consolidador das causas de extincao da punibilidade (rol do art. 107 do CP): identifica a causa, diz onde se confirma e o efeito, e roteia para prescricao-penal ou decadencia-perempcao conforme o caso — sempre com fundamento, nunca de cabeca. Use quando o operador disser extincao da punibilidade, extinguir a pena, abolitio criminis, anistia, graca, indulto ou morte do agente."
---

# EXTINCAO-DA-PUNIBILIDADE

> Camada 3 (motor penal temporal — consolidador). Reune o rol do art. 107 do CP, identifica a causa, fundamenta e roteia. TODO marco vem de `grep` na lei seca. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep** art. 107 (rol I-VI, IX) + 108 (nao se estende a crime pressuposto/conexo) + 120 (perdao judicial). Para prescricao: 109-119. Para decadencia/perempcao/renuncia/perdao: 103-106. O numero pode quebrar de linha — ler a faixa.
- `context/penal-especial.md` + `base-legal-penal-especial` — abolitio criminis e anistia/graca/indulto em legislacao especial.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Dar a porta de entrada do tema: identificar QUAL causa do art. 107 incide, dizer onde ela se confirma na lei seca e o efeito (extingue tudo? so a pena?), e rotear a skill especializada quando o caso exige calculo temporal.

## Quando ativar
- "Da pra extinguir a punibilidade?" / "isso ainda e crime?" / "extinguir a pena".
- Abolitio criminis / lei posterior mais benefica que descriminaliza.
- Anistia, graca ou indulto; morte do agente; retratacao.
- Quando o operador nao sabe QUAL causa alegar (este consolidador classifica e roteia).

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Ler o ROL do art. 107 (grep e conferir os incisos — VII e VIII estao REVOGADOS pela Lei 11.106/2005):**
   - **I — morte do agente:** confirma-se pela **certidao de obito** (CPP 62 exige a certidao + oitiva do MP). Efeito: extingue tudo, personalissima.
   - **II — anistia, graca ou indulto:** anistia por **lei** (apaga o crime); graca (individual) e indulto (coletivo) por **decreto** presidencial. Conferir o ato concreto e o crime alcancado. Efeito: anistia extingue a punibilidade ampla; graca/indulto extinguem **a pena** (executoria), nao o crime.
   - **III — abolitio criminis (retroatividade de lei que nao mais considera o fato criminoso):** confirmar a revogacao do tipo na lei seca / `base-legal-penal-especial`. Efeito: extingue tudo e cessa os efeitos penais da condenacao.
   - **IV — prescricao, decadencia ou perempcao:** **ROTEAR** — prescricao -> `prescricao-penal`; decadencia/perempcao -> `decadencia-perempcao`. Nao calcular aqui.
   - **V — renuncia do direito de queixa ou perdao aceito (acao privada):** **ROTEAR** -> `decadencia-perempcao` (CP 104-106).
   - **VI — retratacao do agente, nos casos em que a lei a admite:** so nos tipos que a preveem (ex.: crimes contra a honra/falso testemunho — conferir o tipo). Efeito: extingue.
   - **IX — perdao judicial, nos casos previstos em lei (CP 120):** concedido pelo juiz na sentenca nas hipoteses legais; **nao gera reincidencia** (CP 120).
2. **Aplicar o art. 108 (limite do alcance):** a extincao da punibilidade de crime que e **pressuposto, elemento constitutivo ou agravante de outro NAO se estende a este**; em crimes conexos, a extincao de um nao impede a agravacao pela conexao. Verificar sempre antes de afirmar "extingue tudo".
3. **Efeito — distinguir o que se extingue:** extingue a **punibilidade inteira** (morte, anistia, abolitio, prescricao da pretensao punitiva, decadencia, perempcao, renuncia, perdao aceito, retratacao, perdao judicial) X extingue **so a pena/execucao** mantendo efeitos penais secundarios (graca, indulto, prescricao da pretensao EXECUTORIA — reincidencia e maus antecedentes podem subsistir). Dizer expressamente qual.
4. **Concurso de crimes:** a extincao incide sobre a pena de **cada crime isoladamente** (CP 119) — checar quando ha mais de um delito.
5. **Confirmar vigencia/existencia da causa** (lei de anistia, decreto de indulto, revogacao do tipo) na lei seca / `base-legal-penal-especial` antes de afirmar — anti-alucinacao.

## Saida obrigatoria
1. **Linha do tempo** dos marcos relevantes da causa identificada (obito · publicacao da lei/decreto · revogacao do tipo · marcos de prescricao se roteado).
2. **Marcos** classificados conforme a causa.
3. **Calculo/verificacao fundamentado** — causa do art. 107 identificada (inciso), **onde se confirma** (artigo + ato concreto: certidao, lei, decreto, revogacao) e o **efeito** (extingue tudo X so a pena), com o art. 108 checado.
4. **Parecer conclusivo** + roteamento explicito (`prescricao-penal` / `decadencia-perempcao`) quando o caso exigir calculo temporal.
5. Handoff ao `criminal-master`; passa pela `suprema-corte-criminal`.

## Guard
Nenhuma causa/efeito sai sem `validador-criminal` (cruza `context/`) — incisos do art. 107, a revogacao de VII/VIII e o alcance do art. 108 vem de `grep` no CP, nunca de memoria. Existencia de lei de anistia/decreto de indulto/revogacao do tipo: confirmar no anexo antes de citar. Jurisprudencia so se ✅. Calculo de prazo NAO se faz aqui — rotear. Na duvida, bloquear e reler a lei seca. Gate final `suprema-corte-criminal`.

extincao-da-punibilidade -> arts. citados: CP 107 (I-VI, IX; VII e VIII revogados pela Lei 11.106/2005), 108, 119, 120; CPP 62; roteia CP 103-106 e 109-119.
