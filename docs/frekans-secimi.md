# Frekans Seçimi

Meshtastic cihazları LoRa radyo teknolojisini kullanır ve bölgeye göre belirlenen lisanssız frekans bantlarında çalışır. Cihazınızı ilk kez kurarken doğru bölgeyi seçmeniz gerekir; aksi takdirde diğer düğümlerle haberleşemezsiniz.

Türkiye'de yasal olarak kullanılan bantlar **868 MHz (EU868)** ve **433 MHz (EU433)** bölgeleridir.

## Türkiye'de Kullanılan Frekanslar

| Frekans | Güç Limiti | Kullanım |
|---|---|---|
| 433 MHz | 10 dBm (0.01 W) | Türkiye'de Meshtastic'e 433 MHz ile başlanmış olup 433 MHz cihaz sayısı daha fazladır. |
| 868 MHz | 27 dBm (0.5 W) | 868 MHz cihazların sayısı şimdilik daha azken yavaş yavaş artıyor. |

!!! tip "İpucu"
    Bölge ayarı, cihaz kurulumu sırasında Meshtastic uygulamasından bir kez yapılır. Kurulum rehberlerinde bu adımı bulabilirsiniz.

## Sonraki Adımlar

- [DIY - ESP32 Kurulumu](diy/esp32.md) ve [DIY - nRF52840 Kurulumu](diy/nrf52840.md) sayfalarında bölge ayarının nasıl yapıldığını bulabilirsiniz.
- Cihaz edinme seçenekleri için [Başlangıç](baslangic.md) sayfasına dönebilirsiniz.
