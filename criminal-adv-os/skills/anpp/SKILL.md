---
name: anpp
description: "Pleiteia o Acordo de Nao Persecucao Penal (CPP art. 28-A, Lei 13.964/2019) para evitar a denuncia: confere requisitos, condicoes, vedacoes e homologacao, sempre com a lei seca aberta. Use quando o operador disser ANPP, acordo de nao persecucao, art. 28-A, evitar a denuncia, acordo penal, ou perguntar se cabe acordo antes do processo."
---

# ANPP

> Camada 5 (acordos & despenalizacao). Acordo de nao persecucao penal — porta de saida ANTES da denuncia. Foco DEFESA: pleitear o ANPP quando cabivel e na melhor condicao para o cliente.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — **grep** art. 28-A (caput, incisos I-V, §§ 1 a 14). O numero pode quebrar de linha — ler a faixa.
- `context/penal-especial.md` — bloco 3 (Pacote Anticrime / ANPP ✅ vigente, ADIs 6.298).
- `context/jurisprudencia-criminal.md` — so citar item ✅ (ANPP art. 28-A esta ✅).

## Objetivo
Verificar se o caso comporta ANPP, montar a proposta nas condicoes menos onerosas ao cliente e conduzir ate a homologacao judicial e a extincao da punibilidade — sem deixar o caso virar denuncia quando ha solucao consensual.

## Quando ativar
- Investigado confessou (ou pode confessar) crime sem violencia/grave ameaca, ainda na fase pre-processual.
- "Da pra fazer acordo antes de virar processo?" / "evitar a denuncia".
- MP nao ofereceu ANPP e o caso parece cabivel (remessa ao orgao superior); ou conferir proposta ja apresentada (evitar condicao abusiva).

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Requisitos cumulativos (art. 28-A caput):** (a) **nao ser caso de arquivamento**; (b) **confissao formal e circunstanciada** da infracao perante o MP; (c) infracao **sem violencia ou grave ameaca**; (d) **pena minima inferior a 4 anos**; (e) acordo necessario e suficiente para reprovacao e prevencao. **§1: a pena minima considera as causas de aumento e diminuicao aplicaveis ao caso** (calcular, nao olhar so o preceito secundario seco) — passar pelo `motor-calculo-de-pena`.
2. **Condicoes (incisos I a V — ajustadas cumulativa e alternativamente):** I reparar o dano/restituir a coisa (salvo impossibilidade); II renunciar voluntariamente a bens e direitos (instrumento/produto/proveito); III prestar servico a comunidade por periodo correspondente a pena minima diminuida de 1 a 2/3 (art. 46 CP); IV pagar prestacao pecuniaria (art. 45 CP); V outra condicao proporcional e compativel indicada pelo MP. **Defesa: negociar a combinacao menos onerosa.**
3. **Vedacoes (§2, I a IV):** I cabivel **transacao penal** (JECrim — rotear `transacao-penal`); II reincidente ou conduta criminal habitual/reiterada/profissional (salvo infracoes pretretitas insignificantes); III ter sido beneficiado nos **5 anos** anteriores por ANPP, transacao penal ou suspensao condicional do processo; IV crime no ambito de **violencia domestica/familiar** ou contra a mulher por razoes de genero, em favor do agressor. Conferir cada vedacao no caso.
4. **Forma e homologacao (§§3-9):** §3 acordo escrito firmado por MP + investigado + defensor; §4 audiencia em que o juiz verifica voluntariedade (oitiva na presenca do defensor) e legalidade; §5 condicoes inadequadas/insuficientes/abusivas -> devolve ao MP para reformular; §§6-7 homologado, segue ao juizo de execucao; §8 recusada a homologacao, volta ao MP; §9 vitima intimada da homologacao e do descumprimento.
5. **Descumprimento (§§10-12):** §10 descumpridas as condicoes, o MP comunica ao juizo para **rescisao e posterior denuncia**; §11 pode justificar o nao oferecimento de suspensao condicional do processo; §12 o ANPP **nao consta** em certidao de antecedentes (salvo §2, III).
6. **Cumprimento integral (§13)** -> juizo decreta a **extincao da punibilidade** (rotear `extincao-da-punibilidade`). **MP recusa indevida (§14):** investigado pode requerer **remessa dos autos ao orgao superior** (art. 28 CPP) — instrumento de defesa quando o caso e cabivel.

## Entrega obrigatoria final
Parecer de cabimento (requisitos § a §) + proposta de condicoes na combinacao menos onerosa + minuta do requerimento (proposta de ANPP ou remessa ao orgao superior pelo §14) + fundamento artigo a artigo + handoff ao `criminal-master`. Passa pela `suprema-corte-criminal`.

## Guard
Nenhum dispositivo/percentual/calculo sai sem `validador-criminal` (cruza `context/`). Pena minima do caput sempre calculada com as causas do §1, nunca de cabeca. Conferir cada vedacao do §2 antes de afirmar cabimento. Jurisprudencia so se ✅. Na duvida, bloquear e reler o art. 28-A. Gate final `suprema-corte-criminal`.

anpp -> arts. citados: CPP 28-A (caput; I-V; §§ 1, 2 [I-IV], 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14), 28; CP 45, 46.
