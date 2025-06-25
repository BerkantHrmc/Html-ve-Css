## `padding` Özelliği

CSS'de en çok kullandığımız özelliklerden biridir.  
Padding, bir HTML öğesinin içeriği ile kenarlığı (border) arasındaki iç boşluktur.

- 🟦 Yani içerik ile çerçeve arasında nefes alanı oluşturur.  
- 🟦 Yazı ile kutunun kenarı yapışmasın diye kullanılır.

---

### `padding` Alt Özellikleri

HTML'deki bir öğenin içeriği ile kenarlıkları (border) arasındaki iç boşlukları ayrı ayrı tanımlamak için aşağıdaki alt özellikler kullanılır:

- **`padding-top`**  
  ➤ Öğenin **üst kısmındaki** iç boşluğu belirler.

- **`padding-right`**  
  ➤ Öğenin **sağ kısmındaki** iç boşluğu belirler.

- **`padding-bottom`**  
  ➤ Öğenin **alt kısmındaki** iç boşluğu belirler.

- **`padding-left`**  
  ➤ Öğenin **sol kısmındaki** iç boşluğu belirler.

---

### Örnek CSS Kullanımı

```css
div {
  padding: 10px;            /* Etrafına 10px boşluk bırakır */
  background-color: lime;   /* Arka plan rengi lime */
  width: max-content;       /* İçeriğe göre genişlik alır */
}

div{
    padding: 100px 50px;    /*ilk değer yukarı-aşşağı , ikinci değer sağa sola etki eder.*/
}

div{
    padding: 100px 50px 60px;    /*ilk değer yukarı  , ikinci değer sağa sola , üçüncü aşşağıdan etki eder.*/
}
```

`yukarı sağ sol aşşağı şeklinde devam eder.`

---

Satır içi (inline) elemanlar, genişlik ve yükseklik değerlerini tam olarak kabul etmediği gibi, padding de sadece yatayda (left, right) etkili olur; dikey (top, bottom) padding genellikle öğenin yüksekliğini değiştirmez.

🔹 Neden?
Çünkü satır içi elemanlar, yazı akışı içinde yer alır ve satır yüksekliğiyle sınırlıdır. Bu yüzden yukarı-aşağı boşluk verse bile görünürde etkisi olmaz ya da sınırlı olur.

🔸 Çözüm: display: inline-block; yaparak tüm padding’i etkili kullanabilirsin.(ileride)