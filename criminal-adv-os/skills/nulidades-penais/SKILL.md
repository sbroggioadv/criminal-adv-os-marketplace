---
name: nulidades-penais
description: "Arguir e dimensionar nulidades no processo penal e atacar prova ilicita — pas de nullite sans grief, rol do art. 564, prejuizo, momento de arguicao/preclusao, nulidade absoluta x relativa e frutos da arvore envenenada. Use quando o operador disser nulidade, vicio processual, prova ilicita, cerceamento de defesa, anular o processo."
---

# NULIDADES-PENAIS

> Camada 2 (gestao processual penal). Mapear vicios antes de toda peca de defesa. Sem prejuizo nao ha nulidade — mas a prova ilicita contamina. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (563-573 + 157) e ler a faixa.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Identificar o vicio, classifica-lo (absoluto x relativo), demonstrar o prejuizo e indicar o momento/peca de arguicao — antes de redigir a defesa.

## Quando ativar
- Suspeita de vicio processual (citacao, defesa, competencia, formas do 564).
- Prova obtida em violacao a norma constitucional ou legal.
- Cerceamento de defesa / contraditorio.
- Decidir se o vicio anula e ate onde (extensao).

## Metodologia
1. **Pas de nullite sans grief — CPP 563.** Nenhum ato e nulo se da nulidade nao resultar **prejuizo** para a acusacao ou a defesa. Toda arguicao demonstra prejuizo concreto. Reforco: CPP 566 (nao se anula ato que nao influiu na apuracao da verdade ou na decisao).
2. **Rol exemplificativo — CPP 564.** Incompetencia/suspeicao/suborno do juiz (I), ilegitimidade de parte (II), falta de formulas/termos do III (denuncia/queixa, corpo de delito, nomeacao de defensor, intervencao do MP, citacao/interrogatorio, atos do Juri), omissao de formalidade essencial (IV), **decisao sem fundamentacao** (V, Lei 13.964/2019). Rol nao taxativo.
3. **Quem nao pode arguir — CPP 565.** Parte nao argui nulidade a que deu causa, para que concorreu, ou referente a formalidade que so interesse a parte contraria.
4. **Convalidacao/sanatoria — CPP 567-570, 572.** Incompetencia anula so os atos decisorios (567); ilegitimidade do representante sana por ratificacao (568); omissoes da denuncia/queixa supriveis ate a sentenca (569); falta de citacao/intimacao sana com o comparecimento (570). CPP 572: nulidades relativas sanadas se nao arguidas a tempo, se o ato atingiu o fim, ou se a parte aceitou os efeitos.
5. **Momento de arguicao — CPP 571.** As nulidades devem ser arguidas nos momentos dos incisos I-VIII (instrucao, processo sumario, pos-pronuncia, instancia superior, razoes de recurso, plenario) — **sob pena de preclusao nas relativas**. Identificar o inciso do caso.
6. **Absoluta x relativa.** **Absoluta:** prejuizo presumido, arguivel a qualquer tempo, nao preclui, conhecivel de oficio (incompetencia absoluta, ausencia de defesa, falta de fundamentacao — 564, V). **Relativa:** prejuizo a comprovar, sujeita a preclusao (571) e convalidacao (572). Enquadrar antes da estrategia.
7. **Atos que se renovam — CPP 573.** Os nao sanados sao renovados/retificados; a nulidade declarada contamina os atos dependentes ou consequentes (§1 — cascata) e o juiz declara a extensao (§2).
8. **Prova ilicita — CPP 157.** Inadmissiveis e desentranhadas as provas obtidas em violacao a normas constitucionais ou legais (caput). **§1: frutos da arvore envenenada** — inadmissiveis as derivadas das ilicitas, salvo sem nexo de causalidade ou fonte independente (§2 a define). §3: inutilizacao apos preclusao. **§5: descontaminacao do julgado** — o juiz que conhecer da prova inadmissivel nao podera proferir sentenca/acordao (Lei 13.964/2019; vide ADIs 6.298-6.305).
9. Se o unico elo for **reconhecimento sem o rito do art. 226 do CPP**, somar a tese de nulidade/insuficiencia probatoria do **STJ Tema 1.016** (✅ em `jurisprudencia-criminal.md`).

## Entrega obrigatoria final
Vicio + classificacao (absoluto x relativo) + prejuizo (563) + momento/peca de arguicao (571) + extensao (573) + para prova ilicita: pedido de desentranhamento (157) e, se cabivel, descontaminacao (157 §5) + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo entra sem `validador-criminal` (cruza `context/cpp-3689-41.md`). Sempre demonstrar prejuizo concreto (563) — nulidade relativa sem prejuizo nao prospera. Jurisprudencia (ex.: Tema 1.016) so se ✅ em `jurisprudencia-criminal.md`. Gate final `suprema-corte-criminal`.

nulidades-penais -> arts. citados: CPP 563, 564 (I-V), 565, 566, 567, 568, 569, 570, 571, 572, 573 (§§1-2), 157 (§§1, 2, 3, 5), 226; STJ Tema 1.016 (✅).
