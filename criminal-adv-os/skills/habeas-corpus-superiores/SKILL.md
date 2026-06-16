---
name: habeas-corpus-superiores
description: "Estrategia de HC nos tribunais superiores (STJ e STF) e RECLAMACAO constitucional na defesa criminal. Use para HC no STJ, HC no STF, habeas corpus nos tribunais superiores, HC originario ou substitutivo, reclamacao, preservar competencia, garantir autoridade de decisao, descumprimento de sumula vinculante ou de tese vinculante."
---

# HABEAS-CORPUS-SUPERIORES

> Camada 7 (estrategia no STJ/STF). Define quando e como levar o HC ao tribunal superior e quando usar a RECLAMACAO. Foco: DEFESA. Cross-link: skill `habeas-corpus` (a base — hipoteses do CPP art. 648, liminar, alvara).

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — grep o HC (art. 647 cabimento; art. 648 hipoteses de coacao ilegal; art. 647-A — concessao de oficio, Lei 14.836/2024).
- `context/jurisprudencia-criminal.md` — so itens ✅ (Tema 1.016 art. 226 CPP; ADC 43/44/54; Tema 1.068 juri ≥15 anos — uteis no HC).
- `context/penal-especial.md` — reformas 2024-2026.

## Objetivo
Escolher a via correta no topo do sistema: subir HC ao STJ/STF quando a coacao ilegal persiste apos a instancia ordinaria, e usar a RECLAMACAO quando ato judicial usurpa competencia da Corte ou descumpre decisao/tese vinculante — sem cair na vedacao ao HC substitutivo de recurso proprio.

## Quando ativar
Prisao/constrangimento ilegal mantido por tribunal (TJ/TRF) com decisao a impugnar no STJ; ou ato que afronta sumula vinculante / tese de repetitivo / acordao do STJ/STF -> reclamacao. Tambem "HC pra trancar acao no STJ", "reclamacao porque descumpriram a sumula vinculante".

## Metodologia
1. **HC originario nos superiores (competencia constitucional):**
   - **STJ — CF art. 105, I, "c":** HC quando o coator ou paciente tiver foro no STJ OU quando o coator for tribunal sujeito a sua jurisdicao (ex.: ato de TJ/TRF -> HC ao STJ) — ambas as hipoteses estao na alinea "c".
   - **STF — CF art. 102, I:** "d" HC originario; "i" HC quando o coator for tribunal superior (ex.: ato do STJ -> HC ao STF).
2. **HC substitutivo — cuidado.** As Cortes restringem o HC como **substitutivo do recurso cabivel** (🟡 validador). Saida: impetrar o HC e, havendo coacao flagrante, pedir tambem **concessao de oficio** (CPP art. 647-A — Lei 14.836/2024). Com recurso proprio (agravo, RESE), avaliar a via recursal em paralelo (ver `recursos-excepcionais-criminais`).
3. **Cabimento material do HC** — a coacao tem de se enquadrar no **CPP art. 648** (falta de justa causa; excesso de prazo; incompetencia do coator; cessacao do motivo; fianca negada; processo manifestamente nulo; extinta a punibilidade). Liminar + alvara/relaxamento conforme a skill base `habeas-corpus`.
4. **RECLAMACAO (via autonoma, nao e HC):**
   - **STJ — CF art. 105, I, "f":** preservar a competencia do STJ e garantir a autoridade de suas decisoes.
   - **STF — CF art. 102, I, "l":** preservar a competencia do STF e garantir a autoridade de suas decisoes.
   - **Cabimento tipico na defesa:** ato que descumpre **sumula vinculante** (CF art. 103-A) ou nao aplica tese de repetitivo/repercussao geral vinculante. Exige aderencia estrita ao paradigma — apontar a decisao/sumula descumprida e a identidade material. ⚠️ Esgotamento de instancia e requisitos da reclamacao (regime, Sumula 734 STF): **remeter ao `validador-criminal`**.
5. **Decisao de via:** HC para coacao a liberdade de locomocao; reclamacao para usurpacao de competencia ou descumprimento de precedente vinculante. Nunca trocar uma pela outra.

## Entrega obrigatoria final
- Via escolhida (HC originario STJ 105, I / STF 102, I — ou reclamacao 105, I "f" / 102, I "l") + fundamento de cabimento (CPP art. 648 no HC; paradigma vinculante descumprido na reclamacao) + alerta sobre HC substitutivo + minuta com liminar (HC) ou pedido de cassacao do ato (reclamacao).

## Guard
Fecha em `suprema-corte-criminal` (R1-R4) e toda tese/sumula/tema passa por `validador-criminal`. Dispositivos da CF (105, I "c"/"f"; 102, I "d"/"i"/"l"; 103-A) sao constitucionais — citar como CF, sem inventar. Vedacao ao HC substitutivo e requisitos da reclamacao (esgotamento, paradigma, Sumula 734 STF): validador antes de sustentar. Na duvida, bloquear.

habeas-corpus-superiores -> CF art. 105, I ("c" HC — foro STJ ou coator=tribunal sujeito a STJ, "f" reclamacao STJ); CF art. 102, I ("d"/"i" HC, "l" reclamacao STF); CF art. 103-A (sumula vinculante); CPP art. 647, 648 e 647-A (Lei 14.836/2024); cross-link `habeas-corpus`.
