---
name: base-legal-lep
description: "Porta de fundacao para a LEI DE EXECUCAO PENAL (Lei 7.210/84). Ensina a ler a redacao VIGENTE do art. 112 (progressao reescrita pela Lei 15.402/2026, base 1/6 + excecoes; os 16-70% de 2019 estao TACHADOS) + camada Antifacao 15.358/2026. Use quando o operador disser LEP, execucao penal, progressao de regime, remicao, livramento, saida temporaria, falta grave, ou perguntar percentual de progressao."
---

# BASE-LEGAL-LEP — Porta para a Lei de Execucao Penal

> Camada 1 (fundacao enraizada). Esta skill NAO redige peca — ela aponta e ensina a navegar a lei seca da LEP, para que regime, progressao e beneficios saiam da redacao vigente do arquivo, nunca da memoria de treino (que esta defasada).

## Anexos obrigatorios (context/)
- `context/lep-7210-84.md` — Lei de Execucao Penal consolidada (~159KB). **Localizar o artigo por busca ("Art. N") + ler a faixa**; nunca abrir o arquivo inteiro.

## Objetivo
Entregar a regra de execucao penal exata (regime, progressao, remicao, livramento, saida, falta) na redacao VIGENTE 2026, lida do arquivo, para alimentar o Motor Penal Temporal sem citar percentual revogado.

## Quando ativar
- Pergunta por LEP, execucao penal, progressao de regime, remicao, livramento condicional, saida temporaria, detracao ou faltas.
- Necessidade do percentual de progressao ou de requisito de beneficio.
- Antes de qualquer calculo de execucao (progressao, livramento, remicao).

## Como navegar (regra de uso)
1. **Buscar** `Art. N` no `context/lep-7210-84.md` e ler so a faixa.
2. **Mapa da LEP:** deveres/direitos do preso; **faltas (50-52)**; juiz da execucao (66); regimes e **PROGRESSAO (112)**; **remicao (126-130)**; **livramento (131-146)**; **saida temporaria (122-125)**.
3. **⚠️ DESTAQUE — art. 112 (progressao):** o arquivo tem versoes TACHADAS (`~~`) e a redacao NAO-tachada VIGENTE. **Ler somente a nao-tachada.** A redacao em vigor e da **Lei 15.402/2026** (modelo base **1/6** + excecoes graduadas), combinada com a camada **Antifacao (Lei 15.358/2026)** que elevou as fracoes de hediondos: V=70%, VI=75% (inclui lider de orcrim ultraviolenta VI-b), VII=80%, VIII=85% (reincidente+hediondo+morte). ⚠️ Os percentuais **16-70% de 2019** estao REVOGADOS/tachados — nunca citar.
4. **Nao repetir numero de cabeca:** ler o percentual aplicavel no arquivo a cada caso.

## Entrega obrigatoria final
- Numero do artigo + redacao NAO-tachada aplicavel + o percentual/requisito vigente, transcritos do `context/lep-7210-84.md`, com nota de qual lei deu a redacao (15.402/2026 e/ou 15.358/2026) — pronto para o Motor Penal Temporal calcular.

## Guard
Nenhum percentual, requisito ou regime entra em peca/calculo sem passar pelo `validador-criminal` (cruza o `context/`). Se a redacao parecer ser a de 2019 (16-70%), BLOQUEAR — esta tachada; ler a vigente. Toda entrega fecha pela `suprema-corte-criminal`.
