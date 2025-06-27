# word-break, overflow-wrap ve hyphens Özellikleri

Bu üç özellik, uzun kelimelerin veya satıra sığmayan metinlerin nasıl kırılacağını ve sarılacağını kontrol eder.

---

## word-break

Uzun kelimelerin satır sonunda nasıl kırılacağını belirler.

### Değerler:

- `normal` → Kelimeler gerektiğinde kırılır, ancak çok uzun kelimeler taşabilir  
- `break-all` → Gerekirse kelimenin herhangi bir yerinden kırılır  
- `keep-all` → Asla kelimeyi bölmez (özellikle Asya dillerinde kullanılır)

### Örnek:

```css
p {
  word-break: break-all;
}
```

---

## overflow-wrap (eski adıyla word-wrap)

Satıra sığmayan kelimelerin zorla kırılıp kırılmayacağını belirler.

### Değerler:

- `normal` → Kelime sığmazsa taşabilir  
- `break-word` → Gerekirse kelimeyi parçalayarak satıra sığdırır

### Örnek:

```css
div {
  overflow-wrap: break-word;
}
```

---

## hyphens

Kelimelerin **heceleme** kurallarına göre kesilmesini sağlar (tarayıcı desteğine bağlıdır).

### Değerler:

- `none` → Heceleme yapılmaz  
- `manual` → Sadece `<wbr>` veya `&shy;` ile belirlenen yerlerden kesilir  
- `auto` → Tarayıcı uygun gördüğü yerde otomatik olarak heceler

### Örnek:

```css
p {
  hyphens: auto;
}
```

---

## Not

- `word-break` → kelimeyi **zorla** kırar  
- `overflow-wrap` → sadece **taşan** kelimeler için  
- `hyphens` → **heceleme** ile kırma yapar  
Bu özellikler, özellikle uzun URL’ler, teknik terimler veya dar alanlı tasarımlarda kullanışlıdır.
