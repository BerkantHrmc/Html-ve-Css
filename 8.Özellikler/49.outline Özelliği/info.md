# Outline Özelliği

`outline`, HTML öğesinin çevresine çizilen **kenarlığa benzer ama border'dan farklı** bir çizgidir.

---

## Özellikleri

- `outline`, öğenin **dışında** yer alır ve **kutunun boyutunu etkilemez**.  
- Genellikle **klavye ile odaklanıldığında** (`:focus`) tarayıcı tarafından otomatik olarak uygulanır.  
- `border` ile benzer görünse de **kenarlardan ayrı çalışır**.

---

## Temel Kullanım

```css
div {
  outline: 2px solid red;
}
```

---

## outline vs border

| Özellik       | border                         | outline                         |
|---------------|--------------------------------|----------------------------------|
| Yerleşim      | İç çerçeve                     | Dış çerçeve                      |
| Boyut etkisi  | Kutu boyutunu etkiler          | Etkilemez                        |
| Yuvarlama     | `border-radius` ile yuvarlanır | `outline` yuvarlanamaz          |

---

## Sık Kullanım

```css
input:focus {
  outline: 2px dashed blue;
}
```

---

## outline: none

```css
button:focus {
  outline: none;
}
```

Klavye odak çizgisini kaldırır. **Erişilebilirlik açısından dikkatli kullanılmalıdır.**

## outline-offset Özelliği

`outline-offset`, outline çizgisinin öğeden ne kadar uzakta olacağını belirler.

```css
div {
  outline: 2px solid red;
  outline-offset: 5px;
}
```

- Pozitif değer: Outline dışarı taşar  
- Negatif değer: Outline içeri yaklaşır
