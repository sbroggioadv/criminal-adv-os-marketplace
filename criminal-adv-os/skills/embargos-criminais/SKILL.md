---
name: embargos-criminais
description: "Embargos criminais — distingue EMBARGOS DE DECLARACAO (CPP 619-620 / 382) contra ambiguidade, obscuridade, contradicao ou omissao, e EMBARGOS INFRINGENTES E DE NULIDADE (CPP 609 par. unico) cabiveis so quando o acordao NAO for unanime e for desfavoravel ao reu. Use quando o operador disser embargos de declaracao, embargos infringentes, omissao no acordao, acordao nao unanime, ou embargos criminais."
---

# EMBARGOS-CRIMINAIS

> Camada 7 (recursos criminais). Foco DEFESA. Dois embargos distintos com requisitos e prazos OPOSTOS — identificar QUAL antes de redigir.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (619, 620, 382 para ED; 609 para infringentes) e ler a faixa.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Escolher o embargo correto e redigi-lo: ED para sanar vicio do julgado; infringentes para reverter o voto vencido favoravel ao reu.

## Quando ativar
- **ED:** acordao/sentenca com ambiguidade, obscuridade, contradicao ou omissao.
- **Infringentes e de nulidade:** acordao de 2a instancia NAO unanime e desfavoravel ao reu.

## Metodologia
1. **DISTINGUIR os dois embargos ANTES de tudo:**
   - **EMBARGOS DE DECLARACAO (ED):** sanar **ambiguidade, obscuridade, contradicao ou omissao** (vicios formais), NAO rediscutir merito.
   - **EMBARGOS INFRINGENTES E DE NULIDADE:** reverter o resultado quando ha **voto divergente favoravel ao reu** em julgamento NAO unanime.
2. **ED contra ACORDAO — CPP 619-620: prazo 2 dias** da publicacao, deduzido em requerimento que aponte os pontos ambiguo/obscuro/contraditorio/omisso (620). apresentado pelo relator e julgado na 1a sessao, independentemente de revisao (620 §1); se nao preencher as condicoes, indeferimento liminar pelo relator (620 §2).
3. **ED contra SENTENCA de 1o grau — CPP 382: prazo 2 dias** para pedir ao juiz que declare a sentenca (mesmas hipoteses: obscuridade, ambiguidade, contradicao, omissao).
4. **EMBARGOS INFRINGENTES E DE NULIDADE — CPP 609 par. unico:** so cabem quando a decisao de 2a instancia **NAO for unanime** E for **desfavoravel ao reu**; **prazo 10 dias** da publicacao do acordao; **so a parte/materia divergente** (se o desacordo for parcial, restritos a materia objeto da divergencia). Recurso exclusivo da DEFESA.
5. ⚠️ Prazo PROCESSUAL conta pelo CPP 798 §1 (EXCLUI o dia do comeco) — cross-link `prazos-processuais-penais` para a data fatal. Nunca de cabeca. Atentar: ED interrompe/abre prazo para os demais recursos — confirmar no `validador-criminal`.
6. **ED com efeito infringente (excepcional):** quando sanar a omissao/contradicao altera o resultado — fundamentar o vicio E a consequencia. Usar com parcimonia; gate na `suprema-corte-criminal`.
7. **Conteudo (DEFESA):** ED = apontar o vicio ponto a ponto + prequestionamento (se mira REsp/RE). Infringentes = adotar a fundamentacao do voto vencido + atacar a do voto majoritario.

## Entrega obrigatoria final
Identificacao do embargo correto (ED x infringentes) + peca redigida (vicios apontados ou voto vencido adotado) + linha do tempo de tempestividade (CPP 619/382 = 2 dias; 609 = 10 dias, via `prazos-processuais-penais`) + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo/jurisprudencia sem `validador-criminal` (cruza `context/`). NAO confundir os embargos: infringentes exigem acordao NAO unanime + desfavoravel ao reu (CPP 609 par. unico) — fora disso e inadmissivel. ED nao serve para rediscutir merito. Prazo SEMPRE pelo CPP 798 via `prazos-processuais-penais`, nunca de memoria. Jurisprudencia so se ✅. Gate final `suprema-corte-criminal`.

embargos-criminais -> arts. citados: CPP 619, 620 (§§1, 2), 382 (ED 1o grau), 609 par. unico (infringentes e de nulidade, 10 dias); + CPP 798 (via prazos-processuais-penais).
