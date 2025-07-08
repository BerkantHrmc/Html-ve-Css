# appearance

**appearance**, bir HTML öğesinin tarayıcıya özgü yerleşik stilini kaldırmak veya değiştirmek için kullanılır.

```css
input {
  appearance: none;
}
```

- Özellikle form elemanlarında (input, select) tarayıcı varsayılan stilini devre dışı bırakmak için kullanılır.

---

# user-select

**user-select**, bir öğedeki metnin seçilip seçilemeyeceğini belirler.

```css
p {
  user-select: none;
}
```

- `none`: Metin seçilemez.  
- `text`: Metin seçilebilir (varsayılan).  
- `all`: Tıklayınca tüm içerik seçilir.  
- `auto`: Tarayıcı varsayılanı.

---

# calc()

**calc()**, CSS’te bir ölçü birimini matematiksel işlemlerle hesaplamak için kullanılır.

```css
div {
  width: calc(100% - 50px);
}
```

- Sabit ve yüzde birimlerini birleştirmek için idealdir.
- Toplama (+), çıkarma (-), çarpma (*), bölme (/) yapılabilir.
- Arada boşluk bırakmak zorunludur: `calc(50% + 20px)` gibi.

---

# ::file-selector-button

**::file-selector-button**, `<input type="file">` öğesindeki dosya seç butonunun stilini değiştirmek için kullanılır.

```css
input::file-selector-button {
  background: #333;
  color: #fff;
  border: none;
  padding: 8px 12px;
  cursor: pointer;
}
```

- Sadece `<input type="file">` içindeki butona özel stillendirme sağlar.
- Modern tarayıcılar tarafından desteklenir.
# CSS Dersleri - appearance, user-select, calc(), ::file-selector-button

---

## Kısa Tanıtımlar

- **appearance**: Öğenin tarayıcıya özel varsayılan stilini devre dışı bırakır.
- **user-select**: Metnin seçilebilir olup olmadığını belirler.
- **calc()**: CSS ölçülerinde matematiksel işlem yapılmasını sağlar.
- **::file-selector-button**: Dosya seç butonunun stilini değiştirmek için kullanılır.

---

## appearance

**appearance**, bir HTML öğesinin tarayıcıya özel varsayılan stilini kaldırmak veya değiştirmek için kullanılır.

```css
input {
  appearance: none;
}
```

- Genelde `<input>`, `<select>` gibi form elemanlarında kullanılır.

---

## user-select

**user-select**, bir öğedeki metnin seçilip seçilemeyeceğini kontrol eder.

```css
p {
  user-select: none;
}
```

- `none`: Seçilemez  
- `text`: Seçilebilir (varsayılan)  
- `all`: Tıklanınca tüm içerik seçilir  
- `auto`: Tarayıcı varsayılanı

---

## calc()

**calc()**, CSS ölçülerinde hesaplama yapmak için kullanılır.

```css
div {
  width: calc(100% - 50px);
}
```

- Farklı birimleri birleştirir.
- +, -, *, / işlemleri yapılabilir.
- Operatörlerin etrafında boşluk olmalıdır.

---

## ::file-selector-button

**::file-selector-button**, `<input type="file">` öğesindeki dosya seç butonuna özel stil vermek için kullanılır.

```css
input::file-selector-button {
  background: #333;
  color: #fff;
  border: none;
  padding: 8px 12px;
  cursor: pointer;
}
```

- Sadece dosya seç düğmesine stil uygular.
- Modern tarayıcılar destekler.
