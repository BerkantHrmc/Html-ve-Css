# scroll-behavior, scroll-margin

---

## Kısa Tanıtım

- **scroll-behavior**: Sayfanın kaydırma hareketini ani mi yoksa yumuşak mı yapacağını belirler.
- **scroll-margin**: Bir öğeye kaydırıldığında kenarda boşluk bırakılmasını sağlar.

---

## scroll-behavior

**scroll-behavior**, sayfanın kaydırma davranışını ayarlar.

```css
html {
  scroll-behavior: smooth;
}
```

- `auto`: Anında kaydırır (varsayılan)
- `smooth`: Yumuşak geçişli kaydırır

**Nerede Kullanılır?**  
- Sayfa içi bağlantılarda (`<a href="#bölüm">`)
- `scrollIntoView()` gibi JS kaydırmalarda

---

## scroll-margin

**scroll-margin**, bir öğeye kaydırıldığında kenarda boşluk bırakmak için kullanılır.

```css
h2 {
  scroll-margin-top: 70px;
}
```

- Genelde sabit başlık (fixed header) olduğunda içerik başlığa yapışmasın diye kullanılır.
- `scroll-margin-top`, `scroll-margin-bottom` gibi yönlere özel ayarlanabilir.

**Nerede Kullanılır?**  
- Anchor linkle gidilen bölüm üstte biraz boşlukla görüntülensin diye.

---

## Örnek

```css
html {
  scroll-behavior: smooth;
}

section {
  scroll-margin-top: 80px;
}
```

- Sayfa içi bağlantı yumuşak kaydırılır.
- Hedef bölüm üstte 80px boşlukla yerleşir.
