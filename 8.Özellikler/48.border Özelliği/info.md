# Border Özelliği

`border`, HTML öğesinin çevresine çerçeve (kenarlık) eklemek için kullanılır. Öğenin görsel sınırlarını belirler.

1.border-style
2.border-width
3.border-color
4.border

## 1. border-style Özelliği

`border-style`, kenarlığın çizgi şeklini belirler. Aşağıdaki değerlerden biri veya birkaçı kullanılabilir:

- `none` → Kenarlık yoktur  
- `solid` → Düz çizgi  
- `dashed` → Kesik çizgi  
- `dotted` → Noktalı çizgi  
- `double` → Çift çizgi  
- `groove`, `ridge`, `inset`, `outset` → 3D görünümlü kenarlıklar (gölgeli efekt)

Örnek:

```css
div {
  border-style: dashed;
}
```

## 2. border-width Özelliği

`border-width`, kenarlığın kalınlığını belirler. Piksel (px), em, rem gibi birimler kullanılabilir.

**Tek değer:**
```css
div {
  border-width: 3px;
}
```
Tüm kenarlar 3px olur.

**Dört değer sırasıyla:**

```css
div {
  border-width: 2px 4px 6px 8px;
}
```
- Üst: 2px  
- Sağ: 4px  
- Alt: 6px  
- Sol: 8px

**Kısayol isimler:**

- `thin`, `medium`, `thick`

```css
div {
  border-width: thick;
}
```

## 3.border-color Özelliği


`border-color`, HTML öğesinin kenarlık rengini belirlemek için kullanılır.


***Tek Değer**

```css
div {
  border-color: red;
}
```

Tüm kenarlar kırmızı olur.

---

**Çoklu Değer (Saat yönünde)**

```css
div {
  border-color: red green blue yellow;
}

```




## 4.border (Temel Kullanım)

```css
div {
  border: 2px solid black;
}
```
 `kalınlık , stil ,renk`

- `2px`: Kenarlığın kalınlığı  
- `solid`: Kenarlığın stili (`solid`, `dashed`, `dotted`, `double`, `none`)  
- `black`: Kenarlığın rengi

```css
div {
  border-top: 1px solid red;       /* Üst kenar: 1px kalın, düz çizgi, kırmızı */
  border-right: 2px dashed blue;   /* Sağ kenar: 2px kalın, kesik çizgi, mavi */
  border-bottom: 3px dotted green; /* Alt kenar: 3px kalın, noktalı çizgi, yeşil */
  border-left: 4px double purple;  /* Sol kenar: 4px kalın, çift çizgi, mor */
}
```


---


## border: none Ne Yapar?

```css
div {
  border: none;
}
```

- Kenarlığı tamamen kaldırır.

---

## Kullanım Amaçları

- Öğeleri vurgulamak  
- Alanları ayırmak  
- Kutu görünümü vermek

## Varsayılan Border Olan Etiketler

Bazı HTML etiketleri tarayıcılar tarafından varsayılan olarak kenarlıklı gelir:

- `input`  
- `textarea`  
- `button`  
- `fieldset`  
- `iframe`

Bu kenarlıkları kaldırmak için:

```css
input, textarea, button, fieldset, iframe {
  border: none;
}
```
