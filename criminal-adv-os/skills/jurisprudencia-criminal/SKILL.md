---
name: jurisprudencia-criminal
description: "Porta de fundacao para a JURISPRUDENCIA criminal (sumulas e temas STF/STJ marcados ✅/🟡/❌). So cita item ✅ confirmado; 🟡 confere ao vivo antes; ❌ nunca. Ensina a achar a tese certa para a defesa. Use quando o operador disser jurisprudencia, sumula, tema repetitivo, tese de defesa, repercussao geral, esse acordao existe, ou pedir precedente para fundamentar peca criminal."
---

# JURISPRUDENCIA-CRIMINAL — Porta para a Jurisprudencia

> Camada 1 (fundacao enraizada). Esta skill NAO redige peca — ela aponta e ensina a buscar a tese certa no arquivo de jurisprudencia, para que nenhuma sumula/tema entre em peca sem estar confirmado.

## Anexos obrigatorios (context/)
- `context/jurisprudencia-criminal.md` — sumulas e temas STF/STJ de uso defensivo recorrente, marcados ✅ confirmado · 🟡 conferir · ❌ superado.

## Objetivo
Entregar a tese de defesa correta (sumula, tema repetitivo, repercussao geral, acordao) com status de vigencia explicito, lida do arquivo, para que a peca cite so o que existe e esta vigente.

## Quando ativar
- Pergunta por jurisprudencia, sumula, tema repetitivo, repercussao geral ou tese de defesa.
- Duvida se um acordao/sumula existe ou esta vigente.
- Antes de inserir qualquer precedente numa peca criminal.

## Como navegar (regra de uso)
1. **Buscar** o numero/tema no `context/jurisprudencia-criminal.md` e ler o teor + status.
2. **Regra de status — inviolavel:**
   - ✅ **so item confirmado pode entrar na peca**;
   - 🟡 **conferir ao vivo (firecrawl/STJ/STF) antes** de citar — nunca citar 🟡 sem reconferencia;
   - ❌ **nunca** citar (superado/cancelado).
3. **Achar a tese para a defesa** — exemplos do arquivo: Sumula 444 STJ + Tema 585 (inqueritos/acoes em curso nao agravam pena); **Tema 1.016 STJ** (reconhecimento fora do art. 226 CPP nao sustenta condenacao sozinho); Sumula Vinculante 56 (sem vaga, nao manter em regime mais gravoso); Tema 506/RE 635.659 (maconha consumo pessoal).
4. **Status pode mudar:** o arquivo traz a verificacao datada — itens 🟡 exigem checagem na fonte oficial no dia do uso.

## Entrega obrigatoria final
- Sumula/tema/acordao + teor sintetico + status (✅/🟡/❌) + uso defensivo, transcritos do `context/jurisprudencia-criminal.md`; se 🟡, indicar a checagem ao vivo necessaria — pronto para a peca citar.

## Guard
Nenhuma sumula/tema/acordao entra em peca sem passar pelo `validador-criminal` e pelo guard global `anti-alucinacao-juridica`. Item 🟡 ou ausente: BLOQUEAR ate confirmar ao vivo. Toda entrega fecha pela `suprema-corte-criminal`.
