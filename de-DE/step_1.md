`stroke()` legt die Farbe fest, die für die Ränder um die Formen verwendet werden soll. Genau wie `fill()` gilt die Funktion `stroke()` für alles, was nach dem Aufruf gezeichnet wird. Du musst also jedes Mal, wenn du die Strichfarbe ändern möchten, den Code `stroke()` hinzufügen.

Um die Ränder vollständig zu entfernen, fügst du vor dem Zeichnen deiner Form(en) `no_stroke()` hinzu.

Die Dicke des Randes kann mit `stroke_weight()` gesteuert werden

Dieses Beispiel verwendet `no_stroke()` für den Himmel, das Gras und den braunen Stand und dann `stroke(WHITE)` `stroke_weight(3)`, um die Zielkreise zu zeichnen.

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

![Eine Bogenschießszene mit dicken weißen Rändern um die Kreise und ohne Ränder um die Rechtecke und Dreiecke.](images/outline-circles.png)
