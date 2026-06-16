---
name: juri-fase-1-pronuncia
description: "Primeira fase do procedimento do juri (judicium accusationis): conduz a defesa da instrucao preliminar ate a decisao de encerramento, mirando IMPRONUNCIA (CPP 414), DESCLASSIFICACAO (CPP 419) ou ABSOLVICAO SUMARIA (CPP 415), e contendo a pronuncia (CPP 413) sem excesso de linguagem. Use quando o operador disser pronuncia, impronuncia, desclassificacao no juri, absolvicao sumaria juri, primeira fase do juri, judicium accusationis."
---

# JURI-FASE-1-PRONUNCIA

> Camada 8 (tribunal do juri). Primeira fase = judicium accusationis: aqui se decide se o reu vai ou nao a plenario. A melhor chance de tirar o reu do juri. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (406-421) e ler a faixa. A numeracao quebra de linha — grepar tambem `^41[3-9]\.`.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Encerrar o processo a favor do reu (impronuncia, desclassificacao ou absolvicao sumaria) ou, ao menos, limitar a pronuncia ao minimo, sem excesso de linguagem que contamine os jurados na segunda fase.

## Quando ativar
- Crime doloso contra a vida (ou conexo) — primeira fase em curso.
- Encerrada a instrucao preliminar, antes da pronuncia/impronuncia.
- Hipotese de impronuncia, desclassificacao ou absolvicao sumaria.
- Pronuncia com excesso de linguagem — preparar impugnacao (cross-link `rese`).

## Metodologia
1. **Procedimento da 1a fase — CPP 406-412.** CPP 406: oferecida a denuncia/queixa, citacao para resposta escrita em **10 (dez) dias**. CPP 407: excecoes em apartado. CPP 408: sem resposta, nomeia-se defensor. CPP 409-411: instrucao preliminar (ofendido, testemunhas, peritos, interrogatorio, debates orais). CPP 412: procedimento concluido em **90 dias** (cross-link `prazos-processuais-penais`).
2. **Conter a PRONUNCIA — CPP 413.** O juiz pronuncia se convencido da **materialidade do fato** e de **indicios suficientes de autoria ou participacao** (juizo de admissibilidade). §1: a fundamentacao **limita-se** a indicar materialidade e indicios — vedado o **excesso de linguagem** (eloquencia acusatoria que invada o merito e contamine os jurados). §2: se o crime for afiancavel, arbitra o valor da fianca para concessao ou manutencao da liberdade provisoria. §3: decide sobre prisao/cautelares. Tese: insuficiencia de indicios + se pronunciar, exigir linguagem contida.
3. **IMPRONUNCIA — CPP 414.** Nao se convencendo da materialidade ou dos indicios suficientes, o juiz **impronuncia**. Paragrafo unico: enquanto nao extinta a punibilidade, cabe **nova denuncia/queixa se houver prova nova**. Tese central quando o lastro probatorio e fraco.
4. **ABSOLVICAO SUMARIA — CPP 415.** Absolve desde logo quando: **I** provada a inexistencia do fato; **II** provado nao ser o reu autor ou participe; **III** o fato nao constituir infracao penal (atipicidade); **IV** demonstrada causa de isencao de pena ou de exclusao do crime (art. 23, 26 CP). Paragrafo unico: **inimputabilidade (CP 26) NAO gera absolvicao sumaria** (leva a medida de seguranca), **salvo quando for a unica tese defensiva**.
5. **DESCLASSIFICACAO — CPP 419.** Convencido o juiz, em discordancia com a acusacao, de **crime diverso** que **nao seja da competencia do juri** e nao sendo ele competente, **remete os autos ao juizo competente**. Tira o reu do juri quando o crime nao e doloso contra a vida (ex.: lesao seguida de morte, latrocinio). Paragrafo unico: reu preso fica a disposicao do juizo destinatario.
6. **Atos correlatos — CPP 416-418, 420-421.** CPP 416: contra impronuncia e absolvicao sumaria cabe **APELACAO** (nao RESE). CPP 417: indicios contra terceiros -> retorno ao MP por 15 dias. CPP 418: definicao juridica diversa (emendatio). CPP 420-421: intimacao da pronuncia e remessa ao presidente do juri.
7. **Recurso da PRONUNCIA = RESE** (CPP 581, IV) — cross-link `rese`. Nao confundir: pronuncia -> RESE; impronuncia/absolvicao sumaria -> apelacao (CPP 416).
8. **Gestao processual transversal.** Passar por `competencia-criminal`, `prazos-processuais-penais` (90 dias/tempestividade), `nulidades-penais` e `estrategia-penal`.

## Entrega obrigatoria final
Peca da fase (resposta + alegacoes/memoriais pedindo impronuncia/desclassificacao/absolvicao sumaria, ou impugnacao da pronuncia) com a tese ancorada no artigo correto (414/415 inciso/419), pedido subsidiario de pronuncia sem excesso de linguagem, indicacao do recurso cabivel (RESE x apelacao) e handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo/jurisprudencia/percentual entra sem `validador-criminal` (cruza `context/cpp-3689-41.md`). Jurisprudencia so se ✅. Nao trocar o recurso: pronuncia = RESE; impronuncia/absolvicao sumaria = apelacao (CPP 416). Inimputabilidade (CP 26) nao gera absolvicao sumaria salvo tese unica (CPP 415 par. unico). Foco DEFESA. Gate final `suprema-corte-criminal`.

juri-fase-1-pronuncia -> arts. citados: CPP 406, 407, 408, 409, 410, 411, 412, 413 (§§1-3), 414 (par. unico), 415 (I-IV + par. unico), 416, 417, 418, 419 (par. unico), 420, 421; CP 23, 26; CPP 581 IV (via rese).
