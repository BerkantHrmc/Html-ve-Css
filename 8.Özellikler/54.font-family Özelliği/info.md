# font-family Özelliği

`font-family`, bir öğedeki metnin hangi yazı tipinde (font) görüntüleneceğini belirler.

---

## Temel Kullanım

```css
p {
  font-family: Arial, sans-serif; 
}
```

Tarayıcı önce `Arial` fontunu dener, yoksa `sans-serif` genel ailesini kullanır.

---

## Birden Fazla Font Belirtme

- Birincil font bulunamazsa, sıradaki alternatif kullanılır.
- Boşluk içeren font isimleri tırnak içine alınmalıdır.

```css
body {
  font-family: "Times New Roman", Georgia, serif; /*html dosyasındaki tüm fontları etkiler*/
}
```

---

## Genel Font Aileleri

- `serif` → Uçları çıkıntılı klasik fontlar (örnek: Times)
- `sans-serif` → Uçları düz, modern fontlar (örnek: Arial)
- `monospace` → Her karakterin genişliği eşit (örnek: Courier)
- `cursive` → El yazısı benzeri fontlar
- `fantasy` → Dekoratif fontlar

---

## Not

- Sistem fontları kullanıcı cihazına bağlıdır.
- Web fontları için `@font-face` veya Google Fonts kullanılabilir.
