---
name: transacao-penal
description: "Pleiteia a transacao penal no JECrim (Lei 9.099/1995 art. 76) para infracao de menor potencial ofensivo: aplicacao imediata de pena restritiva/multa sem denuncia e sem reincidencia, sempre conferindo o teor da lei. Use quando o operador disser transacao penal, juizado especial criminal, JECrim, menor potencial ofensivo, ou pena alternativa sem processo."
---

# TRANSACAO-PENAL

> Camada 5 (acordos & despenalizacao). Saida do JECrim — pena restritiva/multa aplicada de imediato, SEM denuncia e SEM gerar reincidencia. Foco DEFESA: obter a transacao na menor pena possivel.

## Anexos obrigatorios (context/)
- `context/penal-especial.md` — bloco 3 (despenalizacao / ANPP nao se aplica quando cabivel transacao — §2, I do art. 28-A).
- `context/jurisprudencia-criminal.md` — so citar item ✅; o que nao constar = 🟡.
- ⚠️ **A Lei 9.099/1995 NAO esta na lei seca local (CP/CPP/LEP).** Teor dos arts. 61 e 76 e das sumulas deve ser **confirmado ao vivo no `validador-criminal`** antes de citar numero/redacao em peca — anti-alucinacao.

## Objetivo
Verificar se a infracao e de menor potencial ofensivo, viabilizar a proposta de transacao penal do MP na pena menos onerosa e proteger o cliente dos efeitos (nao reincidencia, nao maus antecedentes), conferindo o teor da Lei 9.099.

## Quando ativar
- Infracao de **menor potencial ofensivo** (contravencao ou crime com pena maxima nao superior a 2 anos) — JECrim.
- "Cabe transacao?" / "pena alternativa sem virar processo"; ou conferir proposta ja apresentada (evitar pena desproporcional).
- Distinguir transacao (antes da denuncia) de `suspensao-condicional-processo` e de `anpp`.

## Metodologia (ARTIGOS REAIS — conferir no validador, lei nao esta em context/)
1. **Competencia / conceito (Lei 9.099/1995 art. 61):** infracao de **menor potencial ofensivo** = contravencoes penais e crimes com **pena maxima nao superior a 2 anos**, cumulada ou nao com multa. Confirmar o teor do art. 61 no `validador-criminal` antes de citar.
2. **Transacao penal (Lei 9.099/1995 art. 76):** o MP, ao inves de oferecer denuncia, **propoe a aplicacao imediata de pena restritiva de direitos ou multa**, aceita pela defesa e homologada pelo juiz. **Nao ha processo de conhecimento nem analise de culpa.**
3. **Efeitos favoraveis ao cliente:** a transacao **nao gera reincidencia** (so impede novo beneficio por **5 anos**); **nao consta para maus antecedentes** civis; nao importa reconhecimento de culpa. Esses efeitos sao a razao de pleitea-la — explicitar no parecer.
4. **Negociar a pena:** a defesa atua para que a pena restritiva/multa seja a menos onerosa (valor da multa, modalidade da restritiva, prazo). Verificar requisitos negativos legais (nao ter sido condenado por crime a pena privativa de liberdade; nao ter recebido transacao nos 5 anos; antecedentes/conduta favoraveis) — conferir o art. 76 e seus paragrafos no validador.
5. **Descumprimento:** o efeito do descumprimento (em regra, prosseguimento com oferecimento da denuncia) **nao e pacifico** — **conferir a jurisprudencia no `validador-criminal`** (ha entendimento do STF/STJ sobre o que ocorre quando a pena transacionada nao e cumprida). Nao afirmar de cabeca; tratar como 🟡 ate confirmar.
6. **Limites de fronteira:** transacao e do JECrim (menor potencial ofensivo); se pena minima inferior a 4 anos mas fora do JECrim e ha confissao, rotear `anpp`; se ja ha denuncia recebida e pena minima ate 1 ano, rotear `suspensao-condicional-processo`.

## Entrega obrigatoria final
Parecer de cabimento (menor potencial ofensivo + requisitos do art. 76) + proposta de pena restritiva/multa menos onerosa + nota sobre efeitos (nao reincidencia / impede novo beneficio por 5 anos) + minuta da manifestacao + fundamento + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Lei 9.099/1995 e sumulas NAO estao em context/ — **nenhum numero/teor de artigo ou sumula sai sem confirmacao ao vivo no `validador-criminal`**. Efeito do descumprimento = 🟡 (conferir antes de afirmar). Jurisprudencia so se ✅. Na duvida, bloquear e checar. Gate final `suprema-corte-criminal`.

transacao-penal -> arts. citados: Lei 9.099/1995 art. 61 (menor potencial ofensivo), art. 76 (transacao penal) — teor confirmado no validador-criminal (lei fora de context/). Cross-link: anpp (CPP 28-A §2,I), suspensao-condicional-processo.
