# column Özellikleri

`column` özellikleri, bir öğenin içeriğini **çok sütunlu (multi-column) bir düzenle** bölmek için kullanılır.

---

## Neden Kullanılır?

- Metin veya içerikleri gazete sayfası gibi sütunlara ayırmak için.
- Uzun içerikleri daha düzenli ve okunabilir hale getirmek için.

---

## Temel Özellikler

### 1️⃣ column-count

Kaç sütun olacağını belirler.

```css
.text {
  column-count: 3;
}
```

Bu örnek `.text` içeriğini 3 sütuna böler.

---

### 2️⃣ column-width

Sütun genişliğini belirtir. Tarayıcı, bu genişliğe uygun sayıda sütun oluşturur.

```css
.text {
  column-width: 200px;
}
```

---

### 3️⃣ column-gap

Sütunlar arasındaki boşluğu belirler.

```css
.text {
  column-gap: 40px;
}
```

---

### 4️⃣ column-rule

Sütunlar arasına çizgi (ayırıcı) ekler.

```css
.text {
  column-rule: 2px solid gray;
}
```

---

## Kısa Kullanım

`column-count` ve `column-width` birlikte `columns` ile yazılabilir.

```css
.text {
  columns: 2 150px;
}
```

Bu örnek `.text` içeriğini en az 2 sütuna böler, sütun genişliği yaklaşık 150px olur.

---

## Örnek

```css
.article {
  column-count: 2;
  column-gap: 30px;
  column-rule: 1px solid #ccc;
}
```

---

## Not

- `column` özellikleri blok seviyesindeki öğelerde çalışır.
- Çok sütunlu düzen, responsive tasarımlar için de uygundur.
