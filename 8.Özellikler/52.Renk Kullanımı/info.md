# Renk Kullanımı

CSS'de renkler çeşitli biçimlerde tanımlanabilir. En yaygın yöntemler: renk anahtar kelimeleri, RGB ve HSL sistemleridir.

---

## Anahtar Kelimeler

```css
color: red;
background-color: blue;
```

Tanımlı renk isimleri kullanılır: `red`, `blue`, `black`, `white`, `gray`, `green` gibi.

---

## RGB Kullanımı

```css
color: rgb(255, 0, 0);       /* Kırmızı */
color: rgb(0, 255, 0);       /* Yeşil */
color: rgb(0, 0, 255);       /* Mavi */
```

- RGB: Kırmızı, Yeşil, Mavi
- Her bileşen 0–255 arası değer alır.

---

### RGBA (Alfa saydamlık)

```css
color: rgba(0, 0, 0, 0.5);   /* %50 saydam siyah */
```

---

## HSL Kullanımı

```css
color: hsl(0, 100%, 50%);    /* Kırmızı */
color: hsl(120, 100%, 50%);  /* Yeşil */
color: hsl(240, 100%, 50%);  /* Mavi */
```

- H: Renk açısı (0–360)  
- S: Doygunluk (%)  
- L: Açıklık (%)

---

### HSLA (Alfa saydamlık)

```css
color: hsla(0, 100%, 50%, 0.5);  /* %50 saydam kırmızı */
```
