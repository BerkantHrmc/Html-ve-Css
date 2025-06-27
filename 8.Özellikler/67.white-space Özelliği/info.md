# white-space Özelliği

`white-space`, HTML metninde boşluk, tab ve satır sonu karakterlerinin nasıl işlendiğini kontrol eder.

---

## <pre> Etiketi ve Varsayımı

`<pre>` etiketi, metni olduğu gibi (boşluklar ve satır sonlarıyla birlikte) gösterir. Bu etki CSS'te `white-space: pre;` ile sağlanır.

```html
<pre>
Bu   metin   
    olduğu gibi      görünür.
</pre>
```

---

# white-space Özelliği

`white-space`, boşluk karakterlerinin ve satır sonlarının metin içinde nasıl işlendiğini belirler.

---

## Değerler

- `normal` → Fazla boşluklar yok sayılır, satır otomatik sarılır (varsayılan)
- `nowrap` → Satır sarma olmaz, metin tek satırda kalır
- `pre` → Boşluklar ve satır sonları korunur, sarma olmaz
- `pre-wrap` → Boşluklar ve satır sonları korunur, metin sarılır
- `pre-line` → Satır sonları korunur, fazla boşluklar kırpılır

---

## Örnek Kullanım

```css
p {
  white-space: pre-wrap;
}
```

---

## Not

Özellikle boşluk duyarlı düzenlerde (`kod`, `şiir`, `tablo`) veya `<pre>` benzeri davranış istenen durumlarda kullanılır.
