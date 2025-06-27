# font Özellikleri

CSS'de yazı tipiyle ilgili birden fazla özelliği kontrol etmek için aşağıdaki `font-*` özellikleri kullanılır:

---

## Temel font Özellikleri

- `font-family` → Yazı tipi
- `font-size` → Yazı boyutu
- `font-style` → Eğik yazı (italic)
- `font-weight` → Kalınlık
- `font-variant` → Küçük büyük harf (small-caps)
- `line-height` → Satır yüksekliği

---

## Kısayol Kullanım (Shorthand)

```css
p {
  font: italic small-caps bold 16px/1.5 "Times New Roman", serif;
}
```

Yukarıdaki sırayla yazılır:

```
font-style font-variant font-weight font-size/line-height font-family
```

---

## Örnek

```css
h1 {
  font: italic normal 700 24px/1.7 Arial, sans-serif;
}
```

---

## Not

`font-size` ve `font-family` kısayol tanımında **zorunludur**, diğerleri isteğe bağlıdır.
