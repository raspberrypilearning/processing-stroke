`stroke()` define a cor a ser usada para as bordas ao redor das formas. Assim como o `fill()`, a função `stroke()` se aplica a tudo criado depois que você a chama, então você precisará adicionar o código `stroke()` toda vez que quiser alterar a cor do traço.

Para remover as bordas completamente, adicione `no_stroke()` antes de criar sua(s) forma(s).

A espessura da borda pode ser modificada usando `stroke_weight()`

Este exemplo tem `no_stroke()` para desenhar o céu, grama e o suporte do alvo marrom, então muda para `stroke(WHITE)` `stroke_weight(3)` para desenhar os círculos alvo.

--- code ---
---
language: python
filename: main.py - draw()
---

    no_stroke()  # removes borders
    fill(BLUE)  # sky
    rect(0, 0, 400, 250)
    fill(GREEN)  # grass
    rect(0, 250, 400, 150)
    fill(BROWN) 
    triangle(150, 350, 200, 150, 250, 350)  #stand
    stroke(WHITE)  # A white outline
    stroke_weight(3)  # A thick outline
    fill(GREY)
    ellipse(200, 200, 170, 170)  # Outer circle
    fill(RED)
    ellipse(200, 200, 110, 110)  # Inner circle
    fill(YELLOW)
    ellipse(200, 200, 30, 30)  # Bullseye

--- /code ---

![An archery scene with thick, white borders on the circles and no borders on the rectangles or triangle.](images/outline-circles.png)
