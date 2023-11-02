Mae `stroke()` yn gosod y lliw i'w ddefnyddio ar gyfer y borderi o amgylch y siapiau. Yn union fel `fill()`, mae'r swyddogaeth `stroke()` yn berthnasol i bopeth sy'n cael ei lunio ar ôl i chi ei galw, felly bydd angen i chi ychwanegu cod `stroke()` bob tro rydych chi am newid y lliw strôc.

I gael gwared ar y borderi yn llwyr, ychwanegwch `no_stroke()` cyn llunio eich siâp(iau).

Mae modd rheoli trwch y border gan ddefnyddio `stroke_weight()`

Mae gan yr enghraifft hon `no_stroke()` ar gyfer yr awyr, y gwair a'r stand brown, wedyn yn newid i `stroke(WHITE)` `stroke_weight(3)` i lunio cylchoedd y targed.

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
