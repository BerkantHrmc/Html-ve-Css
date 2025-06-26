# font-size Özelliği

`font-size`, bir öğedeki metnin boyutunu belirler.

---

## Temel Kullanım

```css
p {
  font-size: 16px;
}
```

---

## Birim Türleri

- **px** → Piksel (sabit)
- **em** → Ebeveyn öğeye göre
- **rem** → Kök öğeye göre (html)
- **%** → Yüzdelik değer
- **vw/vh** → Görüntü alanına göre

---

## Anahtar Kelimeler

```css
small     → Küçük
medium    → Orta (varsayılan)
large     → Büyük
x-small   → Çok küçük
x-large   → Çok büyük
xx-small  → En küçük
xx-large  → En büyük
```

---

## Örnek

```css
h1 {
  font-size: x-large;
}

span {
  font-size: 120%;
}

div {
  font-size: 1.2rem;
}
```

---

## Not

Anahtar kelimeler tarayıcıya göre değişebilir. Tutarlı tasarımlar için `rem` veya `px` tercih edilir.
