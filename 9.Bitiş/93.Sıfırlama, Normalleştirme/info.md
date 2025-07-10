# CSS Dersleri - Sıfırlama (Reset) ve Normalleştirme (Normalize)

---

## Neden Sıfırlama / Normalleştirme Kullanılır?

Tarayıcılar HTML etiketlerine kendi **varsayılan stillerini** uygular.  
Bu stiller her tarayıcıda farklılık gösterir.  
Bu yüzden bir sitede aynı HTML kodu, farklı tarayıcılarda farklı görünebilir.  
Tutarlı ve öngörülebilir bir tasarım için **sıfırlama** ya da **normalleştirme** kullanılır.

---

## Sıfırlama (CSS Reset)

**Sıfırlama**, tüm HTML etiketlerinin margin, padding gibi varsayılan stillerini **tamamen sıfırlar**.

**Amaç:**  
- Tarayıcı farklarını ortadan kaldırmak.
- Tüm etiketleri sıfırdan, kendi tasarımına göre yeniden şekillendirmek.

**Örnek Reset CSS:**

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

- Bu kod tüm öğelerde margin ve padding’i sıfırlar.
- `box-sizing: border-box` ile padding ve border, kutunun genişliğine dahil edilir.

Popüler reset örneği: **Eric Meyer Reset**

---

## Normalleştirme (Normalize.css)

**Normalleştirme**, sıfırlamak yerine tarayıcı farklarını **düzelten** bir yaklaşımdır.

**Amaç:**  
- Bazı varsayılan stilleri korur.
- Varsayılan stilleri daha öngörülebilir, uyumlu hale getirir.
- Form elemanları, başlıklar gibi etiketlerde ortak bir baz sağlar.

Popüler örnek: **normalize.css**

**normalize.css**, HTML5 etiketleri, form elemanları ve metin formatlama gibi detayları düzeltir.

---

## Fark

| Özellik | Sıfırlama (Reset) | Normalleştirme (Normalize) |
|--------------------|------------------------------|-----------------------------|
| Ne yapar? | Tüm stilleri sıfırlar | Tarayıcı farklarını düzeltir |
| Varsayılan stil? | Tamamen siler | Bazı varsayılanları korur |
| Kontrol | Tam kontrol sağlar | Tutarlı taban sağlar |

---

## Ne Zaman Kullanılır?

- **Reset:** Kendi stil
