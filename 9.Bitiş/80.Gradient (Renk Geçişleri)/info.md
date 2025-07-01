# CSS Gradyent (Gradient) Özelliği — Tek Dosya, Tam Örnek

Gradyent, bir öğenin arka planında renk geçişi sağlar. `linear-gradient`, `radial-gradient` ve `conic-gradient` en yaygın türlerdir. Yönler (`to left`, `to right` vb.), açılar ve çoklu renkler desteklenir.

Aşağıda **tek bir CSS bloğunda** yön, açı, radial ve conic örnekleri **bir arada** verilmiştir:

```css
div {
  width: 300px;
  height: 200px;
  border: 2px solid #000;
}

/* 1️⃣ Linear Gradient Yön Örnekleri */
.left {
  background-image: linear-gradient(to left, red, yellow);
}

.right {
  background-image: linear-gradient(to right, red, yellow);
}

.top {
  background-image: linear-gradient(to top, red, yellow);
}

.bottom {
  background-image: linear-gradient(to bottom, red, yellow);
}

/* 2️⃣ Linear Gradient Açı + Çoklu Renk */
.angle {
  background-image: linear-gradient(45deg, red, orange, yellow, green, blue);
}

/* 3️⃣ Radial Gradient */
.radial {
  background-image: radial-gradient(circle at center, red, yellow, green);
}

/* 4️⃣ Conic Gradient */
.conic {
  background-image: conic-gradient(red, yellow, green, red);
}
