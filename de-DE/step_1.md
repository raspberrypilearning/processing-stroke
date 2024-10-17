`stroke()` legt die Farbe fest, die für die Ränder um die Formen verwendet werden soll. Genau wie `fill()` gilt die Funktion `stroke()` für alles, was nach dem Aufruf gezeichnet wird. Du musst also jedes Mal, wenn du die Strichfarbe ändern möchten, den Code `stroke()` hinzufügen.

Um die Ränder vollständig zu entfernen, fügst du vor dem Zeichnen deiner Form(en) `no_stroke()` hinzu.

Die Dicke des Randes kann mit `stroke_weight()` gesteuert werden

Dieses Beispiel verwendet `no_stroke()` für den Himmel, das Gras und den braunen Stand und dann `stroke(WEISS)` `stroke_weight(3)`, um die Zielkreise zu zeichnen.

--- code ---
---
language: python
filename: main.py - draw()
---

    no_stroke()  # entfernt Ränder
    fill(BLAU)  # Himmel
    rect(0, 0, 400, 250)
    fill(GRÜN)  # Gras
    rect(0, 250, 400, 150)
    fill(BRAUN) 
    triangle(150, 350, 200, 150, 250, 350)  # Stand
    stroke(WEISS)  # Eine weiße Umrandung
    stroke_weight(3)  # Eine dicke Umrandung
    fill(GRAU)
    ellipse(200, 200, 170, 170)  # Äußerer Kreis
    fill(ROT)
    ellipse(200, 200, 110, 110)  # Innerer Kreis
    fill(GELB)
    ellipse(200, 200, 30, 30)  # Volltreffer

--- /code ---

![Eine Bogenschießszene mit dicken weißen Rändern um die Kreise und ohne Ränder um die Rechtecke und Dreiecke.](images/outline-circles.png)
