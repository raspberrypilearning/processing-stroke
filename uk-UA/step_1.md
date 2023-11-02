`stroke()` встановлює колір, який буде використовуватися для обведення фігур. Так само як і `fill()`, функція `stroke()` застосовується до всього, що намальовано після її виклику, тому тобі потрібно буде додавати код `stroke()` щоразу, коли ти захочеш змінити колір обведення.

Щоб видалити повністю обведення, додай `no_stroke()` перед тим, як намалювати фігуру(и).

Товщину обведення можна регулювати за допомогою `stroke_weight()`

У цьому прикладі використовується `no_stroke()` для неба, трави та коричневого дерева, а потім змінюється на `stroke(WHITE)` `stroke_weight(3)`, щоб намалювати кола для мішені.

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
