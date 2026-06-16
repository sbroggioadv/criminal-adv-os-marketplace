---
name: base-legal-penal-especial
description: "Porta de fundacao para as LEIS PENAIS ESPECIAIS (drogas 11.343/06, hediondos 8.072/90, anticrime 13.964/19, orcrim 12.850/13, lavagem 9.613/98, Maria da Penha 11.340/06) com alertas de vigencia 2024-2026. Use quando o operador disser lei de drogas, crime hediondo, organizacao criminosa, lavagem, Maria da Penha, lei especial, trafico, rol de hediondos, ou citar uma lei penal extravagante."
---

# BASE-LEGAL-PENAL-ESPECIAL — Porta para as Leis Penais Especiais

> Camada 1 (fundacao enraizada). Esta skill NAO redige peca — ela aponta e ensina a navegar os recortes vigentes das leis especiais, para que o tipo extravagante e seus regimes saiam do arquivo conferido, nunca da memoria de treino.

## Anexos obrigatorios (context/)
- `context/penal-especial.md` — recortes vigentes das leis penais especiais + alertas 2024-2026 (so os artigos centrais, em redacao essencial). **Localizar a lei/artigo por busca + ler o bloco**; conferir o alerta de vigencia antes de citar.

## Objetivo
Entregar o dispositivo da lei especial exato (tipo, pena, regime de beneficios, rol de hediondos) na redacao VIGENTE, lido do arquivo, evitando citar lei revogada ou tese cancelada.

## Quando ativar
- Pergunta sobre lei de drogas, crimes hediondos, organizacao criminosa, lavagem de dinheiro, Maria da Penha ou outra lei penal extravagante.
- Necessidade de saber se um crime e hediondo/equiparado e qual o regime de beneficios.
- Antes de redigir/calcular qualquer caso que toque uma lei especial.

## Como navegar (regra de uso)
1. **Buscar** a lei/artigo no `context/penal-especial.md` e ler so o bloco — e **ler o ALERTA DE VIGENCIA 2024-2026 no topo do arquivo** antes de citar.
2. **Cobertura:** drogas **11.343/06** (art. 28 consumo, 33 trafico, 33 §4 privilegiado, 42 dosimetria, 44 vedacoes); hediondos **8.072/90** (rol atualizado ate **Lei 15.384/2026**); anticrime **13.964/19**; orcrim **12.850/13**; lavagem **9.613/98**; Maria da Penha **11.340/06**.
3. **Pontos vivos confirmados (conferir no arquivo):** trafico privilegiado **nao** e hediondo (Sumula 512 STJ cancelada); maconha consumo pessoal — STF RE 635.659/Tema 506 (parametro ate 40g/6 plantas, presuncao relativa); feminicidio entrou no rol (14.994/2024); rol reescrito por 15.159/2025; dominio social estruturado e fracoes de progressao alteradas pela **Lei 15.358/2026 (Antifacao)**.
4. **Lei nao confirmada = nao citar:** "Lei 15.299/2025" nao foi achada nos codigos — 🟡 conferir no Planalto antes de usar.

## Entrega obrigatoria final
- Nome da lei + artigo + redacao vigente do dispositivo + status (hediondo? beneficio vedado?), transcritos do `context/penal-especial.md`, com nota de vigencia 2024-2026 — pronto para a skill de tipicidade/execucao usar.

## Guard
Nenhum tipo especial, pena ou regime de beneficio entra em peca sem passar pelo `validador-criminal` (cruza o `context/`). Se o alerta de vigencia ou o status (hediondo/cancelado) for duvidoso, BLOQUEAR e checar ao vivo (firecrawl/Planalto). Toda entrega fecha pela `suprema-corte-criminal`.
