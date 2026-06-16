---
name: remicao
description: "Calcula remicao de pena na execucao penal (LEP 126-130) por trabalho, estudo, leitura e cumulacao, com impacto na data de progressao/livramento e parecer. Use quando o operador disser remicao, remir pena, descontar pena por trabalho/estudo/leitura, aproveitamento de estudo na pena, perda de dias remidos por falta grave, ou pedir atestado de remicao."
---

# REMICAO — Desconto de pena por trabalho, estudo e leitura

> Camada 4 (execucao penal — LEP). Skill de calculo: traduz dias trabalhados e horas de estudo em dias de pena remidos, mede o impacto na linha do tempo e devolve parecer. O `criminal-master` acopla a peticao e o gate `suprema-corte-criminal`.

## Anexos obrigatorios (context/)
- `context/lep-7210-84.md` — buscar `Art. 126` a `Art. 130` (Secao IV — Da Remicao), `Art. 57` (referido pelo art. 127) e `Art. 112` (progressao); ler so a faixa, **a redacao NAO-tachada** (remicao = Lei 12.433/2011 + § 9 da Lei 15.402/2026).
- `context/jurisprudencia-criminal.md` — so itens marcados ✅; sumulas de remicao (perda de dias) sao 🟡, remeter a validacao.

## Objetivo
Quantificar com exatidao os dias de pena ja remidos (ou a remir), recalcular a data dos beneficios e entregar parecer fundamentado artigo a artigo — sem inventar numero nem percentual.

## Quando ativar
- Calcular ou conferir remicao por trabalho, estudo ou leitura.
- Saber quanto a remicao adianta a progressao ou o livramento.
- Falta grave ameaca dias ja remidos (perda de ate 1/3 — art. 127).
- Preparar atestado de remicao ou pedido em incidente de execucao.

## Metodologia
1. **Abrir a lei seca.** Buscar `Art. 126` no `context/lep-7210-84.md` e ler a redacao vigente (Lei 12.433/2011). Nunca de memoria.
2. **Trabalho — art. 126 § 1, II:** 1 dia de pena a cada **3 dias de trabalho** (razao 3:1). So conta jornada efetiva; preso impossibilitado por acidente continua a remir (art. 126 § 4).
3. **Estudo — art. 126 § 1, I:** 1 dia de pena a cada **12 horas de frequencia escolar**, **divididas no minimo em 3 dias**. Vale ensino fundamental, medio, profissionalizante, superior ou requalificacao, presencial ou EAD certificado (art. 126 § 2).
4. **Bonus de conclusao — art. 126 § 5:** o tempo remido por estudo e **acrescido de 1/3** quando o apenado conclui ensino fundamental, medio ou superior durante a pena, certificado pelo orgao competente.
5. **Cumulacao trabalho + estudo — art. 126 § 3:** as horas diarias de trabalho e de estudo sao compatibilizadas para somar as duas remicoes; conferir a redacao no arquivo antes de somar.
6. **Quem pode remir — art. 126 caput e § 6:** regime fechado e semiaberto remem por trabalho ou estudo; regime aberto, semiaberto e quem usufrui livramento condicional remem **por estudo** (§ 6). Regime domiciliar nao impede a remicao (art. 126 § 9, Lei 15.402/2026). Aplica-se a prisao cautelar (art. 126 § 7).
7. **Leitura e exames:** ⚠️ a remicao pela LEITURA e por aprovacao em EXAMES (ex.: ENEM/Encceja) **nao esta no art. 126** — decorre de ato normativo/CNJ e jurisprudencia. Citar so o que esta na LEP e **remeter a `validador-criminal`** para confirmar o ato vigente antes de somar; nao inventar razao de conversao.
8. **Falta grave — art. 127:** o juiz **podera revogar ate 1/3 (um terco)** do tempo remido (observado o art. 57), recomecando a contagem da infracao. Nao e perda automatica nem total (a redacao "perdera o direito ao tempo remido" esta TACHADA). ⚠️ Conferir o limite no arquivo; Sumula 9 STF (constitucionalidade da perda) e 🟡 — so apos `validador-criminal` + `anti-alucinacao-juridica`.
9. **Efeito — art. 128:** tempo remido = **pena cumprida para todos os efeitos** (progressao, livramento, indulto). Aplicar o total sobre o saldo e recalcular o proximo beneficio; a fracao de progressao (`Art. 112`, redacao 2026) vem de **`progressao-de-regime`**, nunca cravar percentual aqui.
10. **Declaracao — art. 126 § 8 e art. 129:** declarada pelo juiz, ouvidos MP e defesa; a administracao encaminha mensalmente o registro de dias de trabalho/horas de estudo (atestado).

## Saida obrigatoria
- **Dias remidos** discriminados: por trabalho (com a conta 3:1), por estudo (horas/12 + bonus de 1/3 se houve conclusao), por cumulacao — cada parcela com o artigo.
- **Impacto na linha do tempo:** nova data estimada de progressao e de livramento, com o saldo antes e depois da remicao (a fracao vem de `progressao-de-regime` / `livramento-condicional`).
- **Falta grave (se houver):** quanto pode ser revogado (ate 1/3) e novo marco a partir da infracao.
- **Parecer** com o fundamento legal artigo a artigo + ressalva sobre leitura/exames (pendente validacao) + lista de documentos do atestado.

## Guard
Nenhuma razao de conversao, percentual ou data entra sem `validador-criminal` (cruza `context/`). Leitura/exames e Sumula 9 STF: bloquear ate confirmar o ato/sumula vigente — nao citar de memoria. Percentual de progressao/livramento vem das skills proprias, nao deste calculo. Toda entrega fecha pela `suprema-corte-criminal` (R4 — calculo e forma).
