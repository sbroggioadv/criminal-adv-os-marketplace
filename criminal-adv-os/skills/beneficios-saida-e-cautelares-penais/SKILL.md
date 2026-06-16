---
name: beneficios-saida-e-cautelares-penais
description: "Analisa cabimento de beneficios e cautelares na execucao penal (LEP) — saida temporaria (122-125), monitoracao eletronica (146-B a 146-D) e prisao domiciliar na execucao (117). Use quando o operador disser saida temporaria, saidao, monitoracao eletronica, tornozeleira, prisao domiciliar na execucao, recolhimento em residencia, ou perguntar se o apenado tem direito a sair do estabelecimento."
---

# BENEFICIOS DE SAIDA E CAUTELARES PENAIS — Saidao, tornozeleira e domiciliar

> Camada 4 (execucao penal — LEP). Skill de analise de cabimento: cruza requisitos, situacao do apenado e redacao vigente para dizer se o beneficio cabe e como pedir. O `criminal-master` acopla a peticao e o gate `suprema-corte-criminal`.

## Anexos obrigatorios (context/)
- `context/lep-7210-84.md` — buscar `Art. 122` a `Art. 125` (saida temporaria), `Art. 146-B` a `Art. 146-D` (monitoracao eletronica) e `Art. 117` (recolhimento em residencia); ler so a faixa, **a redacao NAO-tachada** (saida temporaria reformada pela **Lei 14.843/2024**).
- `context/jurisprudencia-criminal.md` — so itens marcados ✅ (Sumula Vinculante 56 = falta de vaga, ✅).

## Objetivo
Dizer se cabe saida temporaria, monitoracao eletronica ou prisao domiciliar, listar requisitos atendidos e faltantes e devolver parecer pronto — lendo a lei vigente do arquivo, nunca de memoria.

## Quando ativar
- Apenado em regime semiaberto quer saida temporaria (curso, datas comemorativas).
- Pedido ou defesa de monitoracao eletronica (tornozeleira).
- Prisao domiciliar/recolhimento em residencia na execucao (idoso, doente, mae, gestante, ou falta de vaga — SV 56).
- Revogacao de qualquer desses beneficios ameaca o apenado.

## Metodologia
1. **Abrir a lei seca** e identificar a situacao prisional (regime, lapso cumprido, comportamento, natureza do crime) com a `memoria-de-caso-criminal`.
2. **Saida temporaria — art. 122:** so para **regime semiaberto**, **sem vigilancia direta**. ⚠️ A Lei 14.843/2024 **revogou os incisos I (visita a familia) e III (retorno ao convivio social)** — sobrou o inciso II (frequencia a curso supletivo/profissionalizante/ensino medio ou superior na comarca). § 2 (red. 14.843/2024): **nao tem direito** a saida temporaria nem a trabalho externo sem vigilancia direta o condenado por crime hediondo ou com violencia/grave ameaca contra pessoa. ⚠️ Conferir no anexo se lei de 2026 (ex.: 15.358/2026) alterou requisitos ou datas comemorativas antes de afirmar.
3. **Saida temporaria — requisitos do art. 123:** (I) comportamento adequado; (II) cumprimento minimo de **1/6 da pena se primario, 1/4 se reincidente**; (III) compatibilidade com os objetivos da pena. Concedida por ato motivado do juiz, ouvidos MP e administracao (art. 123 caput). ⚠️ Art. 124 (prazo de 7 dias renovavel) esta **revogado** pela Lei 14.843/2024 — nao citar como vigente; ler a regra de prazo/intervalo vigente no arquivo.
4. **Revogacao da saida — art. 125:** revoga automaticamente se o apenado praticar fato definido como crime doloso, for punido por falta grave, desatender condicoes ou revelar baixo aproveitamento do curso; a recuperacao depende de absolvicao, cancelamento da punicao ou demonstracao de merecimento.
5. **Monitoracao eletronica — art. 146-B:** o juiz pode fiscalizar por monitoracao ao autorizar saida temporaria no semiaberto (II), determinar prisao domiciliar (IV), aplicar pena/conceder progressao para regime aberto ou semiaberto (VI), pena restritiva com limitacao de frequencia a lugares (VII) e conceder livramento condicional (VIII) — incisos VI a VIII pela Lei 14.843/2024.
6. **Deveres e revogacao — arts. 146-C e 146-D:** o apenado recebe visitas do servidor e nao viola o equipamento (146-C); violar dever ou cometer falta grave pode gerar regressao, revogacao da saida/domiciliar/livramento ou conversao da PRD (146-C, par. unico). A monitoracao se revoga quando desnecessaria/inadequada ou por violacao/falta grave (146-D).
7. **Prisao domiciliar na execucao — art. 117:** recolhimento em residencia ao beneficiario de regime aberto quando: (I) maior de 70 anos; (II) doenca grave; (III) condenada com filho menor ou deficiente; (IV) condenada gestante. ⚠️ **Falta de vaga** em estabelecimento adequado autoriza regime mais brando/domiciliar ate surgir vaga — **Sumula Vinculante 56 do STF (RE 641.320/RS), ✅** — citar so apos `validador-criminal`.
8. Em divergencia entre memoria e texto, vence o texto do arquivo.

## Saida obrigatoria
- **Veredito de cabimento** por beneficio pedido (cabe / nao cabe / cabe com ressalva), com o artigo.
- **Requisitos atendidos x faltantes** (regime, lapso 1/6 ou 1/4, comportamento, natureza do crime, hipotese do art. 117) em lista objetiva.
- **Fundamento legal artigo a artigo** + ressalva sobre reformas 2024-2026 (saida temporaria) e SV 56 (falta de vaga), so se validadas.
- **Parecer** com o pedido recomendado e os documentos/provas a juntar no incidente.

## Guard
Nenhum requisito, lapso ou natureza de crime entra sem `validador-criminal` (cruza `context/`). Saida temporaria: se o texto parecer a redacao antiga (incisos I/III ativos, art. 124 com prazo de 7 dias), BLOQUEAR — esta tachada; ler a vigente (Lei 14.843/2024). SV 56 e demais sumulas: so com `validador-criminal` + `anti-alucinacao-juridica`. Toda entrega fecha pela `suprema-corte-criminal`.
