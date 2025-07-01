# transition Özelliği

`transition`, bir öğenin CSS özelliklerinin **bir değerden diğerine yumuşak geçişle değişmesini** sağlar.

---

## Neden Kullanılır?

- Hover, focus gibi durumlarda ani değişimleri akıcı hale getirir.
- Renk, boyut, konum gibi özellik değişimlerini yumuşatır.
- JavaScript olmadan basit animasyon efekti sağlar.

---

## Temel Kullanım

```css
.box {
  transition: all 0.3s ease;
}
```

Bu örnekte `.box` üzerindeki tüm geçişler 0.3 saniyede ve `ease` hız eğrisiyle gerçekleşir.

---

## Parçaları

- **transition-property**  
  Geçiş yapılacak özellik.  
  Örn: `width`, `opacity`, `transform`.

- **transition-duration**  
  Geçişin ne kadar süreceği.  
  Örn: `0.5s`, `200ms`.

- **transition-timing-function**  
  Geçişin hız eğrisi. Hareketin başlama, hızlanma ve bitiş şeklini ayarlar.  
  Yaygın değerler:  
  - `ease` → Yavaş başlar, hızlanır, yavaş biter (varsayılan)  
  - `linear` → Sabit hızda geçiş  
  - `ease-in` → Yavaş başlar, hızlanarak biter  
  - `ease-out` → Hızlı başlar, yavaş biter  
  - `ease-in-out` → Yavaş başlar, hızlanır, yavaş biter  
  - `cubic-bezier` → Özel hız eğrisi tanımlamak için kullanılır.  
  Örn: `cubic-bezier(0.25, 0.1, 0.25, 1)`

- **transition-delay**  
  Geçiş başlamadan önceki gecikme süresi.

---

## Kısa Kullanım

```css
.box {
  transition: background-color 0.4s ease-in-out 0.2s;
}
```

---

## Örnek

```css
.button {
  background: blue;
  transition: background 0.5s ease-out;
}

.button:hover {
  background: red;
}
```

Bu örnekte `.button` hover olunca arka plan rengi mavi iken kırmızıya `ease-out` hız eğrisiyle geçer.

---

## Not

- `transition` yalnızca sayısal değişebilen özelliklerde çalışır: renk, boyut, konum, opacity, transform vb.
- `display` gibi ani değişen özelliklerde geçiş uygulanamaz.
