---
name: prescricao-penal
description: "Calcula a prescricao penal (pretensao punitiva e executoria) com calculo fundamentado artigo a artigo — NUNCA numero de cabeca: tabela do art. 109, termo inicial, causas suspensivas e interruptivas, reducao pela metade e prescricao da multa. Use quando o operador disser prescricao, prescreveu?, calcular prescricao, extincao pela prescricao, prescricao retroativa, intercorrente ou executoria."
---

# PRESCRICAO-PENAL

> Camada 3 (motor penal temporal). A skill mais sensivel: errar prescricao sob OAB e catastrofe. Foco DEFESA. TODO marco vem de `grep` na lei seca — zero numero de memoria.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep CADA artigo** (107, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119) e ler a faixa. O numero pode quebrar de linha — ler o paragrafo inteiro.
- `context/penal-especial.md` + handoff `base-legal-penal-especial` — prescricao em crimes falimentares/tributarios/legislacao especial.
- `context/jurisprudencia-criminal.md` — so citar item ✅ (ex.: Sumula 438 STJ esta 🟡 — conferir antes).

## Objetivo
Dizer se a punibilidade foi extinta pela prescricao e dar o calculo auditavel: linha do tempo de TODOS os marcos + fundamento artigo a artigo + parecer conclusivo.

## Quando ativar
- "Prescreveu?" / "calcular prescricao" / "ja prescreveu o crime?".
- Tese de extincao pela prescricao em resposta a acusacao, alegacoes finais ou HC.
- Prescricao retroativa, superveniente (intercorrente), executoria, da multa, em medida de seguranca ou em lei especial.

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Classificar a especie ANTES de calcular** — muda a base e o termo inicial:
   - **PPP em ABSTRATO (art. 109):** antes do transito, pela **pena MAXIMA cominada**. **Ler a TABELA do anexo (incisos I a VI) e usa-la** — NAO decorar: superior a 12 -> 20 anos; >8 a 12 -> 16; >4 a 8 -> 12; >2 a 4 -> 8; de 1 a 2 -> 4; inferior a 1 -> 3 (redacao Lei 12.234/2010). Paragrafo unico: penas restritivas de direito seguem os mesmos prazos.
   - **PPP superveniente/intercorrente e RETROATIVA (art. 110):** apos o transito **para a acusacao** (ou improvido seu recurso), pela **pena APLICADA** (concreta). **§1: a prescricao regulada pela pena aplicada NAO pode ter termo inicial anterior a denuncia/queixa** (Lei 12.234/2010). ⚠️ **§2 foi REVOGADO pela Lei 12.234/2010 — a prescricao retroativa para periodo ANTERIOR ao recebimento da denuncia continua VEDADA; conferir a redacao tachada no anexo.** Reincidente: prazo do art. 109 aumentado de 1/3 (so na executoria — caput do 110).
   - **PPE (executoria, art. 110 c/c art. 112):** apos o transito definitivo, pela **pena aplicada**.
2. **Termo inicial da PPP (art. 111 — grep e ler I a V):** I consumacao; II tentativa = cessada a atividade; III permanente = cessada a permanencia; IV bigamia/falso registro = fato conhecido; V crimes sexuais/violencia contra crianca = vitima completar 18 (salvo acao ja proposta — Lei 14.344/2022).
3. **Termo inicial da PPE (art. 112 do CP — NAO confundir com art. 112 da LEP!):** I transito para a acusacao, ou revogacao do sursis/livramento; II interrupcao da execucao (salvo tempo computado na pena).
4. **Evasao/revogacao (art. 113):** evadindo-se o condenado ou revogado o livramento, a prescricao regula-se pelo **tempo que RESTA da pena**.
5. **Prescricao da multa (art. 114):** I 2 anos se unica; II mesmo prazo da PPL se alternativa/cumulativa.
6. **Reducao pela METADE (art. 115):** prazos reduzidos de metade se o agente era **menor de 21 ao tempo do crime** OU **maior de 70 na data da sentenca** — **salvo se o crime envolver violencia sexual contra a mulher** (redacao Lei 15.160/2025 — grep e ler a NAO-tachada). Aplicar a reducao ANTES de comparar com o intervalo entre marcos.
7. **Causas SUSPENSIVAS (art. 116 — nao corre):** I questao prejudicial em outro processo; II pena cumprida no exterior; III pendencia de ED/recurso a Tribunais Superiores inadmissiveis; IV ANPP nao cumprido/nao rescindido (II-IV pela Lei 13.964/2019). Paragrafo unico: apos o transito, nao corre enquanto preso por outro motivo.
8. **Causas INTERRUPTIVAS (art. 117, incisos I-VI — zera e recomeca):** I recebimento da denuncia/queixa; II pronuncia; III decisao confirmatoria da pronuncia; IV publicacao de sentenca/acordao condenatorios recorriveis; V inicio/continuacao do cumprimento; VI reincidencia. §2: interrompida, todo o prazo recomeca do dia da interrupcao (salvo inciso V).
9. **Concurso (art. 118-119):** penas mais leves prescrevem com as mais graves (118); em concurso de crimes a extincao incide sobre a pena de **cada um, isoladamente** (119).
10. **Medida de seguranca / lei especial:** prazo segue a pena cominada ao fato (CP 109); falimentar/tributario/legislacao especial tem marcos proprios -> remeter a `base-legal-penal-especial` antes de fixar prazo.
11. **Montar a linha do tempo:** termo inicial (111 ou 112) -> aplicar reducao 115 se cabivel -> marcar cada interruptiva (117) e cada suspensiva (116) -> medir o maior intervalo entre dois marcos contra o prazo (109/110) -> concluir. Prescricao virtual/em perspectiva pela pena minima NAO e admitida (Sumula 438 STJ — 🟡, conferir antes de citar).

## Saida obrigatoria
1. **Linha do tempo** com TODOS os marcos datados (fato/consumacao · recebimento · pronuncia/confirmatoria se houver · publicacao da sentenca · transito p/ acusacao · transito definitivo) e os intervalos entre eles.
2. **Marcos** classificados (interruptivo art. 117 / suspensivo art. 116 / termo inicial 111-112).
3. **Calculo fundamentado** — especie (PPP abstrata/retroativa/superveniente ou PPE), base usada (pena maxima 109 ou aplicada 110), prazo da tabela, reducao 115 se aplicada, com o artigo a artigo.
4. **Parecer conclusivo:** prescreveu (qual especie, em qual intervalo) ou nao prescreveu (faltam quantos anos/meses), com a peca/tese recomendada.
5. Handoff ao `criminal-master`; passa pela `suprema-corte-criminal`.

## Guard
Nenhum prazo/marco sai sem `validador-criminal` (cruza `context/`) — todo numero vem de `grep` no CP, nunca de memoria. Jurisprudencia so se ✅ (Sumula 438 = 🟡, conferir). Especie ou termo inicial em duvida: bloquear e reler a lei seca. Calculo penal sob OAB = catastrofe se errado — na duvida, bloquear. Gate final `suprema-corte-criminal` (R4 refaz o calculo).

prescricao-penal -> arts. citados: CP 107 IV, 109 (I-VI), 110 (§§1, 2-revogado), 111 (I-V), 112 (I-II — do CP, nao da LEP), 113, 114 (I-II), 115 (Lei 15.160/2025), 116 (I-IV), 117 (I-VI, §2), 118, 119; Sumula 438 STJ (🟡).
