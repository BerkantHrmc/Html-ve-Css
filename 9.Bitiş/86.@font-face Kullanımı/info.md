# @font-face Kullanımı

`@font-face`, bir web sitesine **özel bir yazı tipi (font)** eklemek için kullanılır. Böylece ziyaretçinin cihazında font yüklü olmasa bile tarayıcı fontu sunucudan indirir ve uygular.

---

## Neden Kullanılır?

- Özel veya marka fontları siteye eklemek.
- Tüm cihazlarda aynı görünümü sağlamak.
- Yerel font bağımlılığını ortadan kaldırmak.

---

## Temel Kullanım

```css
@font-face {
  font-family: 'MyFont';
  src: url('fonts/MyFont.woff2') format('woff2'),
       url('fonts/MyFont.woff') format('woff');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}
```

---

## Açıklama

- **font-family:** Tarayıcıda kullanılacak takma isim.
- **src:** Font dosyalarının yolu ve formatı.
  - Formatlar: `woff2` (modern), `woff` (yaygın), `ttf` (eski).
- **font-weight:** Kalınlık (`normal`, `bold` vb.).
- **font-style:** Stil (`normal`, `italic` vb.).
- **font-display:** Font yüklenene kadar nasıl davranılacağını belirler.
  - `swap`: Tarayıcı önce yedek fontu kullanır, font gelince yeni fontu uygular. En yaygın ve performans dostu seçenektir.
  - Diğer değerler: `auto`, `block`, `fallback`, `optional`.

---

## Kullanım Örneği

```css
body {
  font-family: 'MyFont', Arial, sans-serif;
}
```

---

## Not

- `woff2` modern tarayıcılar için önerilir.
- Eski tarayıcılar için `woff` veya `ttf` eklenebilir.
- `font-display: swap` kullanmak, **FOIT (Flash of Invisible Text)** sorununu azaltır ve sayfa hızını iyileştirir.
---
# Transfonter Nedir?

**Transfonter**, web için font dosyalarını kolayca dönüştürmek, optimize etmek ve kullanıma hazır hale getirmek için kullanılan popüler bir **online font dönüştürücü** ve **@font-face jeneratörüdür**.

---

## Ne İşe Yarar?

- `.ttf`, `.otf` gibi font formatlarını modern web için uygun `woff` ve `woff2` formatlarına dönüştürür.
- Web projeleri için gerekli `@font-face` CSS kodunu otomatik hazırlar.
- Font dosyalarını **gzip sıkıştırma** ile optimize eder.
- İstemediğiniz karakterleri (ör. gereksiz dil desteği) çıkarmanıza imkan tanır, böylece dosya boyutunu küçültür.
- Web fontlarını self-host (kendi sunucunda barındır) mantığına uygun şekilde hazırlar.

---

## Nasıl Kullanılır?

1️⃣ Transfonter web sitesine gir: [transfonter.org](https://transfonter.org)

2️⃣ Kendi `.ttf` veya `.otf` font dosyalarını yükle.

3️⃣ Gerekirse alt ayarları yap:
   - Karakter seti seç (Latin, Kiril vs.)
   - Sıkıştırma ve format ayarlarını kontrol et.

4️⃣ **Convert** butonuna tıkla.

5️⃣ İndirilen dosya içinde dönüştürülmüş `woff/woff2` fontları ve hazır `@font-face` CSS kodu bulunur.

---

## Avantajları

✅ Ücretsiz ve hızlıdır.  
✅ Teknik bilgi gerektirmez.  
✅ Birden fazla fontu aynı anda dönüştürebilir.  
✅ Hazır CSS ile entegrasyonu kolaydır.

---

## Örnek Çıktı

İndirilen zip dosyasında:
- `MyFont.woff`  
- `MyFont.woff2`  
- `styles.css` (otomatik oluşturulmuş `@font-face` tanımı)

---

## Not

Transfonter ile dönüştürdüğün fontları kendi sunucunda barındırmak, harici font servisi (Google Fonts gibi) kullanmaya göre hız ve gizlilik avantajı sağlar.

---

# Google Fonts Nedir?

**Google Fonts**, web projelerinde ücretsiz, hızlı ve kolay şekilde kullanılabilen açık kaynaklı fontları sağlayan bir **web font kütüphanesidir**.

---

## Ne İşe Yarar?

- Binlerce ücretsiz font sunar.
- Tarayıcı uyumlu, modern `woff` formatlarıyla gelir.
- CDN (Content Delivery Network) üzerinden hızlı yüklenir.
- Kolayca HTML veya CSS içine eklenir.
- Web tasarımda tipografi uyumunu sağlar.

---

## Nasıl Kullanılır?

1️⃣ [fonts.google.com](https://fonts.google.com) adresine git.

2️⃣ İstediğin fontu seç.  
Örneğin: **Roboto**

3️⃣ Stilleri seç (normal, bold, italic vs.)

4️⃣ Google sana bir `<link>` etiketi veya `@import` kodu verir:

```html
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

veya

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
```

---

## HTML'de Kullanım

```html
<head>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>

<body>
  <p style="font-family: 'Roboto', sans-serif;">Merhaba Google Fonts!</p>
</body>
```

---

## CSS'de Kullanım

```css
body {
  font-family: 'Roboto', sans-serif;
}
```

---

## Avantajları

✅ Ücretsiz ve lisanslıdır.  
✅ Yüzlerce dil desteği vardır.  
✅ CDN üzerinden hızlı yüklenir.  
✅ `display=swap` parametresiyle FOIT (Flash of Invisible Text) engellenir.

---

## Not

- Performans için sadece gerekli font ağırlıklarını seç.
- Çok fazla font yüklemek sayfa hızını yavaşlatabilir.
