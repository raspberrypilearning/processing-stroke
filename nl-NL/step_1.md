`stroke()` stelt de kleur in die moet worden gebruikt voor de randen rond de vormen. Net als bij `fill()` is de functie `stroke()` van toepassing op alles wat getekend wordt nadat je het hebt aangeroepen, dus je moet `stroke()` code toevoegen elke keer dat je de lijnkleur wilt wijzigen.

Om de randen volledig te verwijderen, voeg je `no_stroke()` toe voordat je je vorm(en) tekent.

De dikte van de rand kan worden ingesteld met `stroke_weight()`

Dit voorbeeld heeft `no_stroke()` voor de lucht, het gras en de bruine standaard, verandert dan in `stroke(WHITE)` en `stroke_weight(3)` om de doelcirkels te tekenen.

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
