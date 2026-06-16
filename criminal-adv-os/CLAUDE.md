# CLAUDE.md — criminal-adv-os (Criminal Defense & Procedure Master)

> Estende o CLAUDE.md global/workspace. Regras locais do plugin de defesa penal.

## Regras invioláveis do plugin
1. **Sempre consultar `context/` antes de redigir ou calcular.** CP/CPP/LEP, leis especiais e jurisprudência vivem nos anexos — os arquivos são grandes (CP ~388KB, CPP ~384KB, LEP ~159KB): **localizar o artigo por busca (grep) e ler a faixa**, não despejar o anexo inteiro. Cada skill lista seus anexos.
2. **`criminal-master` dirime TODAS as skills** pertinentes à tarefa, sem esquecer nenhuma. Nunca produzir peça ou cálculo sem antes passar pela gestão processual transversal (competência, prazos/tempestividade, nulidades, estratégia).
3. **Gate Suprema Corte.** Antes de QUALQUER entrega, `suprema-corte-criminal` (R1 fatos/competência · R2 tipicidade + lei vigente · R3 jurisprudência real · R4 forma/prazo/dosimetria/cálculo).
4. **Anti-alucinação.** Nenhum dispositivo/súmula/tese/acórdão e nenhum cálculo de pena entra em peça sem `validador-criminal` (cruza `context/` + guard global `anti-alucinacao-juridica`). Na dúvida, bloquear e checar ao vivo.
5. **Lei vigente (2024-2026) — NÃO errar (meu conhecimento de treino vai até jan/2026; a lei mudou depois):**
   - **Art. 112 da LEP (progressão)** foi **REESCRITO pela Lei 15.402/2026** — modelo de **base 1/6 + exceções graduadas**. Os percentuais 16-70% da Lei 13.964/2019 estão **TACHADOS (revogados)** no Planalto. **Ler a redação não-tachada.**
   - **Lei 15.358/2026 (Antifacção)** — elevou frações de hediondos no art. 112 LEP (V=70%, VI=75% incl. líder orcrim ultraviolenta, VII=80%, VIII=85% reincidente+hediondo+morte); criou domínio social estruturado (novo hediondo). ⚠️ 85% é do inciso VIII — NÃO é percentual genérico "para facção" (líder orcrim = 75% VI-b).
   - **Lei 14.994/2024** — feminicídio é **crime autônomo** (CP art. 121-A), hediondo. **Lei 15.159/2025** reescreveu o rol de hediondos.
   - Em prescrição/dosimetria/progressão, SEMPRE conferir a redação vigente no arquivo da lei seca antes de citar número/percentual.
6. **Foco: DEFESA.** A Suprema Corte valida a tese defensiva. Acusatório só como contraponto (júri, assistente de acusação).
7. **Motor Penal Temporal:** todo cálculo (prescrição, pena, progressão, livramento) sai com **linha do tempo + marcos + fundamento legal artigo a artigo + parecer**, e passa pelo `validador-criminal`. Calcular errado a pena/prescrição sob OAB é catástrofe — na dúvida, bloquear.
8. **Fronteiras:** cálculo monetário → `calculosjudiciais-adv-os`; execução cível → `execucao-adv-os`; cível/família/trabalhista fora.

## Porta única
`criminal-master` é o orquestrador: classifica via `triagem-criminal` (fase da persecução + objetivo), carrega `memoria-de-caso-criminal`, seleciona e conduz todas as skills, e fecha pela `suprema-corte-criminal`.
