---
name: suspensao-condicional-processo
description: "Pleiteia a suspensao condicional do processo / sursis processual (Lei 9.099/1995 art. 89) quando a pena minima for ate 1 ano: suspende o processo por periodo de prova com condicoes, ate a extincao da punibilidade, sempre conferindo o teor da lei. Use quando o operador disser suspensao condicional do processo, sursis processual, art. 89, suspender o processo, ou periodo de prova."
---

# SUSPENSAO-CONDICIONAL-PROCESSO

> Camada 5 (acordos & despenalizacao). Sursis PROCESSUAL — suspende o processo (ja com denuncia) por periodo de prova; cumprido, extingue a punibilidade SEM condenacao. Foco DEFESA. NAO confundir com sursis PENAL (suspende a pena ja aplicada — `sursis-penal`).

## Anexos obrigatorios (context/)
- `context/jurisprudencia-criminal.md` — so citar item ✅; o que nao constar = 🟡.
- ⚠️ **A Lei 9.099/1995 NAO esta na lei seca local (CP/CPP/LEP).** Teor do art. 89 e das sumulas (723 STF, 337 STJ) deve ser **confirmado ao vivo no `validador-criminal`** antes de citar numero/redacao — anti-alucinacao.

## Objetivo
Verificar se o caso comporta sursis processual, conseguir a suspensao na proposta menos onerosa e conduzir ate a extincao da punibilidade ao fim do periodo de prova sem revogacao — evitando a condenacao.

## Quando ativar
- Ja ha **denuncia** e a **pena minima** cominada e **igual ou inferior a 1 ano**.
- "Da pra suspender o processo?" / "periodo de prova"; ou conferir proposta ja oferecida (condicoes/prazo).
- Distinguir do sursis penal (`sursis-penal`), da transacao (`transacao-penal`) e do ANPP (`anpp`).

## Metodologia (ARTIGOS REAIS — conferir no validador, lei nao esta em context/)
1. **Cabimento (Lei 9.099/1995 art. 89 caput):** cabe quando a **pena minima cominada for igual ou inferior a 1 ano**, abrangidos ou nao pela Lei 9.099 (aplica-se alem do JECrim). Proposta do MP **ao oferecer a denuncia**; periodo de prova de **2 a 4 anos**. Confirmar o teor do art. 89 no `validador-criminal`. Requisitos pessoais: nao estar sendo processado/condenado por outro crime + requisitos do art. 77 do CP (conferir).
2. **Condicoes (art. 89 §1):** I reparar o dano (salvo impossibilidade); II proibicao de frequentar determinados lugares; III proibicao de ausentar-se da comarca sem autorizacao do juiz; IV comparecimento pessoal e obrigatorio a juizo, mensalmente, para informar e justificar atividades. O juiz pode especificar outras condicoes adequadas (conferir §2).
3. **Revogacao OBRIGATORIA (art. 89 §3):** o beneficio e revogado se, no curso do prazo, o acusado **vier a ser processado por outro crime** ou **nao efetuar, sem motivo justificado, a reparacao do dano**.
4. **Revogacao FACULTATIVA (art. 89 §4):** pode ser revogado se o acusado vier a ser processado por **contravencao** ou **descumprir qualquer outra condicao** imposta.
5. **Extincao da punibilidade (art. 89 §5):** expirado o prazo **sem revogacao**, o juiz declara **extinta a punibilidade** — rotear `extincao-da-punibilidade` para registrar o efeito. Nao gera condenacao nem reincidencia.
6. **Sumulas (🟡 — conferir antes de citar):** **Sumula 723 do STF** (sobre o cabimento em relacao ao concurso de crimes / soma das penas minimas) e **Sumula 337 do STJ** (suspensao quando a desclassificacao/procedencia parcial reduz a pena minima ao patamar legal). Ambas **NAO constam em `context/`** — tratar como 🟡 e **confirmar teor/numeracao no `validador-criminal`** antes de usar em peca.

## Entrega obrigatoria final
Parecer de cabimento (pena minima ≤ 1 ano + requisitos) + proposta de condicoes do §1 na forma menos onerosa + cronograma do periodo de prova (2 a 4 anos) + alerta sobre revogacao obrigatoria/facultativa + minuta da manifestacao + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Lei 9.099/1995 e sumulas NAO estao em context/ — **nenhum numero/teor de artigo ou sumula sai sem confirmacao ao vivo no `validador-criminal`**. Sumula 723 STF e 337 STJ = 🟡 (conferir antes de citar). NAO confundir com sursis penal (CP 77-82 = `sursis-penal`). Jurisprudencia so se ✅. Na duvida, bloquear e checar. Gate final `suprema-corte-criminal`.

suspensao-condicional-processo -> arts. citados: Lei 9.099/1995 art. 89 (caput; §§ 1 [I-IV], 2, 3, 4, 5) — teor confirmado no validador-criminal (lei fora de context/); CP 77 (requisitos, cross); Sumula 723 STF (🟡), Sumula 337 STJ (🟡).
