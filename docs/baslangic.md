# Başlangıç

Meshtastic'e başlamak için öncelikle bir cihaz edinmeniz gerekir. Cihaz edinmek için ihtiyacınıza ve teknik bilginize göre size uygun olan yöntemi seçebilirsiniz.

## 1. Hazır Cihazlar

Eğer lehimleme, elektronik gibi işlemlerle uğraşmak istemiyorsanız hazır bir Meshtastic cihazı satın alabilirsiniz. Bu cihazlar kutudan çıktığı gibi kullanılabilir ve yalnızca Meshtastic uygulaması ile eşleştirilmeleri yeterlidir.

👉 **Devam etmek için:** [Hazır Cihazlar](hazir-cihazlar.md) sayfasına göz atın.

---

## 2. DIY (Kendin Yap)

Kendi Meshtastic düğümünüzü oluşturmak istiyorsanız DIY seçeneğini tercih edebilirsiniz. Eğer az da olsa elektronik bilginiz varsa ve lehim yapabiliyorsanız DIY olarak cihaz yapabilirsiniz.

DIY için en yaygın iki farklı kart kullanılmaktadır:

| ESP32 | nRF52840 |
|-------|----------|
| Güç tüketimi nRF52840'a göre oldukça yüksektir. | Çok daha düşük güç tüketimine sahiptir. |
| Wi-Fi ve Bluetooth içerir. | Bluetooth içerir, Wi-Fi bulunmaz. |
| Güç konusunda sorun yaşamayacağınız sabit istasyonlar ve genel kullanım için idealdir. | Uzun pil ömrü gerektiren cihazlar, solar ile çalışan düğümler için idealdir. |

### Hangisini Seçmeliyim?

- **İlk kez Meshtastic kullanacaksanız:** Hem nRF52840 hem de ESP32 kullanabilirsiniz.
- **Uzun pil ömrü önceliğinizse:** nRF52840 daha iyi bir seçim olacaktır.
- **Sabit bir röle (Router) veya ev düğümü kuracaksanız:** nRF52840 güç tüketimi dolayısıyla daha uygundur.

## Frekans Seçimi

Meshtastic cihazları LoRa radyo teknolojisini kullanır ve bölgeye göre belirlenen lisanssız frekans bantlarında çalışır. Cihazınızı ilk kez kurarken doğru bölgeyi seçmeniz gerekir; aksi takdirde diğer düğümlerle haberleşemezsiniz.

Türkiye'de kullanılan bant **868 MHz (EU868)** bölgesidir. Bu ayar, Meshtastic mobil uygulamasından **Bölge (Region)** olarak yapılır ve genellikle kurulum sırasında bir kez seçilir.

### Yaygın Bölgeler

| Bölge | Frekans | Kullanıldığı yerler |
|-------|---------|---------------------|
| Eu868 | 868 MHz | Türkiye ve Avrupa |
| Eu433 | 433 MHz | Avrupa'nın bazı bölgeleri |
| US | 915 MHz | ABD ve Amerika kıtası |

!!! warning "Dikkat"
    Ülkenize göre yasal olmayan bir bant seçmek hem cihazınızın diğer düğümlerle haberleşmesini engeller hem de yasal sorunlara yol açabilir. Türkiye'de **Eu868** bölgesini kullanın.

!!! tip "İpucu"
    Donanım alırken ürünün **868 MHz (EU)** bandında çalıştığından emin olun. Yanlış bantta çalışan bir cihaz, başka bölgedeki düğümlerle haberleşemez.

## Sonraki Adımlar

Seçiminize göre aşağıdaki rehberlerden devam edebilirsiniz:

- 📦 [Hazır Cihazlar](hazir-cihazlar.md)
- 🔧 [DIY - ESP32 Kurulumu](diy/esp32.md)
- 🔋 [DIY - nRF52840 Kurulumu](diy/nrf52840.md)
- 🛒 [DIY Parça Listesi](diy/parca-listesi.md)
