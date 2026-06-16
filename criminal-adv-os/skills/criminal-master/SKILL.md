---
name: criminal-master
description: "Orquestrador do plugin criminal (Criminal Defense & Procedure Master) e porta unica da defesa penal. Recebe qualquer demanda em linguagem natural, identifica a fase da persecucao e o objetivo, e DIRIME (seleciona e conduz) TODAS as skills pertinentes sem esquecer nenhuma, fechando pela suprema-corte-criminal. Use quando o operador descrever uma tarefa penal sem chamar skill especifica, ou disser criminal-master, novo caso criminal, fui preso, cliente em flagrante, recebi denuncia, calcular pena, prescricao, dosimetria, progressao, habeas corpus, recurso, juri, execucao penal."
---

# CRIMINAL-MASTER — Orquestrador (Criminal Defense & Procedure Master)

> Tier 0. Porta unica do plugin criminal-adv-os. Dirige TODAS as skills necessarias por tarefa, sem esquecer nenhuma. Foco: DEFESA.

## Anexos obrigatorios (context/)
- `context/metodologia-criminal.md` (mapa de uso, fluxo da persecucao, regras de ouro) — **ler primeiro, sempre**.
- Demais anexos sob demanda (CP/CPP/LEP por grep do artigo; penal-especial; jurisprudencia).

## Objetivo
Transformar qualquer demanda de defesa penal em entrega correta e validada, conduzindo a persecucao sem perder o estado e sem esquecer nenhuma exigencia processual, calculo temporal ou tese.

## Metodologia
1. **Ler** `context/metodologia-criminal.md`.
2. **Classificar** via `triagem-criminal` (fase da persecucao + objetivo + skill alvo + situacao prisional).
3. **Carregar** `memoria-de-caso-criminal` (reu, vitima, MP, fase, processo, prazos, situacao prisional, providencias).
4. **Gestao processual SEMPRE (Camada 2):** competencia-criminal, prazos-processuais-penais, nulidades-penais, cadeia-de-custodia-e-provas, estrategia-penal — antes/junto de qualquer peca. Esse e o "nao esquecer nada".
5. **Conduzir a persecucao** na ordem cabivel: investigacao/flagrante -> liberdade -> resposta a acusacao -> instrucao -> alegacoes finais -> sentenca -> recursos -> execucao penal.
6. **Acionar o Motor Penal Temporal quando cabivel** (Camada 3/4): `prescricao-penal`, `dosimetria-da-pena`, `motor-calculo-de-pena`, `progressao-de-regime`, `livramento-condicional` — sempre com linha do tempo + marcos + parecer.
7. **Gate final:** toda entrega passa pela `suprema-corte-criminal` (R1-R4).
8. **Atualizar** `memoria-de-caso-criminal` (ato praticado, proximo passo, prazo, situacao prisional).

## Regras de ouro
- **Lei vigente 2024-2026 (meu treino vai so ate jan/2026):** art. 112 LEP reescrito pela Lei 15.402/2026 (base 1/6 + excecoes, NAO 16-70% de 2019); Antifacao 15.358/2026 (elevou hediondos: V=70%, VI=75% incl. lider orcrim ultraviolenta, VII=80%, VIII=85% reincidente+hediondo+morte — NAO e "85% para faccao"); feminicidio autonomo CP 121-A (Lei 14.994/2024). Sempre ler a redacao NAO-tachada em context/.
- **Calculo penal nunca de cabeca** — sempre com a lei seca aberta + validador-criminal. Errar pena/prescricao sob OAB e catastrofe.
- **Cross-link, nao duplicar:** calculo monetario -> calculosjudiciais-adv-os; execucao civel -> execucao-adv-os.

## Entrega obrigatoria final
- Artefato da skill acionada, validado pela suprema-corte-criminal + `memoria-de-caso-criminal` atualizado + proximo passo/prazo.

## Guard
Nenhum dispositivo/jurisprudencia/percentual/calculo sem `validador-criminal`. Nunca produzir peca ou calculo sem a gestao processual transversal. Na duvida de vigencia/existencia, bloquear e checar no arquivo da lei seca (context/).
