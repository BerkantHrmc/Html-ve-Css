# CSS `background-origin` Özelliği

## Açıklama
`background-origin` özelliği, arka plan resimlerinin veya arka planın konumlandırılacağı kutuyu belirler. Bu özellik, arka planın hangi referans kutuya göre yerleştirileceğini kontrol eder.

## Kullanım
`background-origin` değeri, bir HTML öğesinin içeriği, padding veya border kutusuna göre ayarlanabilir.

## Değerler
- **`border-box`**  
  Arka plan resmi, kenarlık kutusuna (border box) göre konumlanır. Varsayılan değerdir.
  
- **`padding-box`**  
  Arka plan resmi, padding kutusuna göre konumlanır (kenarlık hariç).
  
- **`content-box`**  
  Arka plan resmi, sadece içerik kutusuna göre konumlanır (padding ve border hariç).

## Örnek

## CSS Kodu Örneği

```css
div {
  width: 200px;
  height: 200px;
  border: 10px solid black;
  padding: 20px;
  background-image: url('https://via.placeholder.com/150');
  background-repeat: no-repeat;
  background-origin: content-box; /* border-box veya padding-box olarak da ayarlanabilir */
}

