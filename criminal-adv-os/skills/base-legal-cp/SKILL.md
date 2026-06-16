---
name: base-legal-cp
description: "Porta de fundacao para o CODIGO PENAL (Decreto-Lei 2.848/40). Ensina a localizar o artigo por busca e ler a faixa certa, sem despejar a lei inteira nem citar de cabeca. Use quando o operador disser artigo do CP, tipo penal, parte geral, qual a pena do crime X, qualificadora, agravante, imputabilidade, ou perguntar onde fica determinado dispositivo do Codigo Penal."
---

# BASE-LEGAL-CP — Porta para o Codigo Penal

> Camada 1 (fundacao enraizada). Esta skill NAO redige peca — ela aponta e ensina a navegar a lei seca do CP, para que a tipicidade e a pena saiam do arquivo, nunca da memoria de treino.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — Codigo Penal consolidado (~388KB, 387 artigos). **Localizar o artigo por busca ("Art. N") + ler a faixa**; nunca abrir o arquivo inteiro.

## Objetivo
Entregar o dispositivo penal exato (tipo, pena cominada, qualificadora, causa de aumento/diminuicao, regra da Parte Geral) na redacao VIGENTE, lido do arquivo, para alimentar tipicidade, dosimetria e prescricao com base segura.

## Quando ativar
- Pergunta por artigo do CP, tipo penal, pena de um crime, qualificadora ou causa de aumento.
- Necessidade de regra da Parte Geral: aplicacao da lei penal, crime, dolo/culpa, imputabilidade, concurso, pena, prescricao.
- Antes de qualquer skill de redacao/calculo que dependa de tipicidade ou da pena cominada.

## Como navegar (regra de uso)
1. **Buscar** `Art. N` no `context/cp-2848-40.md` e ler so a faixa do dispositivo + paragrafos.
2. **Mapa do CP:**
   - **Parte Geral (arts. 1-120):** aplicacao da lei penal, do crime, imputabilidade, concurso de pessoas, das penas, medidas de seguranca, acao penal, extincao da punibilidade (prescricao 109-118).
   - **Parte Especial (arts. 121-361):** os tipos penais por bem juridico (vida, patrimonio, dignidade sexual, fe publica, administracao publica etc.).
3. **Pontos vivos 2024-2026 (conferir no arquivo, nao de cabeca):** feminicidio = crime AUTONOMO no **art. 121-A** (Lei 14.994/2024), nao mais qualificadora; **art. 121-B** vicaricidio (Lei 15.384/2026). Conferir a redacao nao-tachada antes de citar.
4. **Ler a versao vigente:** dispositivos alterados podem ter trechos tachados no compilado — ler a redacao em vigor.

## Entrega obrigatoria final
- Numero do artigo + caput/paragrafo/inciso aplicavel + pena cominada, transcritos do `context/cp-2848-40.md`, com nota de vigencia quando houver alteracao recente — pronto para a skill de tipicidade/dosimetria usar.

## Guard
Nenhum tipo penal, pena ou qualificadora entra em peca sem passar pelo `validador-criminal` (cruza o `context/`). Na duvida de vigencia/existencia, bloquear e checar a redacao nao-tachada no arquivo; toda entrega fecha pela `suprema-corte-criminal`.
