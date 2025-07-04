# transform Özelliği

**transform**, bir HTML öğesini 2D veya 3D düzlemde taşımak, döndürmek, ölçeklendirmek veya eğmek için kullanılan CSS özelliğidir.

---

## Ne İşe Yarar?

- Öğeyi konumlandırmak.
- Döndürmek.
- Büyütmek/küçültmek.
- Eğmek.
- Animasyon ve geçiş efektlerinde kullanılmak.

---

## Temel Kullanım

```css
.box {
  transform: rotate(45deg);
}
```

Bu örnek, `.box` öğesini 45 derece döndürür.

---

## Sık Kullanılan transform Fonksiyonları

| Fonksiyon | Açıklama |
|------------------|----------------------------|
| **translate(x, y)** | Taşır |
| **rotate(deg)** | Döndürür |
| **scale(x, y)** | Ölçekler |
| **skew(x, y)** | Eğim verir |
| **matrix()** | 2D transform parametrelerini tek satırda belirtir |
| **perspective(n)** | 3D perspektif ekler |

---

## Örnekler

```css
/* Sağa 100px taşı */
.box {
  transform: translateX(100px);
}

/* 60 derece döndür */
.box {
  transform: rotate(60deg);
}

/* 1.5 kat büyüt */
.box {
  transform: scale(1.5);
}

/* X ekseninde 15 derece eğ */
.box {
  transform: skewX(15deg);
}

/* Birden fazla transform */
.box {
  transform: translate(50px, 50px) rotate(30deg) scale(1.2);
}
```

---

## Not

- Birden fazla transform fonksiyonu boşlukla ayrılarak aynı anda uygulanabilir.
- `transform` genelde `transition` ile kombinlenir.
- `transform-origin` dönüşüm noktasını belirler.
