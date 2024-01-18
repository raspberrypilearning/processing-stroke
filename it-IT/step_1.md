`stroke()` imposta il colore da utilizzare per i bordi attorno alle forme. Proprio come `fill()`, la funzione `stroke()` si applica a tutto ciò che viene disegnato dopo averlo chiamato, quindi dovrai aggiungere il codice `stroke()` ogni volta che desideri cambiare il colore del tratto.

Per rimuovere completamente i bordi, aggiungi `no_stroke()` prima di disegnare le tue forme.

Lo spessore del bordo può essere controllato utilizzando `stroke_weight()`

Questo esempio ha `no_stroke()` per il cielo, l'erba e il supporto marrone, quindi cambia in `stroke(WHITE)` `stroke_weight(3)` per disegnare i cerchi del bersaglio.

--- code ---
---
language: python
filename: main.py - draw()
---

    no_stroke()  # rimuove i bordi
    fill(BLUE)  # cielo
    rect(0, 0, 400, 250)
    fill(GREEN)  # erba
    rect(0, 250, 400, 150)
    fill(BROWN) 
    triangle(150, 350, 200, 150, 250, 350)  # supporto
    stroke(WHITE)  # Un contorno bianco
    stroke_weight(3)  # Un contorno spesso
    fill(GREY)
    ellipse(200, 200, 170, 170)  # Cerchio esterno
    fill(RED)
    ellipse(200, 200, 110, 110)  # Cerchio interno
    fill(YELLOW)
    ellipse(200, 200, 30, 30)  # Centro

--- /code ---

![Una scena di tiro con l'arco con spessi bordi bianchi sui cerchi e senza bordi sui rettangoli o sul triangolo.](images/outline-circles.png)
