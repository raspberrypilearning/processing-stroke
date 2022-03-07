`stroke()` stelt de kleur in die moet worden gebruikt voor de randen rond de vormen. Net als bij `fill()` is de functie `stroke()` van toepassing op alles wat getekend wordt nadat je het hebt aangeroepen, dus je moet `stroke()` code toevoegen elke keer dat je de lijnkleur wilt wijzigen.

Om de randen volledig te verwijderen, voeg je `no_stroke()` toe voordat je je vorm(en) tekent.

De dikte van de rand kan worden ingesteld met `stroke_weight()`

Dit voorbeeld heeft `no_stroke()` voor de lucht, het gras en de bruine standaard, verandert dan in `stroke(WHITE)` en `stroke_weight(3)` om de doelcirkels te tekenen.

--- code ---
---
language: python
filename: main.py - draw()
---

  no_stroke() # verwijdert randen fill(BLUE) # lucht rect(0, 0, 400, 250) fill(GREEN) # gras rect(0, 250, 400, 150) fill(BROWN) triangle( 150, 350, 200, 150, 250, 350) # standaard stroke(WHITE) # Een witte omtrek stroke_weight(3) # Een dikke omtrek fill (GREY) ellipse(200, 200, 170, 170) # Buitenste cirkel fill(RED) ellipse(200, 200, 110, 110) # Binnenste cirkel fill(YELLOW) ellips (200, 200, 30, 30) # Roos

--- /code ---

![Een boogschietscène met dikke, witte randen om de cirkels en geen randen op de rechthoeken of driehoek.](images/outline-circles.png)
