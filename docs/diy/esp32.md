# DIY - ESP32 Kurulumu

ESP32, fiyat-performans açısından DIY Meshtastic düğümleri için en popüler platformdur. Wi-Fi ve Bluetooth desteği sayesinde yapılandırması ve güncellenmesi kolaydır.

!!! tip "Neden ESP32?"
    Düşük maliyeti, geniş topluluk desteği ve USB ile kolay programlanması onu ilk projeler için ideal kılar. Sabit röleler ve ev düğümleri için mükemmel bir seçimdir.

## İhtiyacınız Olanlar

- ESP32 tabanlı bir LoRa geliştirme kartı (ör. Heltec V3, LILYGO T-Beam)
- 868 MHz için uygun bir LoRa anteni
- USB veri kablosu
- Bilgisayar

Detaylı parça önerileri için [Parça Listesi](parca-listesi.md) sayfasına bakın.

## 1. Firmware'ü İndirin

[Meshtastic Firmware](https://meshtastic.org/docs/software/flashing/) sayfasından kartınıza uygun en son kararlı sürümü indirin.

!!! note "Not"
    Kartınızı seçerken doğru hedef platformu seçtiğinizden emin olun (ör. `heltec-v3`, `tlora-v2` gibi). Yanlış firmware cihazı çalıştırmayabilir.

## 2. Firmware'ü Yükleyin

Meshtastic'in web tabanlı flaşlama aracını kullanarak USB üzerinden firmware yükleyebilirsiniz:

1. Cihazı USB ile bilgisayara bağlayın.
2. Web tarayıcısından **Web Flasher** aracını açın.
3. Cihazınızın hedef platformunu seçin.
4. Firmware dosyasını sürükleyip bırakın ve **Flash** butonuna basın.

Alternatif olarak [esptool](https://github.com/espressif/esptool) ile komut satırından yükleyebilirsiniz:

```bash
pip install esptool
esptool.py --chip esp32 --port /dev/ttyUSB0 erase_flash
esptool.py --chip esp32 --port /dev/ttyUSB0 write_flash 0x0 firmware.bin
```

!!! warning "Sürücü sorunları"
    Bazı ESP32 kartları için CP210x veya CH340 USB sürücülerinin kurulu olması gerekir. Cihaz bilgisayarda görünmüyorsa önce sürücüleri kurun.

## 3. Anteni Bağlayın

- Anteni karttaki **IPEX (U.FL)** konnektörüne takın.
- Daha iyi menzil için harici bir anten tercih edin.

!!! danger "Dikkat"
    LoRa anteni bağlı olmadan cihazı asla açmayın. Antensiz çalışma, radyo modülüne (SX1262/SX1276) kalıcı zarar verebilir.

## 4. Yapılandırma

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

## 5. Güç ve Kurulum

- Sabit kullanım için kartınızı uygun bir kutu içine alın ve koruyun.
- Pil ile çalıştıracaksanız uygun bir LiPo/Li-ion pil kullanın.

!!! tip "İpucu"
    Ev düğümünüzü yüksek ve engelsiz bir konuma yerleştirmek menzili önemli ölçüde artırır.

## Sonraki Adımlar

- [nRF52840 Kurulumu](nrf52840.md) ile düşük güçlü alternatifi inceleyin.
- [Parça Listesi](parca-listesi.md) sayfasından parça önerilerine bakın.
