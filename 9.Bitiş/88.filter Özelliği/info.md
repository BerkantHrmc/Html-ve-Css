# filter Özelliği

**filter**, bir öğeye CSS ile görsel efektler uygulamak için kullanılır. Görseller, arka planlar veya elementler üzerinde parlaklık, bulanıklık, gri tonlama gibi efektler verir.

---

## Ne İşe Yarar?

- Görsel dosyalar, arka planlar veya HTML öğelerine efekt ekler.
- Fotoğraf düzenleme benzeri işlemleri CSS ile yapmanı sağlar.
- Hover efektleriyle animasyonlarda sık kullanılır.

---

## Temel Kullanım

```css
img {
  filter: grayscale(100%);
}
```

Bu örnek, resmi siyah-beyaz yapar.

---

## Yaygın filter Fonksiyonları

| Fonksiyon | Açıklama |
|----------------|--------------------------------|
| **blur(px)** | Bulanıklaştırır |
| **brightness(%)** | Parlaklığı ayarlar |
| **contrast(%)** | Kontrastı ayarlar |
| **grayscale(%)** | Siyah-beyaz yapar |
| **invert(%)** | Renkleri ters çevirir |
| **opacity(%)** | Saydamlığı değiştirir |
| **saturate(%)** | Doygunluğu artırır/azaltır |
| **sepia(%)** | Sepya tonu uygular |
| **drop-shadow(x y blur color)** | Gölge efekti verir |

---

## Örnekler

```css
/* Bulanıklaştırma */
img {
  filter: blur(5px);
}

/* Parlaklık artırma */
img {
  filter: brightness(150%);
}

/* Kontrastı düşürme */
img {
  filter: contrast(50%);
}
```

---

## Not

- `filter` birden fazla fonksiyonla birlikte de kullanılabilir.
- Örnek: `filter: grayscale(50%) blur(2px);`
- Modern tarayıcılar tarafından desteklenir.
