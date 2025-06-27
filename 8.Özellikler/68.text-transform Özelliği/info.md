# text-transform Özelliği

`text-transform`, metindeki harflerin **büyük/küçük** biçimlendirmesini kontrol eder.

---

## Değerler

- `none` → Varsayılan, metin olduğu gibi görünür  
- `uppercase` → Tüm harfleri **büyük harfe** çevirir  
- `lowercase` → Tüm harfleri **küçük harfe** çevirir  
- `capitalize` → Her kelimenin **ilk harfini büyük** yapar

---

## Örnek Kullanım

```css
p {
  text-transform: uppercase;
}

h1 {
  text-transform: capitalize;
}

span {
  text-transform: lowercase;
}
```

---

## Not

`text-transform` sadece **görsel olarak** etki eder, HTML içeriğini değiştirmez.
