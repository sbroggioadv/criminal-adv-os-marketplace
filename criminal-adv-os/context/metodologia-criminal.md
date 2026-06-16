# Metodologia Criminal — Mapa de Uso do Plugin

> Anexo central. O `criminal-master` lê este arquivo primeiro. Define como as skills se articulam, qual anexo cada uma usa, o fluxo da persecução penal e as regras de ouro.

## Arquitetura (10 camadas — ~61 skills)
- **Camada 0 — Orquestração/QA:** `criminal-master`, `criminal-onboarding`, `triagem-criminal`, `memoria-de-caso-criminal`, `estilo-criminal`, `suprema-corte-criminal`.
- **Camada 1 — Fundação:** `base-legal-cp`, `base-legal-cpp`, `base-legal-lep`, `base-legal-penal-especial`, `jurisprudencia-criminal`, `validador-criminal`.
- **Camada 2 — Gestão processual penal:** `competencia-criminal`, `prazos-processuais-penais`, `nulidades-penais`, `cadeia-de-custodia-e-provas`, `estrategia-penal`, `cronologia-penal-e-providencias`.
- **Camada 3 — MOTOR PENAL TEMPORAL (pena & extinção):** `prescricao-penal`, `decadencia-perempcao`, `dosimetria-da-pena`, `motor-calculo-de-pena`, `concurso-de-crimes-e-penas`, `extincao-da-punibilidade`.
- **Camada 4 — Execução Penal (LEP):** `guia-de-execucao-penal`, `progressao-de-regime`, `livramento-condicional`, `remicao`, `detracao`, `beneficios-saida-e-cautelares-penais`, `incidentes-execucao-penal`.
- **Camada 5 — Acordos & despenalização:** `anpp`, `transacao-penal`, `suspensao-condicional-processo`, `sursis-penal`.
- **Camada 6 — Defesa, liberdade & investigação:** `flagrante-e-audiencia-custodia`, `liberdade-provisoria-e-preventiva`, `resposta-a-acusacao`, `alegacoes-finais-memoriais`, `habeas-corpus`, `mandado-seguranca-criminal`, `investigacao-defensiva`, `assistente-de-acusacao`.
- **Camada 7 — Recursos:** `rese`, `apelacao-criminal`, `embargos-criminais`, `recursos-excepcionais-criminais`, `habeas-corpus-superiores`, `revisao-criminal`, `carta-testemunhavel-e-residuais`.
- **Camada 8 — Tribunal do Júri:** `juri-fase-1-pronuncia`, `juri-estrategia-pre-plenario`, `juri-teses-e-quesitos`, `juri-plenario-sustentacao`, `juri-recursos`.
- **Camada 9 — Leis penais especiais:** `lei-de-drogas`, `crimes-hediondos-e-equiparados`, `organizacao-criminosa-e-colaboracao`, `lavagem-e-financeiros`, `violencia-domestica-e-vulneraveis`.

## Anexos de `context/`
| Anexo | Conteúdo | Como usar |
|---|---|---|
| `cp-2848-40.md` | Código Penal consolidado (~388KB) | **grep o artigo** + ler a faixa (não ler inteiro) |
| `cpp-3689-41.md` | Código de Processo Penal consolidado (~384KB) | idem |
| `lep-7210-84.md` | Lei de Execução Penal consolidada (~159KB) | idem — **art. 112 tem redação 2026, ler a NÃO-tachada** |
| `penal-especial.md` | Recortes vigentes de leis especiais + reformas 2024-2026 | ler antes de citar lei especial |
| `lei-9099-95.md` | Lei 9.099/95 — JECrim (recorte criminal arts. 60-92): transação penal, sursis processual, IMPO, TCO | **grep o artigo** (61/76/89) + ler a faixa vigente |
| `jurisprudencia-criminal.md` | Súmulas/temas STF/STJ marcados ✅/🟡/❌ | só citar ✅; 🟡 conferir; nunca ❌ |

## Fluxo da persecução penal (conduzido pelo `criminal-master`)
```
triagem-criminal (fase + objetivo) → memoria-de-caso-criminal (estado) →
[SEMPRE] gestão processual: competência · prazos/tempestividade · nulidades · estratégia →
fase: investigação/flagrante → resposta à acusação → instrução → alegações finais → sentença →
recursos (RESE/apelação/embargos/excepcionais/HC) → execução penal (LEP) →
[QUANDO CABÍVEL] Motor Penal Temporal: prescrição · dosimetria · cálculo de pena · progressão →
suprema-corte-criminal (R1-R4) em TODA entrega
```

## Regras de ouro
1. **Gestão processual transversal** antes de toda peça (competência, prazos em dias — atenção: prazo penal conta diferente do CPC), nulidades, estratégia.
2. **Motor Temporal = cálculo fundamentado**, nunca "de cabeça": prescrição (CP 109-117), dosimetria (CP 59/68), pena, progressão/livramento (LEP) — sempre com a lei seca aberta + linha do tempo + parecer.
3. **🔴 LEI VIGENTE 2024-2026 (crítico — meu treino vai até jan/2026):**
   - **Art. 112 LEP** reescrito pela **Lei 15.402/2026** (base 1/6 + exceções graduadas; os 16-70% de 2019 estão revogados/tachados). **Lei 15.358/2026 (Antifacção)** elevou frações de hediondos: 70% (V), 75% (VI — inclui VI-b: líder de orcrim ultraviolenta), 80% (VII), 85% (VIII — reincidente+hediondo+resultado morte). ⚠️ O 85% é do inciso VIII — NÃO é genérico "para facção"; líder de orcrim ultraviolenta = 75% (VI-b).
   - **Feminicídio** = crime autônomo CP 121-A (**Lei 14.994/2024**), hediondo. **Lei 15.159/2025** reescreveu o rol de hediondos.
   - Leis confirmadas no Planalto capturado: 15.402, 15.397, 15.358, 15.407, 15.410, 15.295, 15.159, 14.994. **NÃO** existe "15.299/2025" nos códigos (🟡). **Fonte de verdade = `context/`, não memória de treino nem busca de IA.**
4. **Anti-alucinação** via `validador-criminal` (cruza `context/`). **Gate final** `suprema-corte-criminal`.
5. **Foco DEFESA.** **Cross-link, não duplicar:** cálculo monetário → `calculosjudiciais-adv-os`; execução cível → `execucao-adv-os`.
