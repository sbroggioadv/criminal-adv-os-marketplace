Mode: production

# criminal-adv-os — Criminal Defense & Procedure Master

Plugin Claude Code de **defesa penal brasileira** — o sistema operacional do advogado criminalista, da investigação à extinção da pena. Orquestrador **`criminal-master`** que dirige (dirime) **todas** as skills necessárias por tarefa, sem esquecer nenhuma.

> Onboarding: **`/start-criminal`**. Porta única: **`criminal-master`**.

## Diferencial — Motor Penal Temporal
Além das peças, o criminal tem um subsistema **computacional**: **prescrição** (todas as modalidades), **dosimetria** (3 fases), **motor de cálculo de pena** (entradas → pena final, regime, benefícios, linha do tempo) e **execução penal temporal** (progressão, livramento, remição, detração). Cada saída = linha do tempo + marcos + cálculo fundamentado + parecer, **sempre grounded na lei seca de `context/`**.

## Cobertura (10 camadas)
- **Orquestração & QA:** criminal-master, triagem, memória de caso, estilo, Suprema Corte R1-R4.
- **Fundação enraizada:** CP, CPP, LEP, leis penais especiais, jurisprudência STF/STJ, validador.
- **Gestão processual penal:** competência, prazos processuais penais, nulidades, cadeia de custódia e provas, estratégia, cronologia.
- **Motor Penal Temporal:** prescrição, decadência/perempção, dosimetria, motor de cálculo de pena, concurso de crimes/penas, extinção da punibilidade.
- **Execução penal (LEP):** progressão, livramento, remição, detração, benefícios/saída, incidentes (falta grave, regressão, unificação).
- **Acordos:** ANPP, transação penal, suspensão condicional do processo, sursis penal.
- **Defesa, liberdade & investigação:** flagrante/custódia, liberdade provisória/preventiva, resposta à acusação, alegações finais, habeas corpus, MS criminal, investigação defensiva, assistente.
- **Recursos:** RESE, apelação, embargos, recursos excepcionais, HC nos tribunais superiores, revisão criminal.
- **Tribunal do Júri:** fase 1 (pronúncia), estratégia pré-plenário, teses e quesitos, plenário/sustentação, recursos.
- **Leis penais especiais:** drogas, hediondos/anticrime, organização criminosa, lavagem, violência doméstica.

## Fundação jurídica enraizada (`context/`)
CP (DL 2.848/40) + CPP (DL 3.689/41) + LEP (Lei 7.210/84) consolidados · leis especiais (drogas 11.343/06, hediondos 8.072/90, anticrime 13.964/19, orcrim 12.850/13, lavagem 9.613/98, Maria da Penha 11.340/06) · jurisprudência STF/STJ.

> **Lei vigente (2024-2026) — não errar:** o art. 112 da LEP (progressão) foi **reescrito pela Lei 15.402/2026** (base 1/6 + exceções graduadas — NÃO os 16-70% de 2019, hoje revogados); **Lei 15.358/2026 (Antifacção)** elevou frações de hediondos no art. 112 LEP (V=70%, VI=75% incl. líder orcrim ultraviolenta, VII=80%, VIII=85% reincidente+hediondo+morte); **Lei 14.994/2024** tornou o feminicídio crime autônomo (CP 121-A). Sempre ler a redação **não-tachada** em `context/`.

## Fronteiras
Cálculo **monetário** (atualização/juros cível) → `calculosjudiciais-adv-os`. Execução **cível** → `execucao-adv-os`. Cível/consumidor/trabalhista/família = fora. **Foco: defesa penal.**

## Comandos principais
`/start-criminal` · `/criminal-master` · `/triagem-criminal` · `/calculo-pena` · `/prescricao` · `/dosimetria` · `/execucao-penal` · `/anpp` · `/habeas-corpus` · `/recurso-criminal` · `/juri` · `/revisao-final` · `/status-criminal`
