# display Özelliği

`display`, bir HTML öğesinin **ekranda nasıl kutu modeli davranışıyla görüntüleneceğini** belirleyen en temel CSS özelliklerinden biridir.

---

## Temel Amaç

- Bir öğeyi **blok**, **satır içi (inline)**, **satır içi blok (inline-block)** gibi farklı kutu türlerine dönüştürmek.
- Öğenin düzen akışındaki davranışını değiştirmek.
- Görünüm ve düzenlemelerde esneklik sağlamak.

---

## Yaygın display Değerleri

- **block**  
  Öğeyi blok kutu haline getirir. Tam genişlik kaplar, yeni satıra geçer.  
  Örnek: `<div>`, `<p>`

  ```css
  div {
    display: block;
  }
  ```

- **inline**  
  Satır içi öğedir, genişlik-yükseklik ayarlanamaz, yan yana dizilir.  
  Örnek: `<span>`, `<a>`

  ```css
  span {
    display: inline;
  }
  ```

- **inline-block**  
  Satır içi gibi yan yana durur, blok gibi genişlik-yükseklik alabilir.

  ```css
  button {
    display: inline-block;
  }
  ```

- **none**  
  Öğeyi tamamen gizler, sayfa akışından çıkarır.

  ```css
  .hidden {
    display: none;
  }
  ```

- **flex**  
  Öğeyi bir **flex container** yapar. İçindeki çocukları esnek kutular haline getirir.

  ```css
  .container {
    display: flex;
  }
  ```

- **grid**  
  Öğeyi bir **grid container** yapar. Izgara düzeni oluşturur.

  ```css
  .grid {
    display: grid;
  }
  ```

---

## Notlar

- `visibility: hidden` öğeyi görünmez yapar ama yerini korur.  
  `display: none` ise hem görünmez yapar hem yerini kaldırır.
- `display` değeri, öğenin kutu modeli davranışını tamamen değiştirir.
- Düzen tasarımında esnek grid ve flex sistemleri için `display` temeldir.

---

## Örnek

```css
.box {
  display: inline-block;
  width: 100px;
  height: 50px;
  background: orange;
}
```
Bu örnekte `.box` hem satır içinde yer alabilir hem de boyutlandırılabilir.
