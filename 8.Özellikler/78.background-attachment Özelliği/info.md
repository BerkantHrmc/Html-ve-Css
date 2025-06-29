# CSS `background-attachment` Özelliği

## Açıklama
`background-attachment` özelliği, arka plan resminin kaydırma davranışını belirler. Yani sayfa kaydırıldığında arka planın hareket edip etmeyeceğini kontrol eder.

## Değerler
- **`scroll`**  
  Varsayılan değerdir. Arka plan, içerikle birlikte kayar.
- **`fixed`**  
  Arka plan, viewport’a sabitlenir. Sayfa kaydırılsa bile arka plan sabit kalır.
- **`local`**  
  Arka plan, içeriğin kaydırılmasıyla birlikte kayar (genelde scrollable öğelerde kullanılır).

## CSS Kodu Örneği

```css
div {
  width: 300px;
  height: 200px;
  overflow: scroll;
  border: 5px solid black;
  background-image: url('https://via.placeholder.com/400');
  background-repeat: no-repeat;
  background-attachment: fixed; /* scroll | local */
}
