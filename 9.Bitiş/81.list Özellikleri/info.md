# HTML Listeler ve CSS list-style Özellikleri

Bu dosya, **düzenli ve düzensiz listeler**, `list-style` özellikleri ve özel sayaç kullanımı (counter-reset) konularını kapsar.

---

## Düzenli (Ordered) ve Düzensiz (Unordered) Listeler

- **Düzensiz Liste (`<ul>`)**  
  Sırasız, madde işaretli liste.
  ```html
  <ul>
    <li>Elma</li>
    <li>Armut</li>
  </ul>
  ```

- **Düzenli Liste (`<ol>`)**  
  Sıralı, numaralı liste.
  ```html
  <ol>
    <li>Birinci</li>
    <li>İkinci</li>
  </ol>
  ```

---

## list-style-type

`list-style-type` işaret veya numara biçimini belirler.

Örnek değerler:
- `disc` (•) → Düzensiz listeler için varsayılan.
- `circle` (○)
- `square` (■)
- `decimal` (1, 2, 3)
- `lower-alpha` (a, b, c)
- `upper-alpha` (A, B, C)
- `upper-roman` (I, II, III)

```css
ul {
  list-style-type: circle;
}

ol {
  list-style-type: upper-roman;
}
```

---

## list-style-position

İşaretin veya numaranın metne göre konumunu belirler.

- `outside` → İşaret metnin dışında başlar (varsayılan).
- `inside` → İşaret metin hizasında içeride başlar.

```css
ul {
  list-style-position: inside;
}
```

---

## list-style-image

İşaret yerine özel bir görsel kullanılır.

```css
ul {
  list-style-image: url("icon.png");
}
```

Eğer görsel bulunamazsa `list-style-type` devreye girer.

---

## list-style (Kısa Kullanım)

Üç özellik (type, position, image) tek satırda tanımlanabilir.

```css
ul {
  list-style: square inside url("icon.png");
}
```

---

## Listeyle Sayaç Oluşturma (counter-reset)

`counter-reset` ve `counter-increment` ile listeyi özelleştirilmiş numaralandırma için kullanabilirsiniz.

Örnek:

```html
<ol class="custom-counter">
  <li>Madde</li>
  <li>Madde</li>
</ol>
```

```css
.custom-counter {
  counter-reset: my-counter;
  list-style: none;
}

.custom-counter li {
  counter-increment: my-counter;
}

.custom-counter li::before {
  content: counter(my-counter) ". ";
  font-weight: bold;
}
```

Burada liste işareti gizlenir (`list-style: none`) ve her `li` öğesi kendi numarasını `::before` ile alır.

---

## Not

Listeyi tamamen işaretsiz yapmak için `list-style: none;` kullanılır. Özel ikon, sayaç veya CSS tabanlı simge eklenir.
