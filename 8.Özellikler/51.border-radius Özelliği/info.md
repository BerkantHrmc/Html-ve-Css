# border-radius Özelliği

`border-radius`, HTML öğesinin köşelerini yuvarlatmak için kullanılır.

---

## Temel Kullanım

```css
div {
  border-radius: 10px;
}
```

Tüm köşeler 10px yuvarlatılır.

---

## Köşelere Özel Kullanım

```css
div {
  border-top-left-radius: 20px;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 5px;
  border-bottom-left-radius: 0;
}
```

Her köşe ayrı ayrı ayarlanabilir.

---

## Oval/Kapsül Şekli

```css
div {
  border-radius: 50%;
}
```

Kare öğeleri daire yapar.

---

## Yuvarlak Kenarlı Buton

```css
button {
  border-radius: 999px;
}
```

Tam yuvarlatılmış buton görünümü verir.
