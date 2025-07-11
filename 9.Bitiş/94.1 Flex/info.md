# CSS Dersleri - Flex


## Flex Nedir?

**Flex**, bir kapsayıcı içindeki öğeleri esnek ve düzenli bir şekilde hizalamak için kullanılan CSS düzen modelidir.

- `display: flex;` ile tanımlanır.
- İçindeki elemanlar **flex item** olur.
- Karmaşık hizalama problemlerini basit çözer.

---

## Temel Kullanım

```css
.container {
  display: flex;
}
```

- `.container` artık bir **flex konteyner** olur.
- İçindeki elemanlar yatayda (row) hizalanır (varsayılan).

---

## Sık Kullanılan Flex Özellikleri

### `flex-direction`

Öğelerin yönünü belirler.

```css
.container {
  flex-direction: row; /* Yatay - varsayılan */
}

.container {
  flex-direction: column; /* Dikey */
}
```

---

### `justify-content`

Ana eksende hizalama yapar.

```css
.container {
  justify-content: center; /* Ortalar */
  justify-content: space-between; /* Boşluk bırakır */
  justify-content: space-around; /* Etrafına boşluk ekler */
}
```

---

### `align-items`

Çapraz eksende hizalama yapar.

```css
.container {
  align-items: center; /* Ortalar */
  align-items: flex-start; /* Üst hizalar */
  align-items: flex-end; /* Alt hizalar */
}
```

---

### `flex-wrap`

Öğeler taşarsa alt satıra geçer.

```css
.container {
  flex-wrap: wrap;
}
```

---

### `gap`

Flex öğeleri arasında boşluk bırakır.

```css
.container {
  gap: 20px;
}
```

---

### `flex` (Öğe Bazında)

Öğelerin alan paylaşımını ayarlar.

```css
.item {
  flex: 1; /* Eşit paylaşım */
}

.item {
  flex: 2; /* Diğerlerinden 2 kat fazla yer kaplar */
}
```

---

## Avantajlar

✅ Yatay ve dikey hizalama kolaydır.  
✅ Responsive tasarımlar için uygundur.  
✅ Karmaşık düzenlerde pratik çözüm sunar.

---

## Basit Örnek

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 15px;
}
```
