`stroke()` define a cor a ser usada para as bordas ao redor das formas. Assim como o `fill()`, a função `stroke()` se aplica a tudo criado depois que você a chama, então você precisará adicionar o código `stroke()` toda vez que quiser alterar a cor do traço.

Para remover as bordas completamente, adicione `no_stroke()` antes de criar sua(s) forma(s).

A espessura da borda pode ser modificada usando `stroke_weight()`

Este exemplo tem `no_stroke()` para desenhar o céu, grama e o suporte do alvo marrom, então muda para `stroke(WHITE)` `stroke_weight(3)` para desenhar os círculos alvo.

--- code ---
---
language: python
filename: main.py - draw()
---

  no_stroke() # remove bordas fill(BLUE) # céu, preenchimento azul rect(0, 0, 400, 250) fill(GREEN) # grama, preenchimento verde rect(0, 250, 400, 150) fill(BROWN) # Preenchimento marrom triangle( 150, 350, 200, 150, 250, 350) # suporte do alvo stroke(WHITE) # Um contorno branco stroke_weight(3) # Um contorno grosso fill(GREY) # Preenchimento cinza elipse(200, 200, 170, 170) # Círculo externo fill(RED) # Preenchimento vermelho elipse(200, 200, 110, 110) # Círculo interno fill(YELLOW) # Preenchimento amarelo elipse(200, 200, 30, 30) # Centro do alvo

--- /code ---

![Uma cena de tiro com arco e flechas, com bordas grossas e brancas nos círculos e sem bordas nos retângulos ou triângulos.](images/outline-circles.png)
