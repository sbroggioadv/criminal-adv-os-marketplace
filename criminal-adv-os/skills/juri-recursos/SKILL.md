---
name: juri-recursos
description: "Recursos contra as decisoes do Tribunal do Juri: APELACAO do CPP 593, III (alineas a nulidade posterior a pronuncia; b sentenca contraria a lei/decisao dos jurados; c erro/injustica na pena; d decisao MANIFESTAMENTE CONTRARIA A PROVA DOS AUTOS), com devolutividade RESTRITA a alinea, novo juri so na alinea d (CPP 593 §3) e SOBERANIA DOS VEREDICTOS (CF 5 XXXVIII c). Trata tambem a execucao provisoria da pena >=15 anos (CPP 492 I e + Tema 1.068). Use quando o operador disser recurso do juri, apelacao do juri, manifestamente contraria a prova, soberania dos veredictos, novo juri."
---

# JURI-RECURSOS

> Camada 8 (tribunal do juri). Recorrer da decisao do conselho tem regras proprias: devolutividade restrita as alineas do CPP 593 III e limite de UM novo juri pela alinea d. A soberania dos veredictos comanda tudo. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (593, 492) e ler a faixa. A numeracao quebra de linha — grepar tambem `^492\.`. CPP 593 esta indexado.
- `context/jurisprudencia-criminal.md` — so citar item ✅ (Tema 1.068 esta confirmado).

## Objetivo
Fundamentar o recurso contra a decisao do juri na **alinea exata** do CPP 593 III, respeitando a soberania dos veredictos (devolutividade restrita), e enfrentar a execucao provisoria da pena >=15 anos com os instrumentos certos.

## Quando ativar
- Sentenca condenatoria (ou absolutoria, no caso da acusacao/assistente) apos o veredicto.
- Nulidade posterior a pronuncia, erro de lei do juiz-presidente, injustica na pena ou veredicto manifestamente contrario a prova.
- Execucao provisoria da pena (>=15 anos) determinada na propria sentenca (CPP 492 I "e").

## Metodologia
1. **APELACAO do juri — CPP 593, III (devolutividade RESTRITA).** O tribunal so revisa o alegado na alinea:
   - **a)** **nulidade posterior a pronuncia** (quesitacao defeituosa, violacao do CPP 478 etc. — cross-link `nulidades-penais`, `juri-teses-e-quesitos`, `juri-plenario-sustentacao`);
   - **b)** **sentenca do juiz-presidente contraria a lei expressa ou a decisao dos jurados** (o ad quem **retifica** — CPP 593 §1);
   - **c)** **erro ou injustica na aplicacao da pena/medida de seguranca** (o ad quem **retifica a pena** — CPP 593 §2; cross-link `dosimetria-da-pena`, `motor-calculo-de-pena`);
   - **d)** **decisao dos jurados MANIFESTAMENTE CONTRARIA A PROVA DOS AUTOS** (provido = **NOVO julgamento pelo juri**, nao reforma direta).
2. **⚠️ Alinea "d" = NOVO JURI e UMA so vez — CPP 593 §3.** Provido o recurso, os autos vao a **novo julgamento**; **nao se admite segunda apelacao pelo mesmo motivo**. Reservar a alinea "d" ao veredicto sem qualquer apoio na prova. Decisao apenas **contra** a tese, mas com **algum** lastro probatorio, **nao** e "manifestamente contraria".
3. **SOBERANIA DOS VEREDICTOS — CF 5, XXXVIII, "c".** Fundamento que **limita** o alcance da apelacao do juri: o tribunal nao substitui o jurado no merito (so anula e devolve na alinea "d"). A mesma soberania embasa a execucao imediata >=15 anos. Sustentar a soberania quando ela **beneficia** a defesa (ex.: absolvicao por clemencia do 3o quesito — cross-link `juri-teses-e-quesitos`).
4. **⚠️ EXECUCAO PROVISORIA da pena >=15 anos — CPP 492, I, "e" + Tema 1.068 ✅.** Na condenacao a **pena igual ou superior a 15 anos de reclusao**, o presidente **determina a execucao provisoria** com mandado de prisao, **sem prejuizo dos recursos** (CPP 492 I "e", Lei 13.964/2019). O **STF confirmou a constitucionalidade** no **Tema 1.068 / RE 1.235.340** (soberania dos veredictos), respeitado o patamar de 15 anos — **vigente em 2026, sem superacao** (`jurisprudencia-criminal.md`, bloco D.2 ✅). **Defesa:** (a) **CPP 492 §3** — o presidente pode, **excepcionalmente, deixar de autorizar** a execucao se houver **questao substancial** que possa plausivelmente levar a revisao da condenacao; (b) **CPP 492 §4** — a apelacao >=15 anos **nao tem efeito suspensivo** quanto a execucao; (c) **CPP 492 §5** — excepcionalmente, o tribunal pode **atribuir efeito suspensivo** quando verificado **cumulativamente** que o recurso nao e meramente protelatorio **e** levanta questao substancial que pode resultar em absolvicao, anulacao, novo julgamento ou reducao da pena para abaixo de 15 anos. ⚠️ **Nao estender** a execucao provisoria do juri abaixo de 15 anos nem ao procedimento comum — fora dai vale a regra geral (sem execucao provisoria — ADC 43/44/54 ✅).
5. **Tempestividade.** Interposicao em **5 dias** (CPP 593) + razoes (CPP 600). ⚠️ Prazo PROCESSUAL pelo CPP 798 §1 (exclui o dia do comeco) — cross-link `prazos-processuais-penais`, nunca de cabeca. Mecanica geral via `apelacao-criminal`.
6. **Gestao processual transversal.** Passar por `nulidades-penais` (alinea "a"), `dosimetria-da-pena`/`motor-calculo-de-pena` (alinea "c"), `prazos-processuais-penais` e `estrategia-penal` antes de fechar.

## Entrega obrigatoria final
Recurso ancorado na **alinea exata** do CPP 593 III (com pedido conforme: retificacao em a/b/c; novo juri em d), enfrentamento da execucao provisoria quando >=15 anos (CPP 492 I "e" + §§3-5 + Tema 1.068 ✅) e linha do tempo de tempestividade (CPP 593/600 via `prazos-processuais-penais`). Handoff ao `criminal-master`. Passa pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo/jurisprudencia/percentual/calculo entra sem `validador-criminal` (cruza `context/`). NAO ultrapassar a devolutividade da alinea do CPP 593 III (soberania dos veredictos). Alinea "d" = novo juri e so uma vez (CPP 593 §3). Execucao provisoria so >=15 anos no juri (CPP 492 I "e" + Tema 1.068 ✅) — nao estender; usar §3 (excecao ao autorizar), §4 (sem efeito suspensivo) e §5 (efeito suspensivo excepcional cumulativo) na defesa. Prazo sempre pelo CPP 798 via `prazos-processuais-penais`. Jurisprudencia so se ✅. Foco DEFESA. Gate final `suprema-corte-criminal`.

juri-recursos -> arts. citados: CPP 593 (III a/b/c/d, §§1, 2, 3), 600; CPP 492 (I "e", §§3, 4, 5, 6); CF 5 XXXVIII "c"; STF Tema 1.068 / RE 1.235.340 (✅); ADC 43/44/54 (✅); + CPP 798 (via prazos-processuais-penais).
