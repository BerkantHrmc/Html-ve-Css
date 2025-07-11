# CSS `position` Özellikleri Tablosu

| **Position Değeri** | **Açıklama** | **Davranışı** |
|----------------------|----------------|----------------|
| `static` | Varsayılan konumlandırma | Eleman normal akıştadır, `top`, `left` gibi konum özellikleri işlemez. |
| `relative` | Göreceli konumlandırma | Eleman normal yerindedir, `top`, `left` ile kendi yerinden kaydırılır. Diğer elemanlar eski yerine göre yerleşir. |
| `absolute` | Mutlak konumlandırma | Eleman en yakın `relative` veya `absolute` kapsayıcıya göre konumlanır. Normal akıştan çıkar. |
| `fixed` | Sabit konumlandırma | Eleman ekrana göre konumlanır, sayfa kaydırıldığında sabit kalır. |
| `sticky` | Yapışkan konumlandırma | Eleman normal akışta başlar, kaydırıldığında belirli bir noktaya gelince sabitlenir. |

---

![CSS Position Property](./position_property_example.png)
