# CSS Dersleri - overflow, scrollbar

---

## Kısa Tanıtım

- **overflow**: Bir kutu içeriğinin kutunun boyutlarını aşıp aşmadığında ne olacağını belirler.
- **scrollbar**: Kutu taşarsa kaydırma çubuğu (scroll bar) gösterilmesini sağlar.

---

## overflow

**overflow**, bir öğenin içerikleri belirtilen genişlik/yükseklik sınırını aşarsa ne yapılacağını ayarlar.

```css
div {
  overflow: auto;
}
```

- `visible`: Taşan içerik görünür (varsayılan).  
- `hidden`: Taşan içerik gizlenir.  
- `scroll`: Her zaman kaydırma çubuğu çıkar.  
- `auto`: Gerekirse kaydırma çubuğu çıkar.

---

## Örnek

```css
.box {
  width: 200px;
  height: 100px;
  overflow: scroll;
}
```

- İçerik kutuya sığmazsa yatay/dikey kaydırma çubuğu çıkar.

---

## scrollbar

**scrollbar**, overflow özelliği ile birlikte içerik taşarsa otomatik olarak çıkar. Özel tarayıcı destekli stillerle kaydırma çubuğunun görünümü de değiştirilebilir.

### Örnek: WebKit Scrollbar Stil

```css
/* Tüm scroll bar */
::-webkit-scrollbar {
  width: 8px;
}

/* Scroll bar track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Scroll bar thumb */
::-webkit-scrollbar-thumb {
  background: #888;
}

/* Scroll bar hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}
```

- Bu örnekle kaydırma çubuğu genişliği, rengi ve hover durumu özelleştirilebilir.
- Sadece WebKit tabanlı tarayıcılarda çalışır (Chrome, Safari).

---

## Not

- `overflow-x` ve `overflow-y` ile yatay/dikey taşmalar ayrı kontrol edilebilir.
- `scrollbar-width` ve `scrollbar-color` gibi modern özellikler Firefox tarafından da desteklenir.
