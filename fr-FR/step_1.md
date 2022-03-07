`stroke()` définit la couleur à utiliser pour les bordures autour des formes. Tout comme `fill()` la fonction `stroke()` s'applique à tout ce qui est dessiné après l'avoir appelée, tu devras donc ajouter le `stroke()` chaque fois que tu souhaites changer la couleur du trait.

Pour supprimer complètement les bordures, ajoute `no_stroke()` avant de dessiner ta ou tes formes.

L'épaisseur de la bordure peut être contrôlée à l'aide de `stroke_weight()`

Cet exemple a `no_stroke()` pour le ciel, l'herbe et le stand marron, puis passe à `stroke(WHITE)` `stroke_weight(3)` pour dessiner les cercles de la cible.

--- code ---
---
language: python
filename: main.py - draw()
---

  no_stroke() # supprime les bordures fill(BLUE) # ciel rect(0, 0, 400, 250) fill(GREEN) # herbe rect(0, 250, 400, 150) fill(BROWN) triangle(150, 350, 200, 150, 250, 350) #support stroke(WHITE) # Un contour blanc stroke_weight(3) # Un contour épais fill(GREY) ellipse(200, 200, 170, 170) # Cercle extérieur fill(RED) ellipse(200, 200, 110, 110) # Cercle intérieur fill(YELLOW) ellipse(200, 200, 30, 30) # Centre de la cible

--- /code ---

![Une scène de tir à l'arc avec des bordures épaisses et blanches sur les cercles et sans bordures sur les rectangles ou le triangle.](images/outline-circles.png)
