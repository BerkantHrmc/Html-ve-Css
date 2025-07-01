# position Özelliği

`position`, bir HTML öğesinin **belirli bir konumda nasıl yerleşeceğini** ve **diğer öğelerle nasıl etkileşeceğini** belirler.

---

## Neden Kullanılır?

- Öğeyi sabitlemek.
- Belirli bir alana konumlandırmak.
- Üst üste yerleşim sağlamak (`z-index`).
- Düzen akışını kırarak mutlak/bağlı yerleşim oluşturmak.

---

## Yaygın position Değerleri

- **static**  
  Varsayılan konumlandırmadır. Öğeler normal akışa göre yerleşir. `top`, `left` gibi konum değerleri işlemez.

  ```css
  div {
    position: static;
  }
  ```

- **relative**  
  Öğeyi normal konumundan göreli olarak taşır. `top`, `left`, `right`, `bottom` değerleri geçerli olur.

  ```css
  .box {
    position: relative;
    top: 20px;
    left: 10px;
  }
  ```

- **absolute**  
  Öğeyi en yakın `position: relative`, `absolute`, `fixed` veya `sticky` üst öğesine göre konumlandırır. Böyle bir üst yoksa sayfanın `body` öğesine göre konumlanır.

  ```css
  .absolute-box {
    position: absolute;
    top: 50px;
    left: 30px;
  }
  ```

- **fixed**  
  Öğeyi ekran görünümüne sabitler. Scroll yapılsa bile aynı yerde kalır.

  ```css
  .fixed-header {
    position: fixed;
    top: 0;
    width: 100%;
  }
  ```

- **sticky**  
  Öğeyi normal akışta başlatır, belirlenen kaydırma noktasına gelince sabitlenir. Hem `relative` hem `fixed` davranışı taşır.

  ```css
  .sticky {
    position: sticky;
    top: 0;
  }
  ```

---

## Örnek

```css
.container {
  position: relative;
}

.child {
  position: absolute;
  top: 20px;
  right: 30px;
}
```

Bu örnekte `.child` mutlak konumlanır ve `.container` içine bağlıdır.

---

## Not

- `z-index` sadece `position` değeri `relative`, `absolute`, `fixed` veya `sticky` olan öğelerde çalışır.
- `static` en basit akıştır, konumlama yapılmaz.
