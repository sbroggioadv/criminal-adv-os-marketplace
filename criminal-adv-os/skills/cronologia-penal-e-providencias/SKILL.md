---
name: cronologia-penal-e-providencias
description: "Monta a linha do tempo do caso e a lista de providencias (Camada 2, metodologica): data do fato, prisao/flagrante, recebimento da denuncia, citacao, AIJ, sentenca, transito — base para prescricao, detracao e prazos. Lista as pendencias e o proximo prazo fatal. Use quando o operador disser linha do tempo, cronologia, marcos do processo, providencias, proximos passos ou o que falta fazer."
---

# CRONOLOGIA-PENAL-E-PROVIDENCIAS

> Camada 2 (metodologica). Organiza o caso no eixo do tempo e na fila de tarefas. Alimenta o Motor Penal Temporal (prescricao, detracao, prazos) e nunca deixa pendencia sem dono nem prazo.

## Anexos obrigatorios (context/)
- `context/cp-2848-40.md` — grep os marcos da prescricao (art. 117) e a detracao (art. 42); ler a faixa nao-tachada.
- `context/cpp-3689-41.md` — atos e ritos processuais (sob demanda).
- `context/metodologia-criminal.md` — fluxo da persecucao e regras de ouro.

## Objetivo
Reconstruir a sequencia exata dos atos do caso, fixar os marcos relevantes para o calculo temporal, e devolver a lista de providencias pendentes com o proximo prazo fatal em destaque.

## Quando ativar
- Caso novo, caso assumido de outro advogado ou pedido de panorama.
- O operador pergunta o que falta fazer, quais os proximos passos ou os marcos do processo.
- Antes de calcular prescricao, detracao ou de planejar a semana de prazos.

## Metodologia
1. **Coletar os atos do caso** a partir da `memoria-de-caso-criminal` e dos autos: data do fato, prisao/flagrante, recebimento da denuncia, citacao, resposta a acusacao, AIJ, alegacoes finais, sentenca, recursos, transito em julgado, inicio de cumprimento.
2. **Montar a linha do tempo** em ordem cronologica, com data de cada ato e a fase correspondente da persecucao.
3. **Marcar os pontos de prescricao (art. 117 do CP — causas interruptivas):** recebimento da denuncia ou queixa (I), pronuncia (II), confirmacao da pronuncia (III), publicacao da sentenca/acordao condenatorio recorrivel (IV), inicio ou continuacao do cumprimento (V), reincidencia (VI). Apos cada marco, o prazo recomeca do zero (art. 117, § 2º). Sinalizar o intervalo entre marcos para `prescricao-penal` calcular.
4. **Computar a detracao (art. 42 do CP):** somar o tempo de prisao provisoria, administrativa e internacao para abater na pena — sinalizar para `detracao`/`motor-calculo-de-pena`.
5. **Levantar as providencias pendentes** (peca a redigir, prova a requerer, recurso a interpor, beneficio a pleitear) e atribuir o **proximo prazo fatal** de cada uma.
6. **Destacar o prazo mais proximo** e conectar com `memoria-de-caso-criminal` para registrar ato praticado, proximo passo e prazo.

## Entrega obrigatoria final
- Linha do tempo do caso (ato + data + fase) + marcos de prescricao e detracao sinalizados + lista de providencias com responsavel e prazo + proximo prazo fatal em destaque, gravado na `memoria-de-caso-criminal`. Validado pela `suprema-corte-criminal` (R1-R4).

## Guard
Nenhum dispositivo ou calculo temporal sem `validador-criminal` (cruza `context/`). Marco de prescricao e detracao sempre conferidos na lei seca nao-tachada (art. 117 e art. 42 do CP). Calculo de prescricao/pena nunca de cabeca — sai com linha do tempo + marcos + fundamento. Gate final obrigatorio `suprema-corte-criminal`.
