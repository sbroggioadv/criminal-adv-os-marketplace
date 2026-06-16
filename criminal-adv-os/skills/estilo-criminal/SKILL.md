---
name: estilo-criminal
description: "Padroniza a voz, a formatacao e a estrutura das pecas e pareceres penais do plugin: linguagem tecnica e sobria, defesa firme mas sem promessa de resultado, estrutura por peca (enderecamento, qualificacao, sintese, fundamentacao, pedidos), citacao correta de CP/CPP/LEP e jurisprudencia. Use ao redigir qualquer peca/parecer penal, ou quando o operador disser padroniza, estilo, formata a peca, como cito."
---

# ESTILO-CRIMINAL

> Tier 0 (transversal). Aplicado em toda peca/parecer/calculo penal, junto com a skill da tarefa.

## Anexos obrigatorios (context/)
- Nenhum direto (e estilo). A citacao de dispositivo sempre confere a redacao em `context/` via a skill da tarefa.

## Objetivo
Toda saida do plugin com a mesma voz: tecnica, objetiva, combativa na defesa, eticamente impecavel (OAB), sem prometer resultado.

## Padroes
1. **Voz:** afirmar a tese defensiva com firmeza; impugnar o que e da acusacao; nunca prometer absolvicao/resultado. Linguagem sobria, sem adjetivacao vazia.
2. **Estrutura da peca penal:** enderecamento correto (juizo/tribunal/relator) -> qualificacao -> sintese processual -> fundamentacao (preliminares/nulidades -> merito/tese -> jurisprudencia) -> pedidos claros e numerados.
3. **Citacao:** "art. N do CP/CPP/LEP" (conferida na redacao vigente em context/); jurisprudencia so com ✅ no anexo (orgao + numero/tema). Nunca citar lei revogada como vigente.
4. **Calculo (Motor Temporal):** apresentar como linha do tempo + marcos + fundamento artigo a artigo + resultado + parecer conclusivo — auditavel.
5. **Fecho:** ressalva de que a responsabilidade tecnica e a assinatura sao do advogado.

## Entrega obrigatoria final
- A peca/parecer na voz e estrutura padrao, pronta para a `suprema-corte-criminal`.

## Guard
Sem promessa de resultado (OAB). Sem dado de cliente real no plugin. Citacao so com a redacao vigente conferida em context/ + validador-criminal.
