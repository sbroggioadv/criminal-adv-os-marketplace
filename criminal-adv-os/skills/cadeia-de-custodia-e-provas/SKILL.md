---
name: cadeia-de-custodia-e-provas
description: "Gestao processual penal da prova (Camada 2, critica para a defesa): cadeia de custodia, prova ilicita e derivadas, reconhecimento de pessoas, busca e apreensao e interceptacao. Use ao discutir validade/nulidade de prova ou quando o operador disser cadeia de custodia, prova ilicita, reconhecimento, busca e apreensao, interceptacao, quebra da cadeia, fonte independente, fruto da arvore envenenada, nulidade da prova."
---

# CADEIA-DE-CUSTODIA-E-PROVAS

> Camada 2 (gestao processual penal). Skill CRITICA: a prova ilicita ou com cadeia quebrada derruba o lastro da acusacao. Transversal — roda antes/junto de qualquer peca que ataque ou dependa de prova.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — grep cada artigo (158-A a 158-F, 157, 226, 240-250) e ler a faixa nao-tachada.
- `context/jurisprudencia-criminal.md` — so itens ✅ (Tema 1.016 STJ sobre reconhecimento esta confirmado).
- `context/metodologia-criminal.md` — fluxo da persecucao e regras de ouro.

## Objetivo
Mapear a prova do caso, testar sua licitude e a rastreabilidade do vestigio, e transformar cada falha em tese de nulidade ou de fragilidade probatoria a favor da defesa.

## Quando ativar
- Ha prova pericial, apreensao, reconhecimento, interceptacao ou flagrante a contestar.
- Suspeita de violacao de domicilio, abordagem sem fundada suspeita ou reconhecimento fora do rito.
- O master pede a analise probatoria transversal antes de resposta a acusacao, alegacoes finais, HC ou recurso.

## Metodologia
1. **Inventario da prova.** Listar toda prova do caso (documental, pericial, testemunhal, reconhecimento, interceptacao) e o elo de cada uma com a acusacao.
2. **Cadeia de custodia (arts. 158-A a 158-F do CPP, incluidos pela Lei 13.964/2019).** Verificar a historia cronologica do vestigio nas etapas do art. 158-B (coleta, acondicionamento, transporte, recebimento). Quebra, lacuna ou ausencia de rastreabilidade = fragilidade ou ilicitude da prova pericial.
3. **Prova ilicita (art. 157 do CPP).** Prova obtida em violacao a norma constitucional ou legal e inadmissivel e deve ser desentranhada. Mapear as **derivadas (art. 157, § 1º — fruto da arvore envenenada)** e checar as excecoes (nexo de causalidade nao evidenciado / fonte independente, art. 157, § 2º).
4. **Reconhecimento de pessoas (art. 226 do CPP).** Conferir o rito (descricao previa; pessoa ao lado de semelhantes; auto pormenorizado com duas testemunhas). **Tema 1.016 STJ ✅:** o art. 226 e cogente; reconhecimento em desacordo nao serve, por si so, para condenar (mesmo confirmado em juizo) — tese de absolvicao por insuficiencia probatoria.
5. **Busca e apreensao (arts. 240 a 250 do CPP).** Domiciliar exige mandado/ordem judicial e fundadas razoes (art. 240, § 1º); pessoal exige fundada suspeita (art. 240, § 2º) e independe de mandado nos casos do art. 244. Sem mandado, sem fundada suspeita ou fora dos limites = prova ilicita.
6. **Interceptacao telefonica (Lei 9.296/1996).** Exige ordem judicial fundamentada, crime punido com reclusao e prazo legal. Captacao sem autorizacao ou fora do prazo = ilicitude (art. 157 do CPP).
7. **Tese probatoria.** Para cada falha, formular o pedido (desentranhamento, nulidade da prova e das derivadas, absolvicao por insuficiencia) e o lastro legal artigo a artigo.

## Entrega obrigatoria final
- Mapa da prova + diagnostico de cada vicio (cadeia / ilicitude / rito) com o dispositivo, mais o pedido defensivo correspondente e a jurisprudencia ✅ aplicavel, pronto para alimentar a peca. Validado pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo, percentual ou jurisprudencia sem `validador-criminal` (cruza `context/`). Jurisprudencia so com ✅ em `context/jurisprudencia-criminal.md` — 🟡/ausente bloqueia ate confirmar. Gate final obrigatorio `suprema-corte-criminal`. Na duvida sobre vigencia/redacao, ler a lei seca nao-tachada em `context/`.
