# text-shadow Özelliği

`text-shadow`, metne **gölge efekti** eklemek için kullanılır.

---

## Sözdizimi

```css
text-shadow: x-offset y-offset blur-radius color;
```

- **x-offset** → Yatay gölge mesafesi  
- **y-offset** → Dikey gölge mesafesi  
- **blur-radius** → Bulanıklık yarıçapı (isteğe bağlı)  
- **color** → Gölge rengi

---

## Örnek Kullanım

```css
h1 {
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
}
```

Bu örnekte gölge 2px sağa, 2px aşağı kayar ve 5px bulanıklığa sahip olur.

---

## Çoklu Gölge

Virgül ile birden fazla gölge uygulanabilir.

```css
p {
  text-shadow: 1px 1px 2px black, -1px -1px 2px gray;
}
```

---

## Not

`text-shadow`, metni vurgulamak, derinlik efekti vermek veya okunabilirliği artırmak için kullanılır.
