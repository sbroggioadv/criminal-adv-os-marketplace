---
name: juri-plenario-sustentacao
description: "Atuacao no plenario do juri: instrucao em plenario (CPP 473-475 — vitima, testemunhas, interrogatorio), DEBATES (CPP 476-481 — acusacao, defesa, replica e treplica; tempo CPP 477 = 1h30 cada + 1h replica/treplica), vedacoes do CPP 478 (nao usar pronuncia, algemas ou silencio como argumento de autoridade), prova nova so com 3 dias uteis (CPP 479) e apartes (CPP 497 XII). Use quando o operador disser plenario, sustentacao oral juri, debates, replica treplica, instrucao em plenario."
---

# JURI-PLENARIO-SUSTENTACAO

> Camada 8 (tribunal do juri). O dia do julgamento: instrucao oral diante dos jurados + debates. A sustentacao defensiva e onde a tese vira conviccao do conselho. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (473-481, 497) e ler a faixa. A numeracao quebra de linha — grepar tambem `^47[3-9]\.`, `^480\.`, `^481\.`, `^497\.`.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Conduzir a instrucao em plenario e os debates para maximizar a tese defensiva diante dos jurados, explorar as vedacoes do CPP 478 contra a acusacao, controlar o tempo (CPP 477) e usar replica/treplica e apartes a favor do reu — sempre alimentando o quesito (cross-link `juri-teses-e-quesitos`).

## Quando ativar
- Sessao de julgamento em plenario designada.
- Preparo da oitiva de vitima/testemunhas e do interrogatorio diante dos jurados.
- Estruturacao da sustentacao oral, replica/treplica e apartes.

## Metodologia
1. **Instrucao em plenario — CPP 473-475.** CPP 473: oitiva do **ofendido** (se possivel) e das **testemunhas** de acusacao e defesa, com perguntas diretas (jurados por intermedio do presidente). CPP 474: **interrogatorio do acusado** em plenario, sustentando sua versao aos jurados. CPP 475: registro/gravacao. Planejar a ordem e o conteudo para sustentar a tese (legitima defesa, negativa de autoria, desclassificacao).
2. **DEBATES — CPP 476.** Encerrada a instrucao, a palavra vai ao **MP** (acusacao nos limites da pronuncia; §3: depois a defesa). §1: assistente apos o MP. §2: na acao privada, primeiro o querelante. §4: cabe **replica** a acusacao e **treplica** a defesa, com reinquiricao de testemunha. A **defesa fala por ultimo** em cada rodada — vantagem a explorar.
3. **TEMPO — CPP 477.** **1h30 para cada parte** na acusacao e na defesa; **1h para a replica e outro tanto para a treplica**. §1: havendo mais de um acusador/defensor, dividem o tempo. §2: havendo **mais de um acusado**, acrescenta-se **1 hora** e dobra-se o tempo de replica/treplica. Controlar a treplica (ultima fala antes da votacao).
4. **⚠️ VEDACOES — CPP 478.** Sob pena de **nulidade**, as partes **nao podem** referir, como **argumento de autoridade** que beneficie ou prejudique o reu: **I** — a **decisao de pronuncia** (e decisoes posteriores) ou ao **uso de algemas**; **II** — ao **silencio do acusado** ou a ausencia de interrogatorio, em seu prejuizo. A defesa **vigia e protesta em ata** quando a acusacao invoca pronuncia/silencio — funda nulidade (cross-link `nulidades-penais`).
5. **Prova nova so com antecedencia — CPP 479.** Vedada a **leitura de documento ou exibicao de objeto** nao juntado com **antecedencia minima de 3 (tres) dias uteis** e ciencia a outra parte (alcanca jornais, videos, fotos, laudos, croqui). Bloquear surpresa probatoria; planejar a propria prova com a antecedencia.
6. **Esclarecimentos e diligencia — CPP 480-481.** CPP 480: partes e jurados podem pedir a folha dos autos; jurados acessam autos/instrumentos do crime se solicitarem. CPP 481: fato essencial nao verificavel de imediato -> **dissolucao do Conselho** e diligencia (pericia com quesitos em 5 dias).
7. **APARTES — CPP 497, XII.** O juiz presidente **regula os apartes**, concedendo a palavra a quem os solicitar. Usar o aparte para corrigir distorcao da acusacao em tempo real, sem perder a linha da sustentacao.
8. **Gestao processual transversal.** Passar por `nulidades-penais` (protesto em ata das violacoes do CPP 478/479), `juri-teses-e-quesitos` e `estrategia-penal` antes de fechar.

## Entrega obrigatoria final
Roteiro de plenario: plano de oitiva (CPP 473-474), estrutura da sustentacao oral defensiva com controle de tempo (CPP 477), checklist de vedacoes a vigiar e protestar em ata (CPP 478-479) e plano de replica/treplica/apartes (CPP 476 §4, 497 XII) — cada bloco amarrado ao quesito. Handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo/jurisprudencia entra sem `validador-criminal` (cruza `context/cpp-3689-41.md`). Jurisprudencia so se ✅. Respeitar os tempos do CPP 477 e as vedacoes do CPP 478 (pronuncia/algemas/silencio = nulidade se usados como argumento de autoridade) — e protestar em ata quando a acusacao violar. Prova nova so com 3 dias uteis (CPP 479). Foco DEFESA. Gate final `suprema-corte-criminal`.

juri-plenario-sustentacao -> arts. citados: CPP 473, 474, 475, 476 (§§1-4), 477 (§§1-2), 478 (I-II), 479 (par. unico), 480 (§§1-3), 481 (par. unico), 497 XII.
