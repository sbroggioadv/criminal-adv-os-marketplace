---
name: apelacao-criminal
description: "Apelacao criminal (CPP 593) — recurso contra sentenca definitiva de condenacao/absolvicao do juiz singular e contra as decisoes do Tribunal do Juri (so nas hipoteses tipicas a-d). Use quando o operador disser apelacao, apelacao criminal, recorrer da sentenca, apelacao do juri, recorri da condenacao, ou 593."
---

# APELACAO-CRIMINAL

> Camada 7 (recursos criminais). Foco DEFESA. Recurso amplo contra sentenca de 1o grau (ampla devolutividade) — salvo a do juri, que tem devolutividade RESTRITA as alineas do 593 III.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (593 + 600) e ler a faixa. Confirmar a hipotese de cabimento e, no juri, a alinea exata.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Interpor apelacao tempestiva, escolher a via correta (sentenca singular x juri) e redigir razoes com a devolutividade adequada (ampla no singular, restrita as alineas no juri).

## Quando ativar
- Sentenca **definitiva de condenacao ou absolvicao** do juiz singular (CPP 593, I).
- Decisao definitiva ou com forca de definitiva nao prevista no capitulo do RESE (CPP 593, II).
- Decisao do **Tribunal do Juri** (CPP 593, III), so nas hipoteses a-d.

## Metodologia
1. **Confirmar o cabimento (CPP 593).** I = sentenca definitiva de condenacao/absolvicao do juiz singular; II = decisao definitiva ou com forca de definitiva; III = decisao do juri. ⚠️ Onde cabe apelacao, NAO usar RESE, ainda que so de parte da decisao (CPP 593 §4).
2. **Tempestividade — CPP 593: 5 dias para interpor + CPP 600: 8 dias para razoes** (3 dias em contravencao). ⚠️ Prazo PROCESSUAL conta pelo CPP 798 §1 (EXCLUI o dia do comeco) — cross-link `prazos-processuais-penais` para a data fatal. Nunca de cabeca.
3. **⚠️ APELACAO DO JURI = devolutividade RESTRITA as alineas do CPP 593 III** — o tribunal so revisa o que foi alegado:
   - **a)** nulidade posterior a pronuncia;
   - **b)** sentenca do juiz-presidente contraria a lei expressa ou a decisao dos jurados (ad quem retifica — 593 §1);
   - **c)** erro ou injustica na aplicacao da pena/medida de seguranca (ad quem retifica a pena — 593 §2);
   - **d)** decisao dos jurados manifestamente contraria a prova dos autos (provido = NOVO julgamento; **nao se admite segunda apelacao pelo mesmo motivo** — 593 §3, limite a um julgamento).
   Fundamentar na alinea correta define o pedido: retificacao (a/b/c) x novo juri (d).
4. **Sentenca do juiz singular = devolutividade AMPLA** (tantum devolutum): atacar nulidades (cross-link `nulidades-penais`), absolvicao (CPP 386), tipicidade/lei vigente, e dosimetria (cross-link `dosimetria-da-pena` + `motor-calculo-de-pena`).
5. **Efeito.** Em regra suspensivo da execucao da pena enquanto nao transita; conferir prisao/excecoes no caso concreto.
6. **Estrutura das razoes (DEFESA):** preliminares (nulidades) -> merito (absolvicao/desclassificacao/atipicidade) -> subsidiario (dosimetria/regime/substituicao). No juri, ancorar cada topico na alinea do 593 III.

## Entrega obrigatoria final
Peticao de interposicao + razoes (devolutividade ampla no singular; alinea a-d no juri) + linha do tempo de tempestividade (CPP 593/600 via `prazos-processuais-penais`) + pedido conforme a hipotese (reforma/absolvicao/retificacao/novo juri) + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo/jurisprudencia/percentual/calculo sem `validador-criminal` (cruza `context/`). No juri, NAO ultrapassar a devolutividade da alinea do 593 III (recurso so devolve o alegado). Prazo SEMPRE pelo CPP 798 via `prazos-processuais-penais`, nunca de memoria. Jurisprudencia so se ✅. Gate final `suprema-corte-criminal`.

apelacao-criminal -> arts. citados: CPP 593 (I, II, III a/b/c/d, §§1, 2, 3, 4), 600 (caput, contravencao 3 dias), 386; + CPP 798 (via prazos-processuais-penais).
