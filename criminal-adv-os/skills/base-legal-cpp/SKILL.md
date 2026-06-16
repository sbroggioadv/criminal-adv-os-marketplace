---
name: base-legal-cpp
description: "Porta de fundacao para o CODIGO DE PROCESSO PENAL (Decreto-Lei 3.689/41). Ensina a localizar o artigo por busca e ler a faixa, e alerta que o prazo PROCESSUAL penal conta diferente do prazo material: CPP 798 §1 EXCLUI o dia do comeco (nao se computa); CP 10 INCLUI o dia do comeco (prazo material). Use quando o operador disser artigo do CPP, procedimento, prazo processual penal, inquerito, prisao cautelar, nulidade, recurso, habeas corpus, juri, ou perguntar onde fica um dispositivo do processo penal."
---

# BASE-LEGAL-CPP — Porta para o Codigo de Processo Penal

> Camada 1 (fundacao enraizada). Esta skill NAO redige peca — ela aponta e ensina a navegar a lei seca do CPP, para que rito, prazo e cabimento saiam do arquivo, nunca da memoria de treino.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — Codigo de Processo Penal consolidado (~384KB, 852 artigos). **Localizar o artigo por busca ("Art. N") + ler a faixa**; nunca abrir o arquivo inteiro.

## Objetivo
Entregar o dispositivo processual exato (rito, requisito, prazo, cabimento de recurso/medida) na redacao VIGENTE, lido do arquivo, para que tempestividade, competencia e nulidade nao errem.

## Quando ativar
- Pergunta por artigo do CPP, procedimento, prazo processual penal, cabimento de medida ou recurso.
- Necessidade de localizar o rito da fase (investigacao, acao penal, prova, prisao, instrucao, recurso).
- Antes de qualquer skill de prazo/peca processual penal que dependa do dispositivo.

## Como navegar (regra de uso)
1. **Buscar** `Art. N` no `context/cpp-3689-41.md` e ler so a faixa do dispositivo + paragrafos.
2. **Mapa do CPP:** inquerito (4-23); acao penal (24-62); prova (155-250); prisoes e medidas cautelares (282-350); procedimentos (394-497), inclusive **juri (406-497)**; nulidades (563-573); recursos em geral (574-667); **habeas corpus (647-667)**; execucao = remissao residual a LEP.
3. **⚠️ Prazo PROCESSUAL penal = CPP 798 §1:** os prazos sao continuos e **NAO se computa o dia do comeco, inclui-se o do vencimento** (exclui o 1o dia — igual ao CPC nesse ponto). Prazo MATERIAL (prescricao/decadencia) = CP art. 10: o dia do comeco INCLUI-SE. Os dois contam de forma OPOSTA — identificar a natureza antes de contar. Para prazo, ler `Art. 798` (e 798-A suspensao) no arquivo antes de calcular.
4. **Ler a versao vigente:** trechos alterados (ex.: Pacote Anticrime, reformas 2024-2026) podem aparecer tachados — ler a redacao em vigor.

## Entrega obrigatoria final
- Numero do artigo + caput/paragrafo aplicavel + (se for prazo) a regra de contagem do CPP 798, transcritos do `context/cpp-3689-41.md`, prontos para a skill de prazo/peca usar.

## Guard
Nenhum rito, prazo ou cabimento entra em peca sem passar pelo `validador-criminal` (cruza o `context/`). Na duvida de contagem ou vigencia, bloquear e checar o arquivo; toda entrega fecha pela `suprema-corte-criminal`.
