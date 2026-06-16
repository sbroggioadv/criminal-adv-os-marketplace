---
name: habeas-corpus
description: "O writ da liberdade na defesa penal (Camada 6): cabimento, hipoteses de coacao ilegal, liberatorio x preventivo, liminar, competencia e procedimento. Use ao atacar prisao ou constrangimento ilegal, ou quando o operador disser habeas corpus, HC, trancar a acao, constrangimento ilegal, excesso de prazo, salvo-conduto, prisao ilegal, tranca-acao."
---

# HABEAS-CORPUS

> Camada 6 (defesa, liberdade & investigacao). O writ da liberdade — remedio constitucional contra coacao ilegal a liberdade de locomocao. Acao autonoma de impugnacao, sem prazo, gratuita, sem advogado obrigatorio.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — grep arts. 647-667 e ler a faixa nao-tachada (cabimento, hipoteses, competencia, procedimento).
- `context/jurisprudencia-criminal.md` — so itens ✅ (Tema 1.016 STJ sobre reconhecimento; Sumula Vinculante 56; ADC 43/44/54 — execucao provisoria).
- `context/metodologia-criminal.md` — fluxo da persecucao e regras de ouro.

## Objetivo
Diagnosticar a coacao ilegal a liberdade de locomocao do cliente, escolher a via (liberatorio ou preventivo), encaixar a hipotese legal e redigir o HC com pedido de liminar e ordem definitiva, lastrado artigo a artigo.

## Quando ativar
- Cliente preso ou na iminencia de prisao por ato sem fundamento legal (prisao ilegal, excesso de prazo, ameaca de coacao).
- Acao penal sem justa causa ou processo manifestamente nulo, a ser trancado.
- O master pede a impugnacao da liberdade antes/junto de outra peca (resposta a acusacao, recurso).

## Metodologia
1. **Mapear a coacao.** Quem e o paciente, quem e a autoridade coatora, qual o ato (prisao, processo, ameaca) e a fase. Cruzar com `competencia-criminal` (qual tribunal/juizo julga o HC) e `cronologia-penal-e-providencias`.
2. **Cabimento (art. 647 do CPP).** Cabe HC sempre que alguem sofrer ou se achar na iminencia de sofrer violencia ou coacao ilegal na liberdade de ir e vir, salvo punicao disciplinar. **De oficio:** art. 647-A (incluido pela Lei 14.836/2024) — qualquer autoridade judicial pode expedir ordem, individual ou coletiva.
3. **Encaixar a hipotese de coacao ILEGAL (art. 648 do CPP):** I — falta de justa causa; II — preso por mais tempo do que a lei determina (excesso de prazo); III — quem ordenou a coacao nao tinha competencia; IV — cessado o motivo que autorizou a coacao; V — nao admissao a prestar fianca quando cabivel; VI — processo manifestamente nulo; VII — extinta a punibilidade.
4. **Definir a via.** **Liberatorio** quando a coacao ja se concretizou (pede-se a soltura/alvara). **Preventivo** quando ha so ameaca concreta (pede-se **salvo-conduto** — art. 660, § 4º, do CPP).
5. **Competencia (arts. 650-651 do CPP).** Identificar o orgao competente conforme a autoridade coatora (art. 650); a competencia do juiz cessa se a coacao provier de autoridade de igual ou superior jurisdicao (art. 650, § 1º). A concessao do HC nao poe termo ao processo, salvo conflito com seus fundamentos (art. 651).
6. **Liminar.** A liminar em HC e construcao jurisprudencial (sem artigo proprio no CPP) — pedir pelo risco a liberdade e plausibilidade do direito. Marcar para o `validador-criminal` antes de citar precedente.
7. **Teses defensivas tipicas.** Trancamento por atipicidade / falta de justa causa (art. 648, I); excesso de prazo (art. 648, II); nulidade (art. 648, VI) — incluindo reconhecimento fora do rito do art. 226 (**Tema 1.016 STJ ✅**); extincao da punibilidade (art. 648, VII). Preventiva sem fundamentacao concreta: cruzar com `liberdade-provisoria-e-preventiva`.
8. **Procedimento (arts. 656-667 do CPP).** Estruturar peticao com o conteudo do art. 654, § 1º (nome do paciente, coator, especie de constrangimento, assinatura) e o rito de informacoes/decisao (arts. 656, 660, 664).

## Entrega obrigatoria final
- HC redigido (liberatorio ou preventivo) com hipotese do art. 648 + via + competencia + pedido de liminar + ordem definitiva (alvara de soltura ou salvo-conduto), com fundamento artigo a artigo e jurisprudencia ✅. Validado pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo, percentual ou jurisprudencia sem `validador-criminal` (cruza `context/`). Jurisprudencia/liminar so com ✅ em `context/jurisprudencia-criminal.md` — 🟡/ausente bloqueia ate confirmar ao vivo. Gate final obrigatorio `suprema-corte-criminal`. Na duvida sobre vigencia/redacao, ler a lei seca nao-tachada em `context/`.
