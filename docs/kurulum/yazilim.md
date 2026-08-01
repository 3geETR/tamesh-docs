# Meshtastic Yazılım Yükleme/Güncelleme

## 1. Cihaz Bağlantısı

- Meshtastic cihazınızı USB kablosu ile bilgisayara bağlayın
- Cihazınızı programlama moduna getirin

!!! note "Not"
    Genellikle programlama moduna getirmeye ihtiyacınız olmayacaktır. Bağlantı olduğunuz cihaz flash işlemi sırasında otomatik olarak programlama moduna girecektir. Ancak yine de programlama moduna otomatik olarak girmezse TTGO cihazları için **Boot** butonuna, T-Beam için **User** butonuna basılı tutarak USB kablosunu bağlayın. WisBlock için flasher aracında **Enter DFU Mode** butonuna basarak çıktı isteyen cihazınızı seçin. nRF52840 cihazlar için ise reset düğmesine 2 kere basın.

## 2. Web Flasher'a Erişim

Meshtastic Web Flasher aracına erişmek için:

[Web Flasher'ı Aç](https://flash.meshtastic.org)

!!! info "Öneri"
    Chrome veya Edge tarayıcı kullanmanız önerilir.

## 3. Firmware'in Cihaza Yüklenmesi

- Flasher sayfasında **Select Target Device** butonuna basarak kullanmış olduğunuz cihazı seçin
- Cihazınızı arayın ve **USB Serial Port** olarak görünen cihazı seçin
- Tarayıcının istediği USB erişim izinlerini onaylayın
- Eğer ilk defa kurulum yapıyorsanız, **full erase and install** seçeneğini aktif edin

!!! note "Not"
    Bu ayar aktif değilse daha önce Meshtastic üzerinde yaptığınız ayarlar korunacaktır. İlk defa bir cihaz kuruyorsanız bu seçeneği aktif etmeniz önerilir.

- **Erase Flash and Install** butonuna tıklayarak yükleme işlemini başlatın
- Yükleme işlemi yaklaşık 2-3 dakika sürecektir
- **Success!** mesajını görene kadar bekleyin

!!! info "Dikkat"
    Yükleme sırasında cihazınızın bağlantısını kesmeyin ve tarayıcı penceresini kapatmayın.

## 4. Doğrulama ve İlk Kullanım

- Cihazınız otomatik olarak yeniden başlayacaktır
- Mavi LED'in düzenli aralıklarla yanıp söndüğünü kontrol edin
- Meshtastic mobil uygulamasını açın ve cihazınızı arayın
- Bluetooth üzerinden cihazınıza bağlanın ve temel ayarları yapılandırın

## Sorun Giderme

### Cihaz Algılanmıyor?
=== "ESP32"
    - Bazı ESP32 kartları için CP210x veya CH340 USB sürücülerinin kurulu olması gerekir. Cihaz bilgisayarda görünmüyorsa önce sürücüleri kurun; ayrıca [Sorun Giderme](#sorun-giderme) bölümüne bakabilirsiniz.
    - USB kablonuzun veri transferi desteklediğinden emin olun
    - Farklı bir USB bağlantı noktası deneyin
=== "nRF52840"
    - nRF52840 cihazlarda cihazı programlama moduna almak için reset düğmesine 2 kez basmanız gerekebilir. Kartınız UF2 desteklemiyorsa nRF Connect Programmer ile yükleyebilirsiniz.
    - USB kablonuzun veri transferi desteklediğinden emin olun
    - Farklı bir USB bağlantı noktası deneyin