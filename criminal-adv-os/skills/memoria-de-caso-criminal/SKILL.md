---
name: memoria-de-caso-criminal
description: "Mantem o estado do caso penal ativo: reu, vitima, MP/querelante, tipo penal, fase da persecucao, numero do processo, situacao prisional, prazos (recursais e de execucao), atos praticados e proxima providencia. Use para abrir/atualizar um caso, retomar de onde parou, ou quando o operador disser memoria de caso, estado do caso, retomar caso, /status-criminal."
---

# MEMORIA-DE-CASO-CRIMINAL

> Tier 0. Estado vivo do caso. Lido no inicio e atualizado no fim de cada tarefa pelo `criminal-master`.

## Anexos obrigatorios (context/)
- Nenhum direto (e estado). Usa os demais anexos via as skills que aciona.

## Objetivo
Nunca perder o fio: quem e quem, em que fase, preso ou solto, que prazos correm, o que ja foi feito e o que vem.

## Estrutura do caso (gravar em `criminal/casos/<slug>.md`, fora do plugin)
1. **Partes:** reu/investigado (qualificacao), vitima, MP/querelante, assistente; advogado.
2. **Imputacao:** tipo(s) penal(is) e dispositivo, data do fato, regime/pena em tese.
3. **Fase da persecucao:** investigacao / acao / instrucao / recursal / execucao.
4. **Processo:** numero, vara/tribunal, comarca/secao.
5. **Situacao prisional:** solto / preso (flagrante, preventiva, definitiva), data da prisao (para detracao/prescricao), regime atual.
6. **Prazos:** recursais (em curso) e de execucao (data-base, fracoes para progressao/livramento) — sempre conferidos pela skill respectiva.
7. **Atos praticados** (append-only) + **proxima providencia** + **proximo prazo fatal**.

## Metodologia
1. Ao abrir: coletar os 7 blocos (perguntar o que faltar).
2. Ao atualizar: registrar o ato praticado (append), recalcular o proximo prazo, atualizar a situacao prisional.
3. Resumir em 5-8 linhas quando o `criminal-master` ou `/status-criminal` pedir.

## Entrega obrigatoria final
- Ficha do caso atualizada + resumo executivo (partes, fase, situacao prisional, proximo passo, proximo prazo).

## Guard
Dados do caso sao sensiveis (LGPD + sigilo). Gravar em `criminal/casos/<slug>.md` no diretorio de trabalho, NUNCA no plugin distribuido. Nao inventar prazo/situacao — o que nao souber, perguntar.
