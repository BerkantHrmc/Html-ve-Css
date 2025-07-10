# CSS Dersleri - Flex

---

## Flex Nedir?

**Flex**, bir konteyner içindeki öğeleri esnek bir şekilde hizalamak ve yerleştirmek için kullanılan bir düzen modelidir.

- Ana kapsayıcıya (`display: flex;`) uygulanır.
- İçindeki elemanlar **flex item** olur.
- Kolay hizalama, boşluk yönetimi ve esnek yerleşim sağlar.

---

## Temel Kurulum

```css
.container {
  display: flex;
}
```

- `.container` bir **flex konteyner** olur.
- İçindeki öğeler otomatik olarak yatayda (row) hizalanır.

---

## Sık Kullanılan Özellikler

### `flex-direction`

Öğelerin ana eksen yönünü belirler.

```css
.container {
  flex-direction: row; /* varsayılan */
}

.container {
  flex-direction: column; /* dikey hizalama */
}
```

---

### `justify-content`

Ana eksende hizalama yapar (yatayda).

```css
.container {
  justify-content: center; /* Ortala */
  justify-content: space-between; /* Arada boşluk */
}
```

---

### `align-items`

Çapraz eksende hizalama yapar (dikeyde).

```css
.container {
  align-items: center; /* Ortala */
  align-items: flex-start; /* Üste yasla */
}
```

---

### `flex-wrap`

Öğelerin taşma durumunda satır atlayıp atlamayacağını belirler.

```css
.container {
  flex-wrap: wrap;
}
```

---

### `gap`

Flex öğeleri arasına boşluk ekler.

```css
.container {
  gap: 20px;
}
```

---

### `flex` (Öğe Bazında)

Bir öğenin ne kadar yer kaplayacağını ayarlar.

```css
.item {
  flex: 1; /* Eşit genişlik */
}
```

---

## Özet Avantajları

✅ Karmaşık grid yapılar yerine daha esnek yerleşim sağlar.  
✅ Dikey ve yatay hizalama kolaydır.  
✅ Responsive (esnek) tasarımlar için idealdir.

---

## Örnek

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 10px;
}
```

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```
