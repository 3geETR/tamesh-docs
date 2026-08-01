# DIY - ESP32 Cihaz Yapımı

ESP32, fiyat-performans açısından DIY Meshtastic düğümleri için en popüler platformdur. Wi-Fi ve Bluetooth desteği sayesinde yapılandırması ve güncellenmesi kolaydır.

!!! tip "Neden ESP32?"
    Düşük maliyeti, geniş topluluk desteği ve USB ile kolay programlanması onu ilk projeler için ideal kılar. Sabit röleler ve ev düğümleri için mükemmel bir seçimdir.

## İhtiyacınız Olanlar

- ESP32 geliştirme kartı
- Meshtastic ile uyumlu bir LoRa modulü
- Lehim ekipmanları

Detaylı parça önerileri için [Parça Listesi](parca-listesi.md) sayfasına bakın.

## 1. Yazılım Yükleme

Meshtastic yazılımının yüklenmesi tüm cihazlarda aynı adımlarla yapılır. [Yazılım Yükleme/Güncelleme](../../kurulum/yazilim.md) rehberini takip ederek cihazınıza firmware'i yükleyin.

!!! note "Not"
    Kartınızı seçerken doğru hedef platformu seçtiğinizden emin olun (ör. `heltec-v3`, `tlora-v2` gibi). Yanlış firmware cihazı çalıştırmayabilir.

!!! warning "Bağlantı sorunları"
    Bazı ESP32 kartları için CP210x veya CH340 USB sürücülerinin kurulu olması gerekir. Cihaz bilgisayarda görünmüyorsa önce sürücüleri kurun; ayrıca [Sorun Giderme](../../kurulum/yazilim.md#sorun-giderme) bölümüne bakabilirsiniz.

## 2. Anteni Bağlayın

- Anteni karttaki **IPEX (U.FL)** konnektörüne takın.
- Daha iyi menzil için harici bir anten tercih edin.

!!! danger "Dikkat"
    LoRa anteni bağlı olmadan cihazı asla açmayın. Antensiz çalışma, radyo modülüne (SX1262/SX1276) kalıcı zarar verebilir.

## 3. Yapılandırma

1. Telefonunuza **Meshtastic** uygulamasını kurun.
2. Cihazın Bluetooth'unu açın ve telefona bağlayın.
3. Düğümünüze bir isim verin ve gerekirse konum, kanal ve şifreleme ayarlarını yapın.
4. Mesajlaşmaya başlayın!

### Önerilen İlk Ayarlar

| Ayar | Öneri |
|------|-------|
| Bölge | Türkiye için uygun bölgeyi seçin ([Frekans Seçimi](../frekans-secimi.md)) |
| Düğüm adı | Örn. `TAMesh-EvDugumu` |
| Kanal | Ağ ile uyumlu ortak kanalı kullanın |
| Konum | Yayınlama istiyorsanız açın |

## 4. Güç ve Kurulum

- Sabit kullanım için kartınızı uygun bir kutu içine alın ve koruyun.
- Pil ile çalıştıracaksanız uygun bir LiPo/Li-ion pil kullanın.

!!! tip "İpucu"
    Ev düğümünüzü yüksek ve engelsiz bir konuma yerleştirmek menzili önemli ölçüde artırır.

## Sonraki Adımlar

- [nRF52840 Kurulumu](nrf52840.md) ile düşük güçlü alternatifi inceleyin.
- [Parça Listesi](parca-listesi.md) sayfasından parça önerilerine bakın.
