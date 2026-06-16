---
name: assistente-de-acusacao
description: "Assistente de acusacao (Camada 6 — contraponto, para quando o cliente e a VITIMA): habilitacao do ofendido junto ao MP, momento, poderes e recursos. Use quando o cliente quer atuar como ofendido no processo, ou quando o operador disser assistente de acusacao, vitima quer participar, habilitar como assistente, ofendido no processo, recurso do assistente."
---

# ASSISTENTE-DE-ACUSACAO

> Camada 6 (defesa, liberdade & investigacao) — contraponto acusatorio. Aciona-se quando o cliente do escritorio e a VITIMA (ofendido), que se habilita ao lado do Ministerio Publico para influir na acao penal publica. Fora desse caso, o foco do plugin permanece na defesa.

## Anexos obrigatorios (context/)
- `context/cpp-3689-41.md` — grep arts. 268-273 (habilitacao, momento, poderes do assistente) e 584, § 1º, e 598 (recursos do assistente), e ler a faixa nao-tachada.
- `context/jurisprudencia-criminal.md` — so itens ✅. Nas notas do Tribunal do Juri, conferir o estado do tema antes de sustentar.
- `context/metodologia-criminal.md` — fluxo da persecucao e regras de ouro.

## Objetivo
Habilitar o ofendido como assistente do Ministerio Publico no momento processual cabivel, exercer os poderes de prova e debate, e usar a via recursal supletiva quando a acusacao oficial nao recorrer, com fundamento artigo a artigo.

## Quando ativar
- O cliente e a vitima (ou seu representante legal / sucessor do art. 31) e quer participar ativamente da acao penal publica.
- Necessidade de propor provas, requerer perguntas, participar do debate ou recorrer supletivamente de impronuncia/sentenca quando o MP nao recorre.
- O master identifica a posicao de ofendido e aciona o contraponto acusatorio.

## Metodologia
1. **Legitimidade (art. 268 do CPP).** Em todos os termos da acao publica pode intervir, como assistente do MP, o **ofendido** ou seu representante legal, ou, na falta, as pessoas do art. 31 (conjuge, ascendente, descendente, irmao). **Vedacao (art. 270):** o corre no mesmo processo nao pode ser assistente.
2. **Momento (art. 269 do CPP).** O assistente e admitido **enquanto nao passar em julgado a sentenca** e recebe a causa no estado em que se achar — ou seja, apos recebida a denuncia e antes do transito em julgado.
3. **Admissao (arts. 272-273 do CPP).** O MP e ouvido previamente sobre a admissao (art. 272). Do despacho que admitir ou nao o assistente **nao cabe recurso** (art. 273) — embora pedido e decisao devam constar dos autos.
4. **Poderes (art. 271 do CPP).** Ao assistente e permitido propor meios de prova, requerer perguntas as testemunhas, aditar os articulados, participar do debate oral e **arrazoar os recursos** interpostos pelo MP ou por ele proprio, nos casos dos arts. 584, § 1º, e 598. O juiz, ouvido o MP, decide sobre as provas propostas (§ 1º); o processo prossegue se o assistente intimado faltar sem forca maior (§ 2º).
5. **Recursos do assistente (arts. 271, 584, § 1º, e 598 do CPP).** O assistente pode **apelar supletivamente** — quando o MP nao recorre, pode recorrer da sentenca (art. 598) e atuar nos casos de impronuncia/situacoes do art. 584, § 1º. Calcular tempestividade pela `prazos-processuais-penais` (prazo supletivo do assistente, contado conforme o CPP e a jurisprudencia — confirmar ao vivo pelo `validador-criminal`).
6. **Estrategia de prova e debate.** Articular requerimentos de prova e perguntas alinhados ao interesse da vitima, cruzando com `estrategia-penal` e `cadeia-de-custodia-e-provas`.
7. **Tribunal do Juri.** Em crimes do juri, atentar para a participacao do assistente e o recurso do art. 598 — conferir as notas defensivas/acusatorias do juri em `jurisprudencia-criminal` antes de sustentar.

## Entrega obrigatoria final
- Peca de habilitacao do assistente (ou arrazoado/recurso supletivo) com legitimidade do art. 268 + momento do art. 269 + poderes do art. 271 + base recursal dos arts. 584, § 1º, e 598, com fundamento artigo a artigo e jurisprudencia ✅. Validado pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo, prazo ou jurisprudencia sem `validador-criminal` (cruza `context/`). Jurisprudencia so com ✅ em `context/jurisprudencia-criminal.md` — 🟡/ausente bloqueia ate confirmar ao vivo (inclui prazo recursal supletivo do assistente). Gate final obrigatorio `suprema-corte-criminal`. Na duvida sobre vigencia/redacao, ler a lei seca nao-tachada em `context/`.
