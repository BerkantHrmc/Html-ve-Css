# font-variant Özelliği

`font-variant`, metindeki küçük harfleri **küçük büyük harf (small-caps)** biçiminde gösterir.

---

## Değerler

- `normal` → Varsayılan yazım (küçük harfler küçük kalır)
- `small-caps` → Küçük harfleri büyük harf gibi ama daha küçük boyutta gösterir

---

## Örnek Kullanım

```css
p {
  font-variant: small-caps;
}
```

"merhaba dünya" → “MERHABA DÜNYA” gibi görünür, ama büyük harf boyutundan daha küçüktür.

---

## Not

Tüm yazı tipleri `small-caps` desteği sunmayabilir. Görsel tutarlılık için uygun font seçilmelidir.
