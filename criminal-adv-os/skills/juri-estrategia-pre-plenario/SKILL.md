---
name: juri-estrategia-pre-plenario
description: "Preparacao e estrategia da segunda fase do juri ANTES do plenario: requerimento de provas e rol de ate 5 testemunhas (CPP 422), diligencias e relatorio (CPP 423-424), DESAFORAMENTO como tese (CPP 427-428), alistamento e sorteio dos jurados (CPP 425-426, 432-435) e planejamento das recusas peremptorias (CPP 468 — 3 sem motivar por parte). Use quando o operador disser preparacao do plenario, desaforamento, estrategia do juri, recusa de jurados, antes do plenario."
---

# JURI-ESTRATEGIA-PRE-PLENARIO

> Camada 8 (tribunal do juri). Entre a preclusao da pronuncia e o plenario: aqui se desenha o julgamento — testemunhas, provas, perfil do conselho e a hipotese de desaforamento. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (422-435, 468) e ler a faixa. A numeracao quebra de linha — grepar tambem `^42[2-9]\.` e `^43[0-5]\.`.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Chegar ao plenario com a melhor configuracao para a defesa: provas e testemunhas certas, recusas planejadas e, quando cabivel, deslocar o julgamento (desaforamento) para afastar parcialidade do juri local, pressao da ordem publica ou risco a seguranca do reu.

## Quando ativar
- Pronuncia preclusa (ou recurso resolvido) — autos no presidente do juri.
- Prazo para arrolar testemunhas de plenario e requerer diligencias.
- Suspeita de parcialidade do conselho, comocao social ou risco a seguranca do reu (desaforamento).
- Planejamento das recusas peremptorias para o sorteio.

## Metodologia
1. **Rol de testemunhas e provas — CPP 422.** Recebidos os autos, o presidente intima MP/querelante e defensor para, em **5 (cinco) dias**, apresentarem **rol de testemunhas de plenario, ate o maximo de 5 (cinco)**, juntar documentos e requerer diligencia. Escolha estrategica: testemunha que humaniza o reu, reforca a tese (legitima defesa, negativa de autoria) ou neutraliza a acusacao. Quem nao arrola, perde — preclusao.
2. **Diligencias e relatorio — CPP 423-424.** CPP 423: o presidente ordena diligencias para sanar nulidade ou esclarecer fato (I) e faz **relatorio sucinto**, incluindo em pauta (II). CPP 424: preparo quando a organizacao judiciaria separa o juizo de preparo do presidente do juri. Nada de prova nova no dia sem antecedencia (cross-link `juri-plenario-sustentacao` — CPP 479, 3 dias uteis).
3. **DESAFORAMENTO — CPP 427.** O **Tribunal** (2o grau), a requerimento do MP, assistente, querelante ou **acusado** (ou representacao do juiz), pode **desaforar** para outra comarca da mesma regiao quando: **interesse da ordem publica** o reclamar, houver **duvida sobre a imparcialidade do juri** ou risco a **seguranca pessoal do acusado**. §1: distribuicao imediata, preferencia. §2: motivos relevantes -> relator pode suspender o julgamento. §3: ouve-se o presidente. §4: **nao cabe** na pendencia de recurso contra a pronuncia nem apos efetivado o julgamento (salvo fato em julgamento anulado).
4. **DESAFORAMENTO por excesso de servico — CPP 428.** Tambem cabe quando, comprovado **excesso de servico**, o julgamento nao ocorrer em **6 (seis) meses** do transito da pronuncia (ouvidos presidente e parte contraria). §1: nao se computa adiamento/diligencia de interesse da defesa. §2: sem excesso, o acusado pode requerer realizacao imediata.
5. **Alistamento e sorteio — CPP 425-426, 432-435.** CPP 425-426: lista geral de jurados (alistamento anual). CPP 432-435: organizacao da pauta, sorteio dos jurados da reuniao e do conselho. Mapear o perfil do corpo de jurados quando ha acesso a lista — base da estrategia de recusa.
6. **Recusas peremptorias (planejamento) — CPP 468.** No sorteio, a **defesa recusa primeiro** e, depois, o MP — **ate 3 (tres) cada, sem motivar**. Alem dessas, cabem recusas motivadas (impedimento/suspeicao). Planejar perfil a evitar (vinculo com vitima, vies) — execucao no plenario (cross-link `juri-plenario-sustentacao`).
7. **Gestao processual transversal.** Passar por `competencia-criminal`, `prazos-processuais-penais` (5 dias do rol; 6 meses do 428) e `estrategia-penal` antes de fechar.

## Entrega obrigatoria final
Plano pre-plenario com: requerimento de provas + rol de ate 5 testemunhas (CPP 422), mapa de diligencias, parecer de cabimento de desaforamento (CPP 427 ou 428, hipotese exata) com peca ao Tribunal se for o caso, e roteiro de recusas peremptorias (CPP 468). Handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo/jurisprudencia entra sem `validador-criminal` (cruza `context/cpp-3689-41.md`). Jurisprudencia so se ✅. Desaforamento e competencia do **Tribunal**, com hipotese tipica do CPP 427/428 — nao requerer fora das hipoteses nem na pendencia de recurso da pronuncia (CPP 427 §4). Rol limitado a 5 testemunhas (CPP 422) e recusas peremptorias limitadas a 3 (CPP 468). Foco DEFESA. Gate final `suprema-corte-criminal`.

juri-estrategia-pre-plenario -> arts. citados: CPP 422, 423 (I-II), 424, 425, 426, 427 (§§1-4), 428 (§§1-2), 432, 433, 434, 435, 468 (par. unico).
