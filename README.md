Esse código cria um objeto invisível (sem sprite) que exibe uma mensagem na tela de forma intermitente, alternando a cada 10 segundos (600 frames, considerando que o jogo roda a 60 FPS).

alarme0 e alarme1 começam com 600, o que equivale a 10 segundos (600 frames) se o jogo estiver rodando a 60 FPS.
Esses valores vão ser usados para controlar quando a mensagem aparece e desaparece.

alarme0 diminui 1 a cada frame, contando o tempo até chegar a 0.

Quando alarme1 chega a 0, ambos os alarmes são reiniciados para 600, reiniciando o ciclo.

Quando alarme0 chega a 0, a mensagem é desenhada na tela.
Enquanto a mensagem está visível, alarme1 começa a diminuir.
Quando alarme1 chega a 0, o Step reinicia alarme0 e alarme1, recomeçando o ciclo.
