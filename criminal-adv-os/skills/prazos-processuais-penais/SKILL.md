---
name: prazos-processuais-penais
description: "Calcula e controla prazos no processo penal e distingue o prazo PROCESSUAL (CPP 798) do prazo MATERIAL/penal (CP 10), que contam de forma OPOSTA. Use quando o operador disser prazo penal, tempestividade, ate quando recorro, contagem de prazo criminal, prazo do recurso, ou pedir para conferir se um recurso esta no prazo."
---

# PRAZOS-PROCESSUAIS-PENAIS

> Camada 2 (gestao processual penal). Tempestividade antes de toda peca. Errar prazo = recurso nao conhecido. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep o artigo** (798 + cada recurso) e ler a faixa.
- `context/cp-2848-40.md` — art. 10 (prazo material).
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Dar a data fatal correta e o parecer de tempestividade, distinguindo prazo processual de prazo material.

## Quando ativar
- Calcular ate quando recorrer / peticionar.
- Conferir tempestividade de recurso ja interposto.
- Duvida sobre contar (ou nao) o dia do comeco.
- Distinguir recurso (processual) de decadencia/prescricao (material).

## Metodologia
> ⚠️ **DIFERENCIAL CRITICO — os dois prazos contam de forma OPOSTA:**
1. **Prazo PROCESSUAL penal — CPP 798.** Continuos e peremptorios, nao se interrompem por ferias/domingo/feriado (caput). **§1: NAO se computa o dia do comeco, incluindo-se o do vencimento** (exclui o 1o dia — como o CPC). **§3: termino em domingo/feriado prorroga ate o dia util imediato.** §4: nao correm por impedimento do juiz, forca maior ou obstaculo da parte contraria. **§5: termo inicial** — da intimacao, da audiencia/sessao se presente, ou da ciencia inequivoca nos autos. Recesso: CPP 798-A suspende entre 20/12 e 20/01 (salvo reu preso, Maria da Penha, urgencias — Lei 14.365/2022).
2. **Prazo MATERIAL/penal — CP 10.** **O dia do comeco INCLUI-SE no computo** (conta o 1o dia); dias/meses/anos pelo calendario comum. Aplica-se a **decadencia** (queixa/representacao — em regra 6 meses, conferir CP 103) e a **prescricao** (CP 109-117). Nao ha prorrogacao por feriado — e direito material.
3. **Identificar a natureza ANTES de contar:** recurso, manifestacao, resposta = processual (CPP 798); decadencia e prescricao = material (CP 10). Misturar inverte o resultado.
4. **Prazos recursais — conferir CADA UM na faixa do CPP:** RESE = 5 dias (586). Apelacao = 5 dias p/ interpor (593) + 8 dias p/ razoes (600; 3 em contravencao). Embargos de declaracao = 2 dias (619; e 382 no 1o grau). Carta testemunhavel (639-640) — conferir o prazo na faixa. REsp/RE = 15 dias (lei processual civil subsidiaria — conferir, nao afirmar sem checar).
5. **Agravo em execucao** = 5 dias por construcao jurisprudencial (Sumula 700 STF). ⚠️ **Sumula 700 NAO esta marcada ✅ em `jurisprudencia-criminal.md`** — tratar como 🟡: descrever e **conferir teor/numeracao no validador antes de citar**.
6. **Calcular com a lei seca aberta:** termo inicial (798 §5) -> excluir o 1o dia (798 §1) -> contar dias corridos (sao continuos, caput) -> prorrogacao por feriado/domingo no vencimento (798 §3) -> recesso (798-A). Entregar **linha do tempo + data fatal + fundamento + parecer**.

## Entrega obrigatoria final
Linha do tempo (termo inicial -> contagem -> data fatal) + natureza do prazo (processual x material) + fundamento (CPP 798 §§ ou CP 10) + parecer de tempestividade + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhuma data sai sem `validador-criminal` (cruza `context/`). Conferir o prazo de CADA recurso na faixa do CPP — nunca de memoria. Sumula 700 STF = 🟡 (conferir antes de citar). Jurisprudencia so se ✅. Na duvida de natureza/contagem, bloquear e reler a lei seca. Gate final `suprema-corte-criminal`.

prazos-processuais-penais -> arts. citados: CPP 798 (§§1, 3, 4, 5), 798-A, 586, 593, 600, 619, 382, 639, 640; CP 10, 103, 109-117; Sumula 700 STF (🟡).
