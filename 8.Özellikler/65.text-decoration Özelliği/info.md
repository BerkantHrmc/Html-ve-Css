# text-decoration Özelliği

`text-decoration`, metne çizgi eklemek veya çizgiyi kaldırmak için kullanılır.

---

## Değerler

- `none` → Çizgi yok  
- `underline` → Altı çizili  
- `overline` → Üstü çizili  
- `line-through` → Üstü çizili (üstünü çizme efekti)  
- `blink` → Yanıp sönen metin (tarayıcı desteği yok denecek kadar az)

---

## Örnek Kullanım

```css
a {
  text-decoration: none;
}

h1 {
  text-decoration: underline;
}

del {
  text-decoration: line-through;
}
```

---

## Kısayol Kullanım (Shorthand)

```css
text-decoration: underline red wavy;
```

- Sırasıyla: çizgi türü, renk, stil (solid, double, dotted, dashed, wavy)

---

## Not

`text-decoration`, bağlantı (a) etiketlerinin alt çizgisini kaldırmak veya özel çizgi stilleri oluşturmak için sıkça kullanılır.
