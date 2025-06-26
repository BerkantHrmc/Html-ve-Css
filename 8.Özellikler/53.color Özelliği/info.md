# color Özelliği

`color`, bir HTML öğesinin **metin rengini** ayarlamak için kullanılır.

---

## Temel Kullanım

```css
p {
  color: red;
}
```

Paragraf metni kırmızı olur.

---

## Renk Biçimleri

- Anahtar kelime: `red`, `blue`, `green`
- HEX kodu: `#ff0000`
- RGB: `rgb(255, 0, 0)`
- RGBA: `rgba(255, 0, 0, 0.5)`
- HSL: `hsl(0, 100%, 50%)`
- HSLA: `hsla(0, 100%, 50%, 0.5)`

---

## Örnek

```css
h1 {
  color: hsl(240, 100%, 50%);
}

span {
  color: rgba(0, 0, 0, 0.7);
}
```

Metin renkleri görsel tasarımda vurgu ve okunabilirlik için kullanılır.

---

`color`, metin rengini belirler ve genellikle **ebeveynden çocuklara miras alır**.

---

## Örnek Kullanım

```css

<body>

<div></div>

</body>

```
---

body'e renk verirsen div ondan miras alır.