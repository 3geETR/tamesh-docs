# Başlangıç

TAMesh ağına katılmanın iki farklı yolu vardır. İhtiyacınıza ve teknik bilginize göre size uygun olan yöntemi seçebilirsiniz.

## 1. Hazır Cihazlar (Önerilir)

Eğer lehimleme, elektronik veya yazılım yükleme gibi işlemlerle uğraşmak istemiyorsanız hazır bir Meshtastic cihazı satın alabilirsiniz. Bu cihazlar kutudan çıktığı gibi kullanılabilir ve yalnızca Meshtastic uygulaması ile eşleştirilmeleri yeterlidir.

👉 **Devam etmek için:** [Hazır Cihazlar](hazir-cihazlar.md) sayfasına göz atın.

---

## 2. DIY (Kendin Yap)

Kendi Meshtastic düğümünüzü oluşturmak istiyorsanız DIY seçeneğini tercih edebilirsiniz. Bu yöntem daha ekonomiktir ve donanım üzerinde tam kontrol sağlar.

DIY için en yaygın iki platform bulunmaktadır:

| | ESP32 | nRF52840 |
|---|-------|----------|
| 💰 Fiyat | Daha uygun fiyatlıdır. | Daha pahalıdır. |
| 🔋 Güç tüketimi | Daha yüksektir. | Daha düşüktür. |
| 📶 Kablosuz | Wi-Fi ve Bluetooth içerir. | Bluetooth içerir, Wi-Fi bulunmaz. |
| 🔌 Programlama | USB üzerinden kolayca programlanabilir. | USB üzerinden programlanabilir. |
| 🏠 Kullanım senaryosu | Sabit istasyonlar ve genel kullanım için idealdir. | Taşınabilir ve uzun pil ömrü gerektiren cihazlar için idealdir. |

### Hangisini Seçmeliyim?

- **İlk kez Meshtastic kullanacaksanız:** ESP32 ile başlamanız önerilir.
- **Uzun pil ömrü önceliğinizse:** nRF52840 daha iyi bir seçim olacaktır.
- **Sabit bir röle (Router) veya ev düğümü kuracaksanız:** ESP32 genellikle daha uygundur.
- **Taşınabilir el cihazı yapmak istiyorsanız:** nRF52840 tercih edilebilir.

!!! tip "İpucu"
    Hangi donanımı alacağınıza karar vermeden önce [Parça Listesi](diy/parca-listesi.md) sayfasına göz atın.

## Sonraki Adımlar

Seçiminize göre aşağıdaki rehberlerden devam edebilirsiniz:

- 📦 [Hazır Cihazlar](hazir-cihazlar.md)
- 🔧 [DIY - ESP32 Kurulumu](diy/esp32.md)
- 🔋 [DIY - nRF52840 Kurulumu](diy/nrf52840.md)
- 🛒 [DIY Parça Listesi](diy/parca-listesi.md)
