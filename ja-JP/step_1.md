`stroke()`は、図形の周りの境界線に使用する色を設定します。 `fill()`と同様に、`stroke()`関数は、呼び出し後に描画されるすべてに適用されるため、輪郭線の色を変更する必要があるたびに`stroke()`コードを追加しなければなりません。

境界線を完全になくすには、図形を描画する前に`no_stroke()`を追加します。

境界線の太さは、`stroke_weight()`を使って変えることができます

この例では、空、草、茶色の台を`no_stroke()`とし、標的の円を描画するのに`stroke(WHITE)`と`stroke_weight(3)`へ変更しています。

--- code ---
---
language: python
filename: main.py - draw()
---

  no_stroke() # 輪郭線なし fill(BLUE) # 空 rect(0, 0, 400, 250) fill(GREEN) # 草 rect(0, 250, 400, 150) fill(BROWN) triangle(150, 350, 200, 150, 250, 350)  # 台 stroke(WHITE) # 白の輪郭線 stroke_weight(3) # 太い輪郭線 fill(GREY) ellipse(200, 200, 170, 170) # 外側の円 fill(RED) ellipse(200, 200, 110, 110) # 内側の円 fill(YELLOW) ellipse(200, 200, 30, 30) # 中心部

--- /code ---

![円に太い白い輪郭線があり、四角形や三角形に輪郭線がないアーチェリー場。](images/outline-circles.png)
