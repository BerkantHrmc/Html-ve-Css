# box-sizing Özelliği

`box-sizing`, bir öğenin genişlik (`width`) ve yükseklik (`height`) değerlerinin nasıl hesaplanacağını belirler.

---

## Değerler

### content-box (Varsayılan)

```css
div {
  box-sizing: content-box;
}
```

- `width` ve `height` sadece içeriği kapsar.  
- `padding` ve `border` dışına eklenir.  
- Toplam kutu boyutu: **içerik + padding + border**

---

### border-box (Tavsiye Edilen)

```css
div {
  box-sizing: border-box;
}
```

- `width` ve `height` tüm kutuyu kapsar (içerik + padding + border).  
- Kutu dışarı taşmaz, daha kontrollü tasarım sağlar.
- yani şöyle diyebilriz diyelim 200 e 200 bir div'im var ve 10 padding ve 10 border ekliyorum 
box-sizing: border-box dersem yeni boyutlarım yine 200 e 200 olur border ve border ona göre ayarlanır(
220 ye 220 olmaz). 

---

## Tüm Sayfaya Uygulama

```css
* {
  box-sizing: border-box;
}
```

Tüm öğelerde tutarlı kutu modeli sağlar.
