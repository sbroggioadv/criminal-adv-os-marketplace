---
name: estrategia-penal
description: "Define o NORTE da defesa (Camada 2, metodologica): mapeia as teses defensivas possiveis e escolhe a melhor combinacao por fase — atipicidade, negativa de autoria, excludentes de ilicitude e de culpabilidade, desclassificacao, causas de diminuicao, nulidades, prescricao. Fixa a tese principal + subsidiarias + o caminho processual. Use quando o operador disser estrategia, qual tese, linha de defesa, como defendo, tese principal, melhor caminho, acordo ou defesa."
---

# ESTRATEGIA-PENAL

> Camada 2 (metodologica). Define o norte: qual tese sustentar, em que ordem, e por qual caminho processual. Roda no inicio e a cada virada de fase, antes de qualquer peca.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — grep os artigos das teses (23 a 28, 21, 22) e ler a faixa nao-tachada.
- `context/cpp-3689-41.md` — ritos e nulidades (sob demanda).
- `context/jurisprudencia-criminal.md` — so itens ✅ (atipicidade material / insignificancia, reconhecimento Tema 1.016 etc.).
- `context/metodologia-criminal.md` — fluxo da persecucao e regras de ouro.

## Objetivo
Escolher, entre as teses cabiveis, a combinacao que melhor protege o reu — uma tese principal forte, subsidiarias em escada, e o caminho processual (acordo, defesa, recurso ou HC) mais favoravel a fase atual.

## Quando ativar
- Novo caso ou virada de fase (recebimento da denuncia, instrucao, sentenca, recurso).
- O operador pergunta qual tese sustentar, como defender ou qual caminho seguir.
- Antes de redigir resposta a acusacao, alegacoes finais, HC ou recurso.

## Metodologia
1. **Quadro factico e probatorio.** Cruzar fatos x prova (apoio em `cadeia-de-custodia-e-provas`) para saber o que e atacavel.
2. **Mapear teses cabiveis:**
   - **Atipicidade** formal ou material — principio da insignificancia/bagatela (jurisprudencia ✅ em `context/`).
   - **Negativa de autoria** — quando o elo probatorio (ex.: reconhecimento sem o rito do art. 226 do CPP) e fragil.
   - **Excludentes de ilicitude (art. 23 do CP):** estado de necessidade (art. 24), legitima defesa (art. 25), estrito cumprimento de dever legal ou exercicio regular de direito (art. 23, III).
   - **Excludentes/causas de exclusao da culpabilidade:** inimputabilidade (art. 26), menoridade penal (art. 27), erro de proibicao (art. 21 — isenta se inevitavel, diminui se evitavel), coacao moral irresistivel (art. 22), embriaguez completa fortuita (art. 28, § 1º).
   - **Desclassificacao** (tipo menos grave), **causas de diminuicao**, **nulidades** (com `nulidades-penais`), **prescricao/extincao da punibilidade**.
3. **Selecionar a tese principal** — a de maior chance de exito + menor risco — e ordenar as **subsidiarias** em escada (ex.: principal atipicidade; subsidiaria 1 desclassificacao; subsidiaria 2 atenuacao na dosimetria).
4. **Definir o caminho processual.** Avaliar despenalizacao/acordo (ANPP, transacao, suspensao) x defesa de merito x recurso x HC, conforme a fase e a situacao prisional.
5. **Verificar coerencia.** A tese principal nao pode contradizer a subsidiaria de forma que enfraqueca ambas; alinhar com a `memoria-de-caso-criminal`.

## Entrega obrigatoria final
- Plano de defesa: tese principal + subsidiarias em ordem + caminho processual escolhido + fundamento legal artigo a artigo de cada tese + proximo passo. Validado pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo ou jurisprudencia sem `validador-criminal` (cruza `context/`). Jurisprudencia so com ✅ — 🟡/ausente bloqueia ate confirmar. Numero de artigo/percentual sempre conferido na lei seca nao-tachada (atencao a vigencia 2024-2026). Gate final obrigatorio `suprema-corte-criminal`.
