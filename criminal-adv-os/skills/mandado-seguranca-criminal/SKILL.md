---
name: mandado-seguranca-criminal
description: "Mandado de seguranca no processo penal (Camada 6): protege direito liquido e certo lesado por ato de autoridade quando NAO cabe habeas corpus. Use para restituicao de coisa apreendida, acesso aos autos, atuacao do assistente, efeito suspensivo a recurso, ou quando o operador disser mandado de seguranca criminal, MS criminal, acesso aos autos, restituicao de coisa apreendida, direito liquido e certo penal."
---

# MANDADO-SEGURANCA-CRIMINAL

> Camada 6 (defesa, liberdade & investigacao). Remedio constitucional residual no processo penal — entra onde o habeas corpus nao alcanca, porque a questao NAO e liberdade de locomocao, mas um direito liquido e certo lesado por ato ilegal de autoridade.

## Anexos obrigatorios (context/)
- Diploma proprio: **Lei 12.016/2009** (rege o MS — direito liquido e certo, prova pre-constituida, prazo, liminar). Nao esta no CPP; citar como diploma autonomo e remeter o teor ao `validador-criminal`.
- `context/cpp-3689-41.md` — grep arts. 118-124 (restituicao de coisa apreendida) e 268-273 (assistente) quando o objeto for esse, e ler a faixa nao-tachada.
- `context/jurisprudencia-criminal.md` — so itens ✅. **Sumula Vinculante 14 (acesso do defensor aos elementos ja documentados na investigacao) NAO esta confirmada ✅ neste anexo — bloquear e conferir ao vivo pelo `validador-criminal` antes de citar.**

## Objetivo
Identificar o direito liquido e certo violado por ato de autoridade no curso da persecucao, confirmar que o caso nao e tutelavel por HC, e redigir o MS com prova pre-constituida e pedido de liminar, lastrado na Lei 12.016/2009.

## Quando ativar
- Ato de autoridade (delegado, juiz, MP) lesa direito do investigado/reu/ofendido e a questao nao e liberdade de locomocao.
- Negativa de acesso aos autos ou aos elementos ja documentados da investigacao; indeferimento de restituicao de coisa apreendida; recusa de atuacao do assistente; recurso sem efeito suspensivo a que se quer dar suspensao.
- O master pede a via residual depois de afastar o cabimento de HC e de recurso proprio.

## Metodologia
1. **Testar a via.** Confirmar que NAO cabe HC (a coacao nao recai sobre a liberdade de locomocao) nem ha recurso proprio com igual eficacia. Cruzar com `habeas-corpus` e com `competencia-criminal`.
2. **Direito liquido e certo (Lei 12.016/2009).** O MS protege direito liquido e certo, nao amparado por HC ou habeas data, lesado ou ameacado por ilegalidade/abuso de poder de autoridade. Exige **prova pre-constituida** (documental, sem dilacao) — montar o dossie probatorio.
3. **Objetos penais tipicos.** (a) **Restituicao de coisa apreendida** — arts. 118-120 do CPP (nao restituivel enquanto interessar ao processo; restituicao quando nao houver duvida sobre o direito do reclamante); o MS ataca o indeferimento ilegal. (b) **Acesso aos autos / elementos ja documentados** — direito de defesa; Sumula Vinculante 14 so apos ✅ do `validador-criminal`. (c) **Atuacao do assistente** — cruzar `assistente-de-acusacao` (arts. 268-273). (d) **Efeito suspensivo a recurso** que a lei nao lhe deu.
4. **Autoridade coatora e competencia.** Identificar a autoridade que praticou o ato e o orgao competente para o MS conforme a hierarquia (Lei 12.016/2009).
5. **Prazo decadencial.** O direito de impetrar MS extingue-se em **120 dias** contados da ciencia do ato impugnado (prazo decadencial da Lei 12.016/2009). Calcular o termo e cruzar com `prazos-processuais-penais`.
6. **Liminar.** Pedir liminar quando houver fundamento relevante e risco de ineficacia da medida (suspensao do ato), nos termos da Lei 12.016/2009.
7. **Pedido.** Concessao da ordem para anular/suspender o ato e impor a conduta devida (entregar a coisa, dar acesso, admitir o assistente).

## Entrega obrigatoria final
- MS criminal redigido com direito liquido e certo identificado + prova pre-constituida + autoridade coatora + competencia + prazo dos 120 dias + pedido de liminar e de ordem definitiva, lastrado na Lei 12.016/2009 (teor confirmado pelo validador) e no CPP onde aplicavel. Validado pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo, prazo ou jurisprudencia sem `validador-criminal` (cruza `context/`). Lei 12.016/2009 e diploma externo — confirmar teor antes de citar artigo; **Sumula Vinculante 14 so apos ✅ confirmado ao vivo** (ausente no anexo = bloqueia). Gate final obrigatorio `suprema-corte-criminal`. Na duvida sobre vigencia/redacao, ler a lei seca nao-tachada em `context/`.
