---
name: suprema-corte-criminal
description: "Gate de qualidade R1-R4 obrigatorio antes de QUALQUER entrega do plugin criminal (peca, calculo ou parecer). R1 fatos/competencia · R2 tipicidade + lei VIGENTE (2024-2026) · R3 jurisprudencia real · R4 forma/prazo/dosimetria/calculo. Use sempre como ultima etapa antes de entregar, ou quando o operador disser revisao final, suprema corte, valida antes de protocolar, /revisao-final."
---

# SUPREMA-CORTE-CRIMINAL — Gate R1-R4

> Tier 0. Revisao adversarial final. Nada sai do plugin sem passar por aqui. Foco: proteger a DEFESA e o advogado (OAB).

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` / `context/cpp-3689-41.md` / `context/lep-7210-84.md` (grep o artigo citado e conferir a redacao VIGENTE/nao-tachada).
- `context/jurisprudencia-criminal.md` (so itens ✅) + `context/penal-especial.md` (reformas 2024-2026).

## Objetivo
Pegar erro antes do juiz/MP pegar: fato sem lastro, tipicidade errada, lei revogada citada como vigente, jurisprudencia inexistente, calculo de pena/prescricao errado, peca intempestiva ou mal-formada.

## As 4 revisoes (R1-R4)
1. **R1 — Fatos & competencia:** os fatos batem com o que consta? Competencia/foro/prerrogativa corretos? Situacao prisional considerada?
2. **R2 — Tipicidade & lei VIGENTE:** o tipo penal e os dispositivos citados existem e estao em vigor HOJE? **Conferir a redacao nao-tachada em context/** (ex.: art. 112 LEP = Lei 15.402/2026, NAO os 16-70% de 2019; feminicidio = CP 121-A). Nenhuma lei revogada como vigente.
3. **R3 — Jurisprudencia real:** toda sumula/tese/acordao citado consta em `context/jurisprudencia-criminal.md` com ✅? Se 🟡/ausente, bloquear ate confirmar via `validador-criminal`.
4. **R4 — Forma, prazo & calculo:** prazo penal/recursal correto e tempestivo? Peca na estrutura certa? **Todo calculo (pena/prescricao/progressao) refeito e conferido contra a lei seca, com linha do tempo + marcos.** Pedidos e dosimetria coerentes.

## Entrega obrigatoria final
- Veredito por R (OK / corrigir: <o que>) + a versao corrigida da peca/calculo, pronta para o advogado revisar e assinar.

## Guard
Se qualquer R falhar, NAO liberar — corrigir e reexaminar. Calculo penal e tipicidade duvidosos: bloquear. A responsabilidade final e do advogado; este gate reduz o risco, nao o substitui.
