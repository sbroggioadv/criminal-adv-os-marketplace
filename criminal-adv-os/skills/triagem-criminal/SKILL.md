---
name: triagem-criminal
description: "Classifica a demanda penal e roteia para a skill certa. Identifica a FASE DA PERSECUCAO (investigacao/flagrante, acao penal, instrucao, recursal, execucao penal, incidente, calculo temporal) e o OBJETIVO, e indica a skill alvo + a situacao prisional. Use quando o operador descrever uma situacao penal e nao souber o caminho, ou disser triagem criminal, qual o caminho, que peca eu uso, em que fase estou, /triagem-criminal."
---

# TRIAGEM-CRIMINAL

> Tier 0. Porta de classificacao. Chamada pelo `criminal-master` no inicio de todo caso.

## Anexos obrigatorios (context/)
- `context/metodologia-criminal.md` (mapa de skills + fluxo da persecucao).
- `context/cpp-3689-41.md` (se a duvida for de fase/procedimento) — grep o artigo.

## Objetivo
Em poucas perguntas, dizer: fase da persecucao + objetivo + skill alvo + situacao prisional (solto/preso/flagrante/cautelar).

## Arvore de decisao
1. **Cliente PRESO agora (flagrante/cautelar)?** -> `flagrante-e-audiencia-custodia` (relaxamento CPP 310) e/ou `liberdade-provisoria-e-preventiva` (CPP 311-316); avaliar `habeas-corpus` se constrangimento ilegal.
2. **Fase de INVESTIGACAO (inquerito/PIC)?** -> `investigacao-defensiva` + avaliar trancamento via `habeas-corpus`; se cabivel acordo, `anpp`/`transacao-penal`.
3. **Recebeu DENUNCIA/QUEIXA?** -> `resposta-a-acusacao` (CPP 396-A, mira absolvicao sumaria 397) + gestao processual (competencia/nulidades) + avaliar `anpp`/`suspensao-condicional-processo`.
4. **Em INSTRUCAO / pos-AIJ?** -> `alegacoes-finais-memoriais`; se juri, `juri-fase-1-pronuncia` -> `juri-estrategia-pre-plenario`/`juri-teses-e-quesitos`.
5. **Recebeu SENTENCA/ACORDAO e quer recorrer?** -> escolher: contra pronuncia/decisoes do art. 581 -> `rese`; sentenca -> `apelacao-criminal`; vicio -> `embargos-criminais`; ultima instancia vs lei federal/CF -> `recursos-excepcionais-criminais`; constrangimento -> `habeas-corpus-superiores`; transitado com prova nova/erro -> `revisao-criminal`.
6. **EXECUCAO PENAL?** -> `guia-de-execucao-penal` -> `progressao-de-regime` / `livramento-condicional` / `remicao` / `detracao` / `beneficios-saida-e-cautelares-penais` / `incidentes-execucao-penal`.
7. **Precisa de CALCULO TEMPORAL?** -> `prescricao-penal` / `dosimetria-da-pena` / `motor-calculo-de-pena` / `concurso-de-crimes-e-penas` / `extincao-da-punibilidade`.
8. **Tipo penal especial?** -> `lei-de-drogas` / `crimes-hediondos-e-equiparados` / `organizacao-criminosa-e-colaboracao` / `lavagem-e-financeiros` / `violencia-domestica-e-vulneraveis`.

## Entrega obrigatoria final
- Fase + objetivo + skill alvo + situacao prisional, em 3-5 linhas, e o handoff para o `criminal-master`.

## Guard
Na duvida de competencia/procedimento, consultar `context/cpp-3689-41.md`. Nao redigir peca nem calcular aqui — so classificar e rotear. Lei vigente em context/ (nao memoria de treino).
