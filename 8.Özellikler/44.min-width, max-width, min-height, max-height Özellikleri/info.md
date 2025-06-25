min-width, max-width, min-height, max-height Özellikleri
--------------------------------------------------------

CSS’de min-width, max-width, min-height, max-height özellikleri, bir HTML elemanının boyutlarını
belirli sınırlar içinde tutmak için kullanılır. Bu özellikler, responsive (duyarlı) tasarımlarda 
özellikle önemlidir.
Bu da inline satır içi elemanlarda işe yaramaz(şimdilik).

min-width – Minimum Genişlik
Bir elemanın alabileceği en küçük genişliği belirler.
max-width – Maksimum Genişlik
Bir elemanın alabileceği en büyük genişliği sınırlar.
min-height – Minimum Yükseklik
Bir elemanın alabileceği en küçük yüksekliği belirler.
max-height – Maksimum Yükseklik
Bir elemanın alabileceği en büyük yüksekliği sınırlar.


----------------------------------------------------------------------------------------------------

div{
  max-width: 1000px;  /*alabileceği max genişlik 1000px 1000den aza düşebilir ekran küçülünce*/
  min-width: 600px;   /*600px'in altına inerse artık scroll devreye girer*/
  background-color: lime;
  max-height: 400px;  /*alabileceği max uzunluk 400px 400den aza düşebilir ekran küçülünce*/
  min-height: 200px;   /*200px'in altına inerse artık scroll devreye girer*/
}



----------------------------------------------------------------------------------------------------



