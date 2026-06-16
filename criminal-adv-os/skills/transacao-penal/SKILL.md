---
name: transacao-penal
description: "Pleiteia a transacao penal no JECrim (Lei 9.099/1995 art. 76) para infracao de menor potencial ofensivo: aplicacao imediata de pena restritiva/multa sem denuncia e sem reincidencia, sempre conferindo o teor da lei. Use quando o operador disser transacao penal, juizado especial criminal, JECrim, menor potencial ofensivo, ou pena alternativa sem processo."
---

# TRANSACAO-PENAL

> Camada 5 (acordos & despenalizacao). Saida do JECrim — pena restritiva/multa aplicada de imediato, SEM denuncia e SEM gerar reincidencia. Foco DEFESA: obter a transacao na menor pena possivel.

## Anexos obrigatorios (context/)
- `context/lei-9099-95.md` — lei seca da Lei 9.099/1995 (recorte criminal). **grep** "Art. 61" e "Art. 76" (caput + §§ 1-6) e ler a faixa na redacao VIGENTE. ✅ capturada do Planalto (2026-06-16).
- `context/penal-especial.md` — bloco 3 (despenalizacao / ANPP nao se aplica quando cabivel transacao — §2, I do art. 28-A).
- `context/jurisprudencia-criminal.md` — so citar item ✅; o que nao constar = 🟡. (Sumulas/teses sobre transacao = ainda 🟡: confirmar ao vivo no `validador-criminal`.)

## Objetivo
Verificar se a infracao e de menor potencial ofensivo, viabilizar a proposta de transacao penal do MP na pena menos onerosa e proteger o cliente dos efeitos (nao reincidencia, nao maus antecedentes), conferindo o teor da Lei 9.099.

## Quando ativar
- Infracao de **menor potencial ofensivo** (contravencao ou crime com pena maxima nao superior a 2 anos) — JECrim.
- "Cabe transacao?" / "pena alternativa sem virar processo"; ou conferir proposta ja apresentada (evitar pena desproporcional).
- Distinguir transacao (antes da denuncia) de `suspensao-condicional-processo` e de `anpp`.

## Metodologia (ARTIGOS REAIS — grep a lei seca em context/lei-9099-95.md)
1. **Competencia / conceito (Lei 9.099/1995 art. 61):** infracao de **menor potencial ofensivo** = contravencoes penais e crimes com **pena maxima nao superior a 2 anos**, cumulada ou nao com multa (redacao Lei 11.313/2006). Ler o teor do art. 61 em `context/lei-9099-95.md`.
2. **Transacao penal (Lei 9.099/1995 art. 76):** o MP, ao inves de oferecer denuncia, **propoe a aplicacao imediata de pena restritiva de direitos ou multa**, aceita pela defesa e homologada pelo juiz. **Nao ha processo de conhecimento nem analise de culpa.** Ler o art. 76 (caput + §§ 1-6) em `context/lei-9099-95.md`.
3. **Efeitos favoraveis ao cliente:** a transacao **nao gera reincidencia** (so impede novo beneficio por **5 anos**); **nao consta para maus antecedentes** civis; nao importa reconhecimento de culpa. Esses efeitos sao a razao de pleitea-la — explicitar no parecer.
4. **Negociar a pena:** a defesa atua para que a pena restritiva/multa seja a menos onerosa (valor da multa, modalidade da restritiva, prazo). Verificar requisitos negativos legais (nao ter sido condenado por crime a pena privativa de liberdade; nao ter recebido transacao nos 5 anos; antecedentes/conduta favoraveis) — conferir o art. 76 e seus paragrafos no validador.
5. **Descumprimento:** **Sumula Vinculante 35 do STF** — a homologacao da transacao **nao faz coisa julgada material**; descumprido o acordo, retoma-se a persecucao (oferecimento de denuncia). Referencia nas notas de `context/lei-9099-95.md`; **confirmar numero/teor da SV ao vivo no `validador-criminal`** antes de citar em peca.
6. **Limites de fronteira:** transacao e do JECrim (menor potencial ofensivo); se pena minima inferior a 4 anos mas fora do JECrim e ha confissao, rotear `anpp`; se ja ha denuncia recebida e pena minima ate 1 ano, rotear `suspensao-condicional-processo`.

## Entrega obrigatoria final
Parecer de cabimento (menor potencial ofensivo + requisitos do art. 76) + proposta de pena restritiva/multa menos onerosa + nota sobre efeitos (nao reincidencia / impede novo beneficio por 5 anos) + minuta da manifestacao + fundamento + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Lei seca (arts. 61, 76) agora em `context/lei-9099-95.md` — **ler a faixa, nunca de memoria**. Sumulas/teses (incl. SV 35) ainda passam pelo `validador-criminal` antes de citar (jurisprudencia so se ✅). Na duvida, bloquear e checar. Gate final `suprema-corte-criminal`.

transacao-penal -> arts. citados: Lei 9.099/1995 art. 61 (menor potencial ofensivo), art. 76 (transacao penal) — lei seca em context/lei-9099-95.md. Cross-link: anpp (CPP 28-A §2,I), suspensao-condicional-processo.
