---
name: decadencia-perempcao
description: "Verifica decadencia e perempcao (e renuncia, perdao do ofendido e perdao judicial) como causas de extincao da punibilidade, com fundamento artigo a artigo — NUNCA prazo de cabeca. Use quando o operador disser decadencia, perempcao, perdi o prazo da queixa, renuncia, perdao do ofendido ou perdao judicial."
---

# DECADENCIA-PEREMPCAO

> Camada 3 (motor penal temporal). Causas de extincao da punibilidade na acao penal privada e na de iniciativa condicionada. TODO prazo vem de `grep` na lei seca. Foco DEFESA.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — **grep** art. 103 (decadencia), 104 (renuncia), 105-106 (perdao do ofendido), 107 (rol — IV decadencia/perempcao, V renuncia/perdao, IX perdao judicial), 120 (perdao judicial). Ler a faixa.
- `context/cpp-3689-41.md` — **grep** art. 38 (decadencia), 49-51 (renuncia/perdao), 58-59 (aceitacao do perdao), 60 (perempcao). O numero pode quebrar de linha.
- `context/jurisprudencia-criminal.md` — so citar item ✅.

## Objetivo
Dizer se ocorreu decadencia ou perempcao (ou renuncia/perdao) e dar o calculo/verificacao auditavel + o fundamento + o parecer conclusivo de extincao.

## Quando ativar
- "Perdi o prazo da queixa?" / "decaiu o direito?" / "ainda da tempo de queixar?".
- Suspeita de perempcao em acao penal privada em curso.
- Renuncia (expressa/tacita), perdao do ofendido (aceito/recusado) ou perdao judicial.

## Metodologia (ARTIGOS REAIS — grep antes de afirmar)
1. **Decadencia (CP 103 + CPP 38):** salvo disposicao em contrario, o ofendido **decai do direito de queixa ou de representacao se nao o exerce em 6 (seis) meses**, contados **do dia em que veio a saber quem e o autor do crime** (CP 103); no caso do art. 100 §3 do CP, do dia em que se esgota o prazo da denuncia. **Prazo MATERIAL** -> conta-se incluindo o dia do comeco (CP 10), nao se prorroga por feriado, e fatal/improrrogavel. Ocorrida -> extingue a punibilidade (CP 107, IV).
2. **Perempcao (CPP 60 — so na acao penal EXCLUSIVAMENTE privada; grep e ler I a IV):** considera-se perempta a acao quando, **iniciada** esta: I o querelante deixa de promover o andamento por **30 dias seguidos**; II falecendo/incapacitando-se o querelante, ninguem habilitado comparece em **60 dias** (ressalvado o art. 36); III o querelante deixa de comparecer, sem motivo justificado, a ato a que deva estar presente, **ou deixa de formular o pedido de condenacao nas alegacoes finais**; IV sendo o querelante pessoa juridica, esta se extingue sem deixar sucessor. **So cabe em acao privada propriamente dita** — nao na privada subsidiaria da publica (MP retoma — art. 29). Ocorrida -> extingue (CP 107, IV).
3. **Renuncia ao direito de queixa (CP 104 + CPP 49-51):** o direito de queixa nao pode ser exercido quando renunciado, **expressa ou tacitamente** (CP 104); renuncia tacita = ato incompativel com a vontade de exerce-lo (paragrafo unico — receber a indenizacao do dano NAO implica renuncia). Renuncia em relacao a um dos autores aproveita a todos (CPP 49). Causa de extincao (CP 107, V).
4. **Perdao do ofendido (CP 105-106 + CPP 51, 58-59):** nos crimes que so se procedem mediante queixa, obsta ao prosseguimento (CP 105). E **bilateral** — depende de **aceitacao** (CP 106, III: se o querelado recusa, nao produz efeito; CPP 58-59 disciplinam a aceitacao). Concedido a qualquer querelado, a todos aproveita (CP 106, I); por um dos ofendidos, nao prejudica os outros (II). **Nao cabe depois do transito em julgado** (CP 106, §2). Aceito -> extingue (CP 107, V). Distinguir da renuncia: renuncia e ANTES de oferecida a queixa e unilateral; perdao e DEPOIS e bilateral.
5. **Perdao judicial (CP 107, IX + 120):** causa de extincao **nos casos previstos em lei** (concedido pelo juiz na sentenca em hipoteses tipicas legais). A sentenca que concede perdao judicial **nao gera reincidencia** (CP 120). Verificar se o tipo penal/lei admite a hipotese antes de afirmar cabimento.
6. **Tudo desagua no art. 107:** decadencia e perempcao -> inciso IV; renuncia e perdao aceito -> inciso V; perdao judicial -> inciso IX. Reconhecida a extincao, o juiz declara de oficio (CPP 61).

## Saida obrigatoria
1. **Linha do tempo** dos marcos relevantes (ciencia da autoria · 6 meses · oferecimento/recebimento da queixa · ultimo ato/impulso do querelante · alegacoes finais) com os intervalos.
2. **Marcos** classificados (termo inicial da decadencia · inercia de 30/60 dias · omissao em ato/pedido de condenacao).
3. **Verificacao fundamentada** — qual causa (decadencia 103 / perempcao 60-I a IV / renuncia 104 / perdao 105-106 / perdao judicial 120), com o artigo a artigo e o prazo conferido na lei seca.
4. **Parecer conclusivo:** ocorreu (qual causa, qual inciso) ou nao ocorreu (o que falta), com a peca/requerimento de extincao recomendado (CP 107 + CPP 61).
5. Handoff ao `criminal-master`; passa pela `suprema-corte-criminal`.

## Guard
Nenhum prazo/causa sai sem `validador-criminal` (cruza `context/`) — 6 meses, 30 dias e 60 dias vem de `grep` no CP/CPP, nunca de memoria. Decadencia = prazo MATERIAL (CP 10: conta o 1o dia, nao prorroga). Confirmar a especie de acao (privada propria x condicionada x subsidiaria) antes de afirmar perempcao. Jurisprudencia so se ✅. Na duvida, bloquear e reler a lei seca. Gate final `suprema-corte-criminal`.

decadencia-perempcao -> arts. citados: CP 103, 104, 105, 106 (I-III, §2), 107 (IV, V, IX), 120, 10; CPP 38, 49, 50, 51, 58, 59, 60 (I-IV), 61.
