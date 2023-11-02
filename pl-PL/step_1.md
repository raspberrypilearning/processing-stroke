`stroke()` ustawia kolor obramowań wokół kształtów. Podobnie jak funkcja `fill()`, funkcja `stroke()` odnosi się do wszystkiego, co zostanie narysowane po jej wywołaniu, więc będziesz musiał dodać kod `stroke()` za każdym razem, gdy będziesz chciał zmienić kolor obrysu.

Aby całkowicie usunąć obramowania, dodaj `no_stroke()` przed narysowaniem kształtu (kształtów).

Grubość obramowania można kontrolować za pomocą `stroke_weight()`

Ten przykład ma `no_stroke()` dla nieba, trawy i brązu, a następnie zmienia się na `stroke(WHITE)` `stroke_weight(3)`, aby narysować docelowe okręgi.

--- code ---
---
language: python
filename: main.py - draw()
---

    no_stroke()  # usuwa obramowanie
    fill(BLUE)  # niebo
    rect(0, 0, 400, 250)
    fill(GREEN)  # trawa
    rect(0, 250, 400, 150)
    fill(BROWN) 
    triangle(150, 350, 200, 150, 250, 350)  # stoisko
    stroke(WHITE)  # Biały kontur
    stroke_weight(3)  # Gruby kontur
    fill(GREY)
    ellipse(200, 200, 170, 170)  # Koło zewnętrzne
    fill(RED)
    ellipse(200, 200, 110, 110)  # Koło wewnętrzne
    fill(YELLOW)
    ellipse(200, 200, 30, 30)  # Bullseye

--- /code ---

![Scena strzelania z łuku z grubymi białymi obwódkami na okręgach i bez ramek na prostokątach lub trójkątach.](images/outline-circles.png)
