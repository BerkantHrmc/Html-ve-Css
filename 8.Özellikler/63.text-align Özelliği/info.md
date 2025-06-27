# text-align Özelliği

`text-align`, metnin yatay hizalamasını belirler.

---

## Değerler

- `left` → Sola hizalar (varsayılan)
- `right` → Sağa hizalar
- `center` → Ortalar
- `justify` → Satırı iki yana yaslayarak boşlukları dengeler
- `start` / `end` → Yazı yönüne göre hizalama (LTR/RTL)

---

## Örnek Kullanım

```css
p {
  text-align: justify;
}

h1 {
  text-align: center;
}
```

---

## Not

`text-align` sadece **blok düzeyindeki öğelerde** etkili olur (örneğin `div`, `p`, `h1`).
