`stroke()` sets the colour to use for the borders around the shapes. Just like `fill()` the `stroke()` function applies to everything drawn after you call it so you will need to add `stroke()` code every time you want to change the stroke colour. 

To remove the borders completely, add `no_stroke()` before drawing your shape(s). 

The thickness of the border can be controlled using `stroke_weight()` 

This example has `no_stroke()` for the sky, grass and brown stand, then changes to `stroke(WHITE)` `stroke_weight(3)` to draw the target circles. 

--- code ---
---
language: python
filename: main.py - draw()
---

  no_stroke() # removes borders
  fill(BLUE) # sky
  rect(0, 0, 400, 250)
  fill(GREEN) # grass
  rect(0, 250, 400, 150)
  fill(BROWN) 
  triangle(150, 350, 200, 150, 250, 350)  #stand
  stroke(WHITE) # A white outline
  stroke_weight(3) # A thick outline
  fill(GREY)
  ellipse(200, 200, 170, 170) # Outer circle
  fill(RED)
  ellipse(200, 200, 110, 110) # Inner circle
  fill(YELLOW)
  ellipse(200, 200, 30, 30) # Bullseye

--- /code ---

![An archery scene with thick, white borders on the circles and no borders on the rectangles or triangle.](images/outline-circles.png)
