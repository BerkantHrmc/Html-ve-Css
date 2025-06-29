# background-repeat Özelliği

`background-repeat`, bir öğenin arka plan resminin nasıl tekrar edeceğini belirler.

---

## Temel Kullanım

```css
div {
  background-image: url("desen.png");
  background-repeat: repeat;
}
```

Varsayılan değer `repeat`tir ve resim hem yatay hem dikey tekrar eder.

---

## Değerler

- `repeat` → Hem yatay hem dikey tekrar eder (varsayılan)
- `repeat-x` → Sadece yatayda tekrar eder
- `repeat-y` → Sadece dikeyde tekrar eder
- `no-repeat` → Tek bir kez gösterilir, tekrar etmez
- `space` → Resim aralarına boşluk ekleyerek tekrar eder.Sığdığı kadar sığdırır
- `round` → Resmi sığacak şekilde ölçekler ve tekrar eder

---

## Örnekler

```css
.box1 {
  background-image: url("bg.png");
  background-repeat: no-repeat;
}

.box2 {
  background-image: url("bg.png");
  background-repeat: repeat-x;
}

.box3 {
  background-image: url("bg.png");
  background-repeat: round;
}
```

---

## Not

`background-repeat`, arka planın kaplama şeklini belirlemek için `background-position` ve `background-size` ile birlikte kullanılır.
