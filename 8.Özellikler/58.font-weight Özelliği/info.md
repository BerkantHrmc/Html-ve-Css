# font-weight Özelliği

`font-weight`, metnin kalınlığını (boldluk derecesini) belirler.

---

## Değerler

### Anahtar Kelimeler

- `normal` → Varsayılan kalınlık  
- `bold` → Kalın metin  
- `lighter` → Ebeveynine göre daha ince  
- `bolder` → Ebeveynine göre daha kalın

### Sayısal Değerler

```css
font-weight: 100;   /* En ince */
font-weight: 400;   /* Normal (eşittir normal) */
font-weight: 700;   /* Kalın (eşittir bold) */
font-weight: 900;   /* En kalın */
```

Değerler 100 ile 900 arasında gider (100’erlik artışlarla).

---

## Örnek Kullanım

```css
h1 {
  font-weight: bold;
}

p {
  font-weight: 300;
}
```

---

## Not

Her yazı tipi tüm ağırlıkları desteklemeyebilir. Uyumlu font seçmek önemlidir.
