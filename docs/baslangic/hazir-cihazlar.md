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

## Türkiyede Bulabileceğiniz Hazır Cihazlar

- [DeepLab Studio MicroMesh 433MHz](https://amzn.eu/d/04tcD37c)

- [DeepLab Studio MiniMesh 433MHz](https://amzn.eu/d/0aZpSRX1)

- [LILYGO ESP32 Geliştirme Kartları](https://motorobit.com/lilygo)

- [TTGO ESP32 Geliştirme Kartı](https://www.direnc.net/esp-32-lora-gelistirme-board-wifi-kiti-096-inch-oled-ekranli)

## Yazılım Yükleme

Meshtastic yazılımının yüklenmesi tüm cihazlarda aynı adımlarla yapılır. [Yazılım Yükleme/Güncelleme](../kurulum/yazilim.md) rehberini takip ederek cihazınıza firmware'i yükleyin.

!!! note "Not"
    Kartınızı seçerken doğru hedef platformu seçtiğinizden emin olun (ör. `heltec-v3`, `tlora-v2` gibi). Yanlış firmware cihazı çalıştırmayabilir.

!!! warning "Bağlantı sorunları"
    === "ESP32"
        Bazı ESP32 kartları için CP210x veya CH340 USB sürücülerinin kurulu olması gerekir. Cihaz bilgisayarda görünmüyorsa önce sürücüleri kurun.
    === "nRF52840"
        nRF52840 cihazlarda cihazı programlama moduna almak için reset düğmesine 2 kez basmanız gerekebilir. Kartınız UF2 desteklemiyorsa nRF Connect Programmer ile yükleyebilirsiniz.

## Sonraki Adımlar

- [Başlangıç](index.md) sayfasına dönerek DIY yolunu da inceleyin.
- [İlk Ayarlar](../kurulum/ilk-ayarlar.md) sayfasına giderek ayarları yapın.