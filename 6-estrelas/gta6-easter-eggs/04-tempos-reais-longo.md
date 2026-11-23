# Vídeo longo — tempos reais (faixa de voz limpa)

Faixa: `audio/longo_voz_limpa.wav` · **8:00,9** (a gravação bruta tem 8:32,6).
Medido sobre a faixa final, não estimado. A transcrição automática usada para localizar os blocos troca algumas palavras (nomes próprios, "Kyle", "Dexter"); isso é erro do reconhecimento, não da sua voz.

## O que foi feito na faixa
- **Pausas enxugadas:** pausas comuns viraram ~0,26 s, mantendo o ruído de fundo da sala. Pausas de virada de bloco ficaram em até 0,75 s (tempo do rank card). Pausas dramáticas foram mantidas em 0,45–0,60 s (por exemplo, antes de "e o Kyle vira um monstro", depois de "olhe para o fogo" e de "só que isso é o começo").
- **Vãos dos clipes ("deixa o clipe falar") fixados:** #4 = 6,0 s · #2 = 8,0 s · #1 = 6,0 s. Estão em **silêncio digital**, para você soltar o áudio do jogo por cima.
- **Volume:** −3 dB de folga, teto de −1 dBFS. Integrada ≈ −21 LUFS, pico −1,7 dBFS. Suba no master (compressor suave + limitador) até ≈ −14 LUFS e true peak ≤ −1 dBTP.
- **Conferência:** transcrevi trechos antes e depois de cada vão na faixa final. Cada vão está no lugar certo ("…ou provocar" | vão | "Número um"; "…voltar para casa" | vão | "Mas ainda existe um segredo"; "…só funciona à noite e sozinho" | vão | "Número três").

> Correção: a primeira versão desta faixa, que cheguei a enviar ao repositório, tinha dois vãos no lugar errado por causa de um defeito no meu processamento. Esta versão a substitui.

## Tempos por bloco (na faixa limpa)

| Bloco | Início | Fim | Duração | Início no plano antigo (§5) |
|---|---|---|---|---|
| B0 Gancho | 0:00,0 | 0:23,3 | 23,3 s | 0:00 |
| B1 Regras | 0:23,8 | 0:41,5 | 17,7 s | 0:28 |
| B2 #10 Cachorro | 0:42,3 | 1:13,6 | 31,3 s | 0:55 |
| B3 #9 Dexter | 1:14,4 | 1:45,5 | 31,1 s | 1:30 |
| B4 #8 San Andreas | 1:46,3 | 2:14,8 | 28,5 s | 2:15 |
| B5 #7 Hotel | 2:15,3 | 2:42,6 | 27,3 s | 3:00 |
| B6 Relâmpago | 2:43,1 | 3:09,3 | 26,3 s | 3:45 |
| B7 #6 Caranguejo | 3:09,8 | 3:38,6 | 28,8 s | 4:35 |
| B8 #5 Farol | 3:39,2 | 4:13,7 | 34,5 s | 5:15 |
| B9 #4 Ritual | 4:14,6 | 4:46,6 | 32,0 s | 6:00 |
| **vão de clipe #4** | 4:46,6 | 4:52,6 | **6,0 s** | |
| B10 #3 Pé Grande | 4:52,6 | 5:28,1 | 35,4 s | 6:55 |
| B11 #2 Hulk | 5:28,9 | 6:05,6 | 36,7 s | 7:40 |
| **vão de clipe #2** | 6:05,6 | 6:13,7 | **8,0 s** | |
| B12 #1 ET | 6:13,7 | 7:27,3 | 73,6 s | 8:35 |
| **vão de clipe #1** | 7:27,3 | 7:33,4 | **6,0 s** | |
| B13 Fecho | 7:33,4 | 8:00,8 | 27,4 s | 10:05 |

**Como usar:** na decupagem do `01-video-longo.md` §5, **substitua os tempos de início de cada bloco pelos desta tabela**. Dentro de cada bloco, mantenha a ordem das linhas e distribua os cortes pela fala (use os pontos-chave abaixo).

## Pontos-chave (para sincronizar efeitos e cortes)

| Momento | Tempo |
|---|---|
| Rank card #10 (a voz começa em "Número dez") | 0:42,3 |
| "…não vá ao telhado" (B5) | 2:32,9 |
| Hora da rodada relâmpago | 2:43,1 |
| "a neblina trava o motor" (B8) | 4:00,3 |
| "olhe para o fogo" (B9) | 4:30,4 |
| "Vinte e dois anos depois…" (B10) | 5:04,7 |
| "e o Kyle vira um monstro vermelho gigante" (B11) | 5:51,4 |
| "O disco volta por você" (B12) | 6:32,5 |
| "você acorda três dias depois" (tela apaga) | 6:34,2 |
| "Só que isso é o começo" | 6:40,8 |
| "dentro, um ET vivo" | 7:06,7 |
| "você foge com ele no colo" | 7:08,6 |
| "Recompensa… aumento permanente" | 7:15,4 |
| "Varginha, 1996" | 7:19,8 |
| "Um monumento com um ovo dourado…" | 7:36,8 |
| "qual dessas missões você vai tentar primeiro" | 7:47,9 |

## O que isso muda no projeto

1. **O vídeo fica com ~8 min, não ~10:40.** O plano antigo previa mais de 2 minutos de imagem sem voz. Na gravação real, os únicos trechos sem voz são os 3 vãos de clipe (20 s no total). Recomendação: **não encher** o vídeo para chegar aos 10 min. A referência GG1 (7 min) teve ótimo desempenho, e menos tempo morto ajuda a retenção. Some só o end screen (10–20 s) após o fecho, e o vídeo vai a ~8:20.
2. **A rodada relâmpago agora dura 26 s, não 50 s.** O cronômetro do card deve marcar **0:25**, e o texto da fala "cinquenta segundos" ainda está na gravação. Ou regrave essa frase como "vinte e cinco segundos", ou mantenha o cronômetro em 0:50 correndo mais devagar. Recomendo **regravar a frase** para não contradizer a imagem.
3. **O B12 (ET) ficou com 73,6 s**, contra os 90 s planejados. Mantenha os três mini-clímax (abdução, ET vivo, nave) e use os pontos-chave acima. O vão de 6 s vem logo depois de "…consegue voltar para casa" e antes de "Mas ainda existe um segredo".
4. **O B13 (fecho) agora começa em 7:33,4**, após o vão. Use o crane-up do monumento do ovo dourado em 7:36,8.

## Conferência roteiro × gravação
Todos os 14 blocos do roteiro estão na gravação, na ordem. Diferenças pequenas, nenhuma exige regravar:
- "Um fazendeiro que **virou** Hulk" (no roteiro: "que vira"). Tempo verbal diferente, sentido igual.
- B4: dito "Ninguém ligou", sem o "Na época".
- Resto do texto idêntico ao roteiro (o reconhecimento errou alguns nomes, mas o conteúdo está lá).
