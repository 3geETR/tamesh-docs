# İlk Ayarlar

Meshtastic yazılımını cihazınıza yüklediyseniz, iletişime geçmeden önce birkaç ayar yapmanız gerekir. Bu rehberde cihazınızı TAMesh ağına bağlamak için gereken adımları bulabilirsiniz.

## Meshtastic Uygulaması

Cihazınızı yapılandırmak için akıllı telefonunuza **Meshtastic** uygulamasını kurun:

- [App Store](https://apps.apple.com/us/app/meshtastic/id1586432531)
- [Google Play](https://play.google.com/store/apps/details?id=com.geeksville.mesh)

Uygulamayı açın ve cihazınızı Bluetooth üzerinden bağlayın.

## TAMesh Kanalı

TAMesh topluluğu varsayılan **LongFast** kanalını değil, **kendi kanalını** kullanır. Ağa katılabilmek için cihazınızın TAMesh kanalına bağlanması gerekir.

!!! info "Kanal nedir?"
    Kanal, Meshtastic ağında iletişimin gerçekleştiği sanal bir ağdır. Aynı kanal ayarlarını kullanan cihazlar birbirini görür. TAMesh kanalına geçmek için aşağıdaki bağlantıları kullanmanız yeterlidir.

### Kanal Bağlantısı

Cihazınızın frekansına göre aşağıdaki bağlantılardan birini telefonunuzda açın:

=== "EU_433 Kanalı"
    433 MHz bandını kullananlar için:

    [https://meshtastic.org/e/#ChEaB1RBX01lc2goATABOgIIIBIYCAEQBDgCQANIAVAKWAFoAXUAkNhDyAYB](https://meshtastic.org/e/#ChEaB1RBX01lc2goATABOgIIIBIYCAEQBDgCQANIAVAKWAFoAXUAkNhDyAYB)

=== "EU_868 Kanalı"
    868 MHz bandını kullananlar için:

    [https://meshtastic.org/e/#ChEaB1RBX01lc2goATABOgIIIBIRCAEQBDgDQANIAVAKaAHIBgE](https://meshtastic.org/e/#ChEaB1RBX01lc2goATABOgIIIBIRCAEQBDgDQANIAVAKaAHIBgE)

!!! tip "İpucu"
    Bağlantıyı telefonunuzda açtığınızda Meshtastic uygulaması kanalı otomatik algılar ve cihazınıza yüklemeyi önerir. Onaylamanız yeterlidir. Fakat bazen ayarları tam uygulamayabilir; aşağıdaki tabloya göre doğrulayabilirsiniz.

### Ayarları Doğrulama

| Ayar | Değer |
|---|---|
| Region | EU433 / EU868 |
| Use Preset | ✅ |
| Preset | Medium Fast |
| Ignore MQTT | ⛔ |
| Ok to MQTT | ✅ |
| Transmit Enabled | ✅ |
| Override Duty Cycle | ⛔ |
| Number Of Hops | 1 - 7 |
| Frequency Slot | 1 |
| Frequency Offset | 0 |
| RX Boosted Gain | ✅ |
| Frequency Override | 433.125 (EU433) / 869.525 (EU868) |
| Transmit Power | 10 (EU433) / 22 (EU868) |


## Sonraki Adımlar

- [MQTT sunucusu için şifre edinmek ve bağlanmak.](../mqtt)