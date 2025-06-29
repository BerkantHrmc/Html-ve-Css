# background-clip Özelliği

`background-clip`, bir öğenin arka planının **hangi sınırlar içinde** görüneceğini belirler.

---

## Temel Kullanım

```css
div {
  background: lightblue;
  border: 5px dashed black;
  background-clip: padding-box;
}
```

---

## Değerler

- `border-box` → Arka plan, border (kenarlık) dahil tüm kutuyu kaplar (varsayılan).
- `padding-box` → Arka plan sadece padding ve içerik alanını kaplar, border'ı kaplamaz.
- `content-box` → Arka plan sadece içerik alanını kaplar.

---

## Örnekler

```css
.box1 {
  background-clip: border-box;
}

.box2 {
  background-clip: padding-box;
}

.box3 {
  background-clip: content-box;
}
```

---

## Not

`background-clip`, genelde `background-origin` ve kenarlıklı kutularla birlikte kullanılarak arka planın sınırlarını netleştirir.
