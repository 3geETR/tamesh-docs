# Hazır Cihazlar

Lehimleme, elektronik veya yazılım yükleme ile uğraşmak istemiyorsanız hazır bir Meshtastic cihazı satın alabilirsiniz. Bu cihazlar kurulu firmware ile birlikte gelir ve yalnızca Meshtastic mobil uygulaması ile eşleştirilmeleri yeterlidir.

## Nasıl Çalışır?

Hazır cihazlar şu şekilde kullanılır:

1. Cihazınızı şarj edin ve açın.
2. Telefonunuza Meshtastic uygulamasını kurun.
3. Cihazı Bluetooth ile telefonunuza bağlayın.
4. Ağa otomatik olarak katılın ve mesajlaşmaya başlayın.

!!! note "Not"
    Hazır cihazlar dağıtımdan önce genellikle bir uzak düğüme eşleştirilir. Kutu açılışında 2.1.0 ve üzeri bir firmware sürümü yüklü olması durumunda cihaz otomatik olarak güvenli şekilde ağa katılır ve ek bir yapılandırma gerekmez.

## Cihaz Seçerken Dikkat Edilecekler

- **Kapsama ihtiyacınız:** Ağaçlık ve engebeli arazide menzil düşebilir; daha yüksek anten kalitesine sahip modelleri tercih edin.
- **Pil ömrü:** Taşınabilir bir cihaz arıyorsanız büyük pili ve düşük güç tüketimi olan modelleri seçin.
- **Form faktörü:** Sabit bir röle için ev tipi modeller, gezinti için elde taşınabilir modeller uygundur.
- **Bant:** Türkiye'de kullanılan frekans bantları için [Frekans Seçimi](frekans-secimi.md) sayfasına bakın.

## Önerilen Hazır Cihazlar

| Cihaz | Öne Çıkan Özellikler | Uygun Senaryo |
|-------|----------------------|---------------|
| SenseCap T1000-E | Küçük, taşınabilir, GPS dahil | Taşınabilir el cihazı |
| LILYGO T-Echo | E-ink ekran, nRF52840, uzun pil ömrü | Taşınabilir / düşük güç |
| LILYGO T-Beam | GPS dahil ESP32, geniş topluluk desteği | Sabit / taşınabilir |
| LILYGO T-Deck | Klavye + ekran, esp32-s3 | Mesajlaşma odaklı kullanım |
| Heltec V3 | Wi-Fi + LoRa, düşük fiyat | Sabit röle / genel kullanım |
| RAK WisBlock | Modüler, profesyonel kalite | Kalıcı kurulumlar |

## Yazılım Yükleme

Meshtastic yazılımının yüklenmesi tüm cihazlarda aynı adımlarla yapılır. [Yazılım Yükleme/Güncelleme](../kurulum/yazilim.md) rehberini takip ederek cihazınıza firmware'i yükleyin.

!!! note "Not"
    Kartınızı seçerken doğru hedef platformu seçtiğinizden emin olun (ör. `heltec-v3`, `tlora-v2` gibi). Yanlış firmware cihazı çalıştırmayabilir.

!!! warning "Bağlantı sorunları"
    === "ESP32"
        Bazı ESP32 kartları için CP210x veya CH340 USB sürücülerinin kurulu olması gerekir. Cihaz bilgisayarda görünmüyorsa önce sürücüleri kurun; ayrıca [Sorun Giderme](../kurulum/yazilim.md#sorun-giderme) bölümüne bakabilirsiniz.
    === "nRF52840"
        nRF52840 cihazlarda cihazı programlama moduna almak için reset düğmesine 2 kez basmanız gerekebilir. Kartınız UF2 desteklemiyorsa nRF Connect Programmer ile yükleyebilirsiniz.

## Sonraki Adımlar

- [Başlangıç](index.md) sayfasına dönerek DIY yolunu da inceleyin.
- [Parça Listesi](diy/parca-listesi.md) ile aksesuar ve yedek parça önerilerine göz atın.
