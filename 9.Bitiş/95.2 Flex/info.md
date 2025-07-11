# CSS Dersleri - order, align-self, flex-grow, flex-basis, flex-shrink

---

## Kısa Tanıtım

- **order**: Öğelerin sırasını değiştirir.
- **align-self**: Tek bir öğeyi kendi hizasında özel konumlandırır.
- **flex-grow**: Öğenin kalan alanı büyütme oranını ayarlar.
- **flex-basis**: Öğenin başlangıç boyutunu belirler.
- **flex-shrink**: Öğenin küçülme oranını belirler.

---

## order

**order**, flex öğelerin sıralamasını değiştirir.

```css
.item {
  order: 2;
}
```

- Varsayılan: `0`
- Daha küçük değerler önce gelir.

---

## align-self

**align-self**, bir öğeyi kendi çapraz ekseninde farklı hizalar.

```css
.item {
  align-self: flex-end;
}
```

- Konteynerin `align-items` ayarını geçersiz kılar.

---

## flex-grow

**flex-grow**, bir öğenin boş alanı büyütme oranını ayarlar.

```css
.item {
  flex-grow: 1;
}
```

- `0`: Büyümez (varsayılan)
- `1`: Boş alanı paylaşır.
- Daha büyük sayı: Daha fazla büyür.

---

## flex-basis

**flex-basis**, öğenin başlangıç boyutunu belirler.

```css
.item {
  flex-basis: 150px;
}
```

- Varsayılan: `auto` (içerik boyutu)
- `flex-grow` ve `flex-shrink` ile birlikte çalışır.

---

## flex-shrink

**flex-shrink**, bir öğenin gerektiğinde küçülme oranını belirler.

```css
.item {
  flex-shrink: 1;
}
```

- Varsayılan: `1` (küçülür)
- `0`: Küçülmez.

---

## Örnek

```css
.container {
  display: flex;
}

.item1 {
  order: 2;
  flex-grow: 2;
  flex-basis: 100px;
}

.item2 {
  order: 1;
  flex-shrink: 0;
  align-self: flex-start;
}
```

- `.item2` önde yer alır.
- `.item1` iki kat fazla boş alan kaplar.
- `.item2` küçülmez ve üst hizaya yerleşir.
