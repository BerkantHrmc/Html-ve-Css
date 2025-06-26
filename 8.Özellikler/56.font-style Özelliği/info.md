# font-style Özelliği

`font-style`, metnin yazı tipinde eğiklik (italic) gibi stil değişiklikleri yapar.

---

## Değerler

- `normal` → Düz metin (varsayılan)
- `italic` → Eğik yazı
- `oblique` → Eğik yazı (italic'e benzer ama fontun kendi eğik versiyonu değilse tarayıcı eğik hale getirir)

---

## Örnek Kullanım

```css
p {
  font-style: italic;
}

span {
  font-style: normal;
}
```

---

## Not

`italic` ve `oblique` benzer görünür, ancak teknik olarak farklıdır. `italic`, fontun kendi eğik stilidir; `oblique`, yapay eğikliktir.
