---
name: progressao-de-regime
description: "A MAIS SENSIVEL — calcula progressao de regime pela redacao VIGENTE do art. 112 da LEP (Lei 15.402/2026 base 1/6 + excecoes; Lei 15.358/2026 fracoes de hediondos). LE o anexo e mapeia o inciso correto por situacao; NUNCA decora percentual. Use quando o operador disser progressao de regime, quando progride, fracao de progressao, semiaberto, regime menos rigoroso, ou pedir a data da progressao."
---

# PROGRESSAO-DE-REGIME

> Camada 4 (execucao penal — LEP). A LEI MUDOU EM 2026: o art. 112 foi reescrito. Conferir SEMPRE no arquivo, jamais de memoria. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/lep-7210-84.md` — **grep "Art. 112"** e ler a faixa NAO-tachada (Lei 15.402/2026 + 15.358/2026). ⚠️ os percentuais 16-70% de 2019 estao TACHADOS — ignorar.
- `context/cp-2848-40.md` — art. 33 (regimes: fechado/semiaberto/aberto).
- `context/jurisprudencia-criminal.md` — so citar item ✅ (SV 26, SV 56).

## Objetivo
Entregar a **fracao aplicavel citando o inciso vigente** do art. 112, a **data da progressao**, o requisito subjetivo e o parecer — sempre lido do arquivo da lei seca, nunca decorado.

## Quando ativar
- Saber quando o apenado progride (fechado -> semiaberto -> aberto).
- Calcular a fracao/data de progressao por situacao (primario/reincidente, comum/hediondo, com/sem resultado morte, orcrim ultraviolenta).
- Falta de vaga no regime mais brando (SV 56).
- Falta grave que reinicia a contagem.

## Metodologia
> ⚠️ **Antes de tudo: abrir `lep-7210-84.md`, ler o art. 112 NAO-tachado e mapear o inciso. NAO decorar numero.**
1. **Caput (Lei 15.402/2026) — base 1/6.** Progride com **ao menos 1/6 da pena** no regime anterior + merito, **observadas as excecoes** dos incisos. So sai dessa base quem cai numa excecao.
2. **Classificar:** primario x reincidente; com x sem violencia/grave ameaca; crime do Titulo XII do CP x demais; hediondo/equiparado; com x sem resultado morte; orcrim ultraviolenta; feminicidio; milicia.
3. **Mapear o inciso vigente (LER no arquivo — abaixo so o esqueleto):**
   - **I** — primario + violencia/grave ameaca (salvo Titulo XII CP) -> **25%** (15.402/2026).
   - **II** — reincidente + violencia/grave ameaca (salvo Titulo XII CP) -> **30%** (15.402/2026).
   - **III** — reincidente em crime **diverso** dos incisos I e II -> **20%** (15.402/2026).
   - **IV** — reincidente em crime com violencia/grave ameaca -> **30%** (13.964/2019, mantido).
   - **V** — hediondo/equiparado, **primario** -> **70%** (15.358/2026).
   - **VI** — **75%** (15.358/2026), se: a) hediondo c/ **resultado morte**, primario (vedado livramento); b) comando de **orcrim ULTRAVIOLENTA** estruturada p/ hediondo (vedado livramento) — **VI-b = 75%, NAO 85%**; c) milicia privada; d) **feminicidio** primario (vedado livramento).
   - **VI-A** — **revogado** (15.358/2026).
   - **VII** — **reincidente** em hediondo/equiparado -> **80%** (15.358/2026).
   - **VIII** — **reincidente** em hediondo c/ **resultado morte** -> **85%** (vedado livramento) (15.358/2026). ⚠️ 85% e o inciso VIII (reincidente+hediondo+morte) — **NAO** e "85% para faccao".
   - **§3** — mulher gestante/mae ou responsavel (cumulativos: sem violencia, nao contra filho, primaria, bom comportamento, sem orcrim) -> **1/8** (13.769/2018).
   - **§5** — trafico privilegiado (art. 33 §4 da Lei 11.343/06) **nao** e hediondo para esse fim.
4. **Requisito SUBJETIVO (LEP art. 112, §1 — red. Lei 14.843/2024).** Boa conduta carceraria comprovada pelo diretor (atestado) **e** resultado do exame criminologico. **SV 26 ✅:** exame exige **decisao fundamentada**; vedacao generica de progressao em hediondo e inconstitucional.
5. **Falta grave (art. 112, §6).** Interrompe o prazo: o requisito objetivo **reinicia sobre a pena remanescente**. Recalcular a data-base. §7: bom comportamento readquirido apos 1 ano do fato (ou antes, se cumprido o requisito temporal).
6. **Regimes (CP 33).** Por etapa: fechado -> semiaberto -> aberto. **SV 56 ✅:** falta de vaga no regime adequado **nao** autoriza regime mais gravoso — cabe regime mais brando/domiciliar ate a vaga (RE 641.320/RS).
7. **Calcular:** saldo a cumprir (apos detracao/remicao) x fracao do inciso -> tempo exigido -> data da progressao a partir da data-base.

## Saida obrigatoria (calculo + data + parecer)
**Fracao aplicavel citando o inciso vigente** + **data da progressao** + requisito subjetivo (atestado + exame se fundamentado — SV 26) + nota de qual lei deu a redacao (15.402/2026 e/ou 15.358/2026) + parecer + handoff. Passa pela `suprema-corte-criminal`.

## Guard
Nenhuma fracao/data sai sem `validador-criminal` (cruza `context/`). ⚠️ **Conferir SEMPRE o inciso no `lep-7210-84.md`, nunca decorar.** Percentual 16-70% de 2019 -> BLOQUEAR (tachado). Lider orcrim ultraviolenta = VI-b = 75% (nao 85%); 85% = VIII. Jurisprudencia so se ✅. Gate final `suprema-corte-criminal`.

progressao-de-regime -> arts. citados: LEP 112 (caput base 1/6 + I-VIII + §1 subjetivo + §3 mulher 1/8 + §5 trafico privilegiado + §6 falta grave), 66; CP 33; SV 26 ✅, SV 56 ✅ — fracao/inciso que LI como vigente: caput 1/6 (15.402/2026); I=25, II=30, III=20, IV=30, V=70, VI=75 (a/b/c/d; VI-b orcrim ultraviolenta), VI-A revogado, VII=80, VIII=85 (15.358/2026).
