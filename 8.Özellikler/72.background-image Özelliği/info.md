# background-image Özelliği

`background-image`, bir öğeye arka plan resmi eklemek için kullanılır.

---

## Temel Kullanım

```css
div {
  background-image: url("resim.jpg");
}
```

Belirtilen URL'deki görsel, öğenin arka planına yerleştirilir.

---

## Çoklu Arka Plan

Birden fazla arka plan resmi eklenebilir. İlk resim üstte olacak şekilde sıralanır.

```css
div {
  background-image: url("ust.png"), url("alt.jpg");
}
```

---

## Değerler

- `none` → Arka plan resmi kullanılmaz.
- `url()` → Resim dosyasının yolu belirtilir.

---

## Örnek

```css
body {
  background-image: url("bg-pattern.png");
}

section {
  background-image: none;
}
```

---

## Not

Arka plan resimleri genelde `background-repeat`, `background-size` ve `background-position` özellikleriyle birlikte kullanılır.
