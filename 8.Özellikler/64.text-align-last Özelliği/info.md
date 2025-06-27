# text-align-last Özelliği

`text-align-last`, çok satırlı bir metin bloğundaki **son satırın hizalamasını** belirler.

---

## Değerler

- `auto` → Varsayılan davranış (çoğunlukla `start`)
- `left` → Sola hizalar
- `right` → Sağa hizalar
- `center` → Ortalar
- `justify` → İki yana yaslar

---

## Örnek Kullanım

```css
p {
  text-align: justify;
  text-align-last: right;
}
```

Yukarıdaki örnekte tüm metin iki yana yaslanır, **yalnızca son satır sağa hizalanır**.

---

## Not

`text-align-last`, sadece `text-align: justify;` gibi çok satırlı hizalamalarda görünür etkisi olur.
