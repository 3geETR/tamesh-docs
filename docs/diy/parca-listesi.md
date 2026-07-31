# DIY Parça Listesi

Kendi Meshtastic düğümünüzü oluşturmak için ihtiyaç duyabileceğiniz parçaları burada topladık. Liste, hem [ESP32](esp32.md) hem de [nRF52840](nrf52840.md) tabanlı kurulumlar için öneriler içerir.

!!! tip "Nereden Alınır?"
    Parçaları yerel elektronik mağazalarından veya online alışveriş sitelerinden (AliExpress, Amazon, resmi üretici mağazaları) temin edebilirsiniz. Resmi mağazaları tercih etmek sahte ürün riskini azaltır.

## ESP32 Tabanlı Kurulum

=== "Önerilenler"

    | Parça | Önerilen Model | Açıklama |
    |-------|----------------|----------|
    | Geliştirme kartı | LILYGO T-Beam | Entegre GPS ve 18650 pil yuvası |
    | Geliştirme kartı | Heltec V3 | Wi-Fi + LoRa, OLED ekran |
    | Geliştirme kartı | LILYGO T-Deck | Klavye ve ekranlı mesajlaşma cihazı |
    | Anten | 868 MHz SMA/IPEX anten | Uygun bantta çalışan bir anten şart |
    | Pil | 18650 Li-ion veya 3.7V LiPo | Kapasite ihtiyacına göre seçin |
    | Kutu | IP55/IP65 muhafaza | Sabit kurulumlar için su geçirmezlik önemli |
    | Bağlantı | USB Type-C veri kablosu | Firmware yükleme ve şarj için |

=== "Bütçe Alternatifi"

    | Parça | Önerilen Model | Açıklama |
    |-------|----------------|----------|
    | Geliştirme kartı | TTGO LoRa32 | Ekransız daha ucuz bir ESP32 seçeneği |
    | Anten | Ucuz 868 MHz coil anten | Giriş seviyesi yeterli olabilir |
    | Pil | 18650 pil | En ekonomik enerji çözümü |

## nRF52840 Tabanlı Kurulum

=== "Önerilenler"

    | Parça | Önerilen Model | Açıklama |
    |-------|----------------|----------|
    | Geliştirme kartı | LILYGO T-Echo | E-ink ekran, yüksek pil ömrü |
    | Geliştirme kartı | RAK WisBlock | Modüler ve profesyonel kalite |
    | Anten | 868 MHz SMA/IPEX anten | Uygun bantta çalışan bir anten şart |
    | Pil | 3.7V LiPo (1000mAh+) | Taşınabilir kullanım için kapasite önemli |
    | Kutu | Taşınabilir muhafaza | Taşınabilirlik ve koruma dengesi |

## Ortak Aksesuarlar

- **Şarj aleti:** Kartınıza uygun USB şarj cihazı.
- **Yedek anten:** Farklı menzil ihtiyaçları için ikinci bir anten.
- **GPS anteni:** Sabit kurulumlarda daha iyi konum için harici GPS anteni.

!!! warning "Uyarı"
    Anten ve radyo kartı satın alırken ürünün **868 MHz** (EU) bandında çalıştığından emin olun. Yanlış bantta çalışan donanım, hem yasal hem de teknik sorunlara yol açabilir.

## Sonraki Adımlar

- [ESP32 Kurulumu](esp32.md) ile kuruluma devam edin.
- [nRF52840 Kurulumu](nrf52840.md) ile düşük güçlü kuruluma geçin.
