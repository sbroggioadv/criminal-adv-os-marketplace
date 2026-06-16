---
name: validador-criminal
description: "Anti-alucinacao do plugin criminal (a skill mais importante da fundacao). Antes de QUALQUER dispositivo, sumula, tese, percentual ou calculo entrar numa peca, CRUZA com o context/ (grep o artigo na lei seca, confere a redacao VIGENTE/nao-tachada; confere a sumula no anexo ✅). Aciona o guard global anti-alucinacao-juridica. Na duvida, BLOQUEIA. Use quando o operador disser validar, confere se existe, isso e vigente, anti-alucinacao, ou antes de citar qualquer norma/jurisprudencia/percentual."
---

# VALIDADOR-CRIMINAL — Anti-Alucinacao da Fundacao

> Camada 1 (fundacao enraizada — a mais importante). Esta skill NAO redige peca — ela e o crivo: nada (dispositivo, sumula, tese, percentual, calculo) entra numa peca sem ser cruzado com o `context/`. A fonte de verdade e o ARQUIVO DA LEI SECA capturado, nunca a memoria de treino nem busca de IA isolada.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` · `context/cpp-3689-41.md` · `context/lep-7210-84.md` — leis secas (grep o artigo + ler a redacao VIGENTE/nao-tachada).
- `context/penal-especial.md` — leis especiais + alertas de vigencia 2024-2026.
- `context/jurisprudencia-criminal.md` — sumulas/temas (so ✅).

## Objetivo
Impedir que dispositivo revogado, percentual defasado, sumula cancelada ou calculo errado cheguem ao juiz/MP — cruzando cada item com o arquivo da lei seca antes de liberar.

## Metodologia
1. **Listar** todos os itens citaveis da peca: dispositivos (CP/CPP/LEP/especiais), sumulas/temas, percentuais de progressao, marcos de prescricao, calculos.
2. **Cruzar dispositivo:** grep `Art. N` na lei seca → conferir a redacao **VIGENTE / nao-tachada** (atencao aos trechos `~~` tachados, sobretudo art. 112 LEP).
3. **Cruzar jurisprudencia:** localizar no `jurisprudencia-criminal.md` → so liberar item ✅; 🟡 manda checar ao vivo; ❌ rejeita.
4. **Cruzar percentual/calculo:** reler o percentual no arquivo (nao de cabeca) e refazer o calculo contra a redacao vigente.
5. **Acionar** o guard global `anti-alucinacao-juridica` para a camada de jurisprudencia.
6. **Veredito por item:** OK (consta no arquivo) ou BLOQUEAR (nao consta / divergente / 🟡 sem checagem).

## ⚠️ Licao real (por que o arquivo vence)
A **Lei 15.402/2026** existe (texto compilado do Planalto, capturado em `context/`), mas uma curadoria de IA chegou a marca-la como "inexistente". Por isso a fonte de verdade e o **arquivo da lei seca**, nao a memoria de treino (vai so ate jan/2026) nem busca de IA isolada. Na duvida, conferir ao vivo (firecrawl/Planalto) — nunca chutar.

## Entrega obrigatoria final
- Tabela de veredito (item · onde consta no `context/` · OK/BLOQUEAR) + a lista do que precisa de checagem ao vivo antes de a peca seguir.

## Guard
Qualquer item que nao constar literalmente no `context/`, divergir da redacao vigente, ou estiver 🟡 sem reconferencia: **BLOQUEAR**. Calculo/percentual duvidoso: bloquear e refazer. Toda entrega fecha pela `suprema-corte-criminal`.
