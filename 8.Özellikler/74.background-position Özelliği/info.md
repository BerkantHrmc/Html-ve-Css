# background-position Özelliği

`background-position`, bir öğenin arka plan resminin konumunu ayarlamak için kullanılır.

---

## Temel Kullanım

```css
div {
  background-image: url("resim.jpg");
  background-position: top left;
}
```

Resim sol üst köşeye yerleşir.

---

## Değerler

- Anahtar kelimeler: `top`, `bottom`, `left`, `right`, `center`
- Yüzdelik: `%` (ör. `50% 50%` → ortalar)
- Uzunluk birimleri: `px`, `em` (ör. `10px 20px`)

---

## Örnekler

```css
.box1 {
  background-position: center center;
}

.box2 {
  background-position: right bottom;
}

.box3 {
  background-position: 20px 30px;
}

.box4 {
  background-position: 50% 0%;
}
```

---

## Not

`background-position`, genelde `background-repeat` ve `background-size` ile birlikte kullanılır. Tek bir değer verilirse ikincisi `center` olur (`left` → `left center` gibi).
