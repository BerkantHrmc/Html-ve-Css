### `margin` Nedir?

`margin`, bir HTML öğesinin **kenarlığı ile diğer öğeler arasındaki dış boşluğu** ayarlamak için kullanılır. Öğeyi dışarıdan uzaklaştırır.

---

### `margin` vs `padding`

| Özellik   | Açıklama                              | Boşluk Konumu              |
|-----------|----------------------------------------|----------------------------|
| `padding` | İçeriği kenarlığa yaklaştırmaz         | İçerik ile kenarlık arası  |
| `margin`  | Öğeyi diğer öğelerden uzaklaştırır     | Kenarlık ile dış ortam arası |


### Satır İçi (Inline) Elemanlarda `margin`

- `margin-left` ve `margin-right`: ✅ Çalışır
- `margin-top` ve `margin-bottom`: ❌ Genellikle etkili olmaz
- Tam verim için: `display: inline-block;` kullanılmalıdır ✅

---

### Negatif `margin` Kullanımı

- `margin` değerleri negatif olabilir: `margin-top: -10px;`
- Bu, öğeyi belirtilen yönde **yaklaştırır** veya **üst üste bindirir**.
- Genellikle özel yerleşimlerde veya hizalamalarda kullanılır.
- ⚠️ Aşırı negatif kullanım tasarımı bozabilir.

---

### Örnek Kullanım:

```css
div {
  margin: 20px; /* Her yöne 20px dış boşluk */
}

div{
    margin: 100px 50px 60px;    /*ilk değer yukarı  , ikinci değer sağa sola , üçüncü aşşağıdan etki eder.*/
}


```

`yukarı sağ sol aşşağı şeklinde devam eder.`

---

### `margin: auto` Kullanımı

- `margin: auto` değeri, öğeyi **ortalamak** için kullanılır.
- Genellikle **yatayda ortalamak** için kullanılır (`margin-left` ve `margin-right`).
- Çalışması için öğeye `width` değeri verilmiş olmalıdır.

#### Örnek:

```css
div {
  width: 300px;
  margin: auto; /* Yatayda ortalar */
}

```
satır içi elemanlarda durum padding ile aynı
