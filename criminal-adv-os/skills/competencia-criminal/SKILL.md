---
name: competencia-criminal
description: "Fixa e impugna a competencia no processo penal — lugar da infracao, domicilio do reu, distribuicao, conexao e continencia, prevencao, prorrogacao e foro por prerrogativa. Use quando o operador disser qual juizo competente, foro, conexao, competencia criminal, prerrogativa de funcao, declinar competencia, ou perguntar onde corre o processo."
---

# COMPETENCIA-CRIMINAL

> Camada 2 (gestao processual penal). Confirmar o juizo antes de toda peca — competencia errada = nulidade (CPP 564, I). Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (arts. 69-91 + 108-109) e ler a faixa.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Dizer o juizo competente (ou apontar a incompetencia para declinar/excecionar), com fundamento artigo a artigo, antes de redigir a peca.

## Quando ativar
- Definir onde ajuizar ou para onde corre o feito.
- Suspeita de juizo incompetente (declinar, excecao, nulidade).
- Multiplos crimes/agentes (conexao, continencia, reuniao/separacao).
- Autoridade com foro por prerrogativa de funcao.
- Duvida Justica comum x Federal.

## Metodologia
1. **Lugar da infracao (regra) — CPP 70.** Competencia pelo lugar da consumacao; na tentativa, pelo lugar do ultimo ato de execucao (70, caput). Conferir §§: consumacao fora do pais (§1), resultado (§2), divisa incerta -> prevencao (§3), estelionato CP 171 pelo domicilio da vitima (§4, Lei 14.155/2021). Continuada/permanente em duas jurisdicoes -> prevencao (CPP 71).
2. **Domicilio do reu — CPP 72.** Lugar da infracao desconhecido: regula-se pelo domicilio/residencia do reu (§§1-2). Acao privada: querelante pode preferir o foro do domicilio do reu mesmo conhecido o lugar (CPP 73).
3. **Natureza da infracao — CPP 74.** Pela organizacao judiciaria, salvo competencia privativa do Juri (74 + §1, conferir o rol).
4. **Distribuicao — CPP 75.** Havendo mais de um juiz igualmente competente, a precedencia da distribuicao fixa a competencia.
5. **Conexao e continencia — CPP 76-82.** Conexao (76: intersubjetiva, objetiva/teleologica, probatoria) e continencia (77). Foro prevalente na reuniao (78: Juri atrai; crime mais grave / maior numero / prevencao). Unidade de processo e julgamento (79) e excecoes (79, I-II). Separacao facultativa (80). Reunidos, persiste a competencia mesmo com absolvicao/desclassificacao do crime atrativo (81). Avocacao de processos ja instaurados (82).
6. **Prevencao — CPP 83.** Fixa-se quando, concorrendo juizes igualmente competentes, um antecede os outros na pratica de ato do processo ou medida, ainda que anterior a denuncia/queixa.
7. **Prorrogacao e incompetencia — CPP 108-109.** Excecao de incompetencia (108); reconhecimento de oficio com remessa ao juiz competente (109). CPP 567: a incompetencia anula so os atos decisorios — os instrutorios podem ser ratificados.
8. **Foro por prerrogativa de funcao.** Decorre da CF e das constituicoes estaduais — **descrever a regra e conferir a hipotese concreta na fonte; nunca afirmar foro sem checar**. Justica comum x Federal segue o art. 109 da CF (taxativo — descrever).

## Entrega obrigatoria final
Juizo competente (ou incompetencia apontada) + fundamento CPP artigo a artigo + indicacao da via (ajuizar no foro X / declinar / opor excecao 108 / arguir nulidade 564,I) + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo entra sem `validador-criminal` (cruza `context/cpp-3689-41.md`). Foro por prerrogativa e Justica comum x Federal: **descrever e conferir a hipotese na fonte — nunca afirmar foro de memoria**. Jurisprudencia so se ✅ em `jurisprudencia-criminal.md`. Gate final `suprema-corte-criminal`.

competencia-criminal -> arts. citados: CPP 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 108, 109, 564 (I), 567; CP 171; CF 109.
