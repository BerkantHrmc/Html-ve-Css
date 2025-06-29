# CSS `background-size` Özelliği

## Açıklama
`background-size` özelliği, bir öğenin arka plan resminin boyutlarını ayarlamak için kullanılır.

## Değerler
- **`auto`**  
  Varsayılan değerdir. Arka plan resmi orijinal boyutunda görüntülenir.
- **`cover`**  
  Arka plan resmi öğenin tamamını kaplayacak şekilde ölçeklenir. Oran korunur.
- **`contain`**  
  Arka plan resmi öğeye tamamen sığacak şekilde ölçeklenir. Oran korunur.
- **`<uzunluk>` veya `<yüzde>`**  
  Genişlik ve yükseklik belirterek özel boyut verilebilir. Örneğin `background-size: 100px 50px;`

## CSS Kodu Örneği

```css
div {
  width: 300px;
  height: 200px;
  border: 5px solid black;
  background-image: url('https://via.placeholder.com/400');
  background-repeat: no-repeat;
  background-size: cover; /* contain veya özel boyut verilebilir */
}
