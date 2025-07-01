# Icon Font Kullanımı

**Icon Font**, ikonları bir yazı tipi (font) gibi yükleyip harf gibi kullanmanı sağlar. Böylece ikonlar metin gibi davranır, kolay ölçeklenir ve CSS ile şekillendirilebilir.

---

## Ne İşe Yarar?

- İkonları PNG veya SVG yerine font dosyası olarak yükler.
- Vektörel olduğu için kalite kaybı olmadan büyür veya küçülür.
- Renk, boyut, hover efekti gibi stiller kolayca verilir.
- Tek dosyada yüzlerce ikon barındırabilir.

---

## Yaygın Örnekler

- **Font Awesome**
- **Material Icons**
- **Ionicons**

---

## Nasıl Kullanılır?

### 1️⃣ HTML’ye Bağla

Örneğin Font Awesome CDN:

```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
```

---

### 2️⃣ HTML’de Kullan

```html
<i class="fa-solid fa-heart"></i>
```

---

### 3️⃣ CSS ile Stil Ver

```css
i {
  font-size: 32px;
  color: crimson;
}
```

---

## Avantajları

✅ Hafif ve hızlıdır.  
✅ Vektörel olduğu için çözünürlük kaybı olmaz.  
✅ Tek dosyada yüzlerce ikon taşır.  
✅ Renk, boyut gibi stil değişiklikleri kolaydır.

---

## Alternatif

- Yeni projelerde **SVG ikonlar** daha modern bir alternatiftir.
- Icon fontlar eski tarayıcı uyumu için hala kullanılır.

---

## Not

Icon fontlar `::before` ve `::after` pseudo-elementleriyle de kullanılabilir.

---


# Flaticon Nedir?

**Flaticon**, milyonlarca vektörel **ikon** sunan, tasarımcılar ve geliştiriciler için popüler bir ikon kütüphanesidir. İkonları PNG, SVG ve **ikon font** formatında sunar.

---

## Ne İşe Yarar?

- Web projelerine hızlıca ikon eklemek için kullanılır.
- İkonları PNG, SVG veya ikon fontu olarak indirebilirsin.
- Kendi özel ikon font setini oluşturup kullanabilirsin.
- Kişisel ve ticari projelerde kullanılabilir (lisansa dikkat!).

---

## Özellikleri

✅ Milyonlarca ikon içerir.  
✅ PNG, SVG, EPS, PSD, ikon font formatlarını destekler.  
✅ Renk ve boyut düzenlenebilir.  
✅ Kendi ikon fontunu oluşturup indirebilirsin.

---

## Nasıl Kullanılır?

### PNG veya SVG Olarak

1️⃣ [flaticon.com](https://www.flaticon.com) adresine git.  
2️⃣ İkonu seç ve PNG/SVG olarak indir.  
3️⃣ HTML’ye ekle:

```html
<img src="icon.svg" alt="Icon">
```

---

### Icon Font Olarak

1️⃣ Seçili ikonları koleksiyona ekle.  
2️⃣ "Generate Icon Font" özelliğiyle kendi ikon font paketini oluştur.  
3️⃣ `@font-face` ile projene entegre et.

Örnek:

```html
<i class="flaticon-search"></i>
```

```css
.flaticon-search {
  font-family: 'Flaticon';
}
```

---

## Avantajları

✅ Kolay ve hızlıdır.  
✅ Geniş ikon arşivi vardır.  
✅ İkonlar vektörel olduğu için kalite kaybı olmaz.  
✅ PNG, SVG veya font olarak esnek kullanım sunar.

---

## Not

Ücretsiz kullanımda genelde **attribution (kaynak belirtme)** zorunludur. Premium hesapla bu zorunluluk kalkar.
---

# The Noun Project Nedir?

**The Noun Project**, milyonlarca vektörel ikon ve sembol barındıran bir **ikon kütüphanesi**dir. Grafik tasarım, sunum, web projeleri gibi alanlarda yaygınca kullanılır.

---

## Ne İşe Yarar?

- Farklı kategorilerde yüz binlerce ikon sunar.
- İkonları SVG veya PNG formatında indirebilirsin.
- Sunum, mobil uygulama veya web arayüzlerinde kullanmak için uygundur.
- İkonlar kişisel ve ticari projelerde kullanılabilir (lisans kurallarına dikkat!).

---

## Özellikleri

✅ Geniş ve çeşitli ikon koleksiyonu.  
✅ Vektörel olduğu için kalite kaybı olmaz.  
✅ PNG ve SVG formatında indirilebilir.  
✅ Renk ve boyutları özelleştirilebilir.

---

## Nasıl Kullanılır?

1️⃣ [thenounproject.com](https://thenounproject.com) adresine git.

2️⃣ Anahtar kelimeyle ikon ara (ör. "search", "home", "mail" vb.).

3️⃣ Beğendiğin ikonu seç, boyutunu ve formatını belirle.

4️⃣ İndir ve projene ekle:

**Örneğin SVG kullanımı:**

```html
<img src="icon.svg" alt="Icon">
```

---

## Avantajları

✅ Kolay bulunur, arşivi zengindir.  
✅ Kullanımı basittir.  
✅ Yüksek çözünürlüklü, vektörel dosyalar sunar.  
✅ Web tasarım, sunum, infografik gibi pek çok alana uygundur.

---

## Lisans Durumu

- Ücretsiz kullanımda genelde **attribution (kaynak belirtme)** gerekir.
- Premium üyelikle kaynak belirtmeye gerek kalmaz.
- Ticari kullanımda telif kurallarını kontrol etmek önemlidir.

---

## Not

The Noun Project, özellikle geniş ikon yelpazesi ve tasarım stili çeşitliliği sayesinde UI/UX tasarımcıları için sık kullanılan bir kaynaktır.

---# Fontello Nedir?

**Fontello**, kendi özel **ikon fontlarını** kolayca oluşturmanı sağlayan bir **online icon font jeneratörüdür**. Font Awesome, Entypo, Typicons gibi popüler ikon setlerinden istediğin ikonları seçip tek bir dosyada birleştirirsin.

---

## Ne İşe Yarar?

- Yüzlerce ikon içinden sadece ihtiyacın olanları seçip kendi ikon font dosyanı oluşturursun.
- Tek font dosyası sayesinde web sitenin yükleme süresi hızlanır.
- İkonlar vektörel olduğu için kalite kaybı olmadan ölçeklenir.
- CSS sınıf isimlerini düzenleyerek kendi isimlendirme standardına uydurabilirsin.

---

## Özellikleri

✅ Popüler ikon setlerini destekler (Font Awesome, Entypo vb.).  
✅ Sadece seçilen ikonları içeren hafif font dosyası oluşturur.  
✅ Otomatik `@font-face` CSS dosyasını üretir.  
✅ SVG, PNG sprite ve ikon font desteği sunar.

---

## Nasıl Kullanılır?

1️⃣ [fontello.com](https://fontello.com) adresine git.

2️⃣ İstediğin ikonları seç.

3️⃣ İkon sınıf isimlerini düzenle (isteğe bağlı).

4️⃣ "Download Webfont" butonuna tıkla.

5️⃣ İndirilen zip dosyasında `font` dosyaları (`.woff`, `.ttf`, `.eot`), CSS dosyası ve örnek HTML bulunur.

---

## HTML’de Kullanım

```html
<link rel="stylesheet" href="css/fontello.css">

<i class="icon-home"></i>
```

---

## CSS ile Stil Ver

```css
.icon-home {
  font-size: 32px;
  color: #333;
}
```

---

## Avantajları

✅ Hafif dosya boyutu.  
✅ Sadece gereken ikonlar yüklenir.  
✅ Kolayca kişiselleştirilebilir.  
✅ Açık kaynaklı ve ücretsizdir.

---

## Not

Fontello, **proje bazlı özelleştirilmiş ikon fontları** hazırlamak için pratik bir alternatiftir. Daha hafif, optimize edilmiş web siteleri için idealdir.
``
