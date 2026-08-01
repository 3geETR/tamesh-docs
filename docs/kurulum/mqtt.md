# MQTT

MQTT, kısaca RF ile haberleşemeyen cihazların bir sunucu üzerinden Wi-Fi ile haberleşmesini sağlayan bir sistemdir. Meshtastic cihazları, bu sunucu üzerinden internete bağlanarak harita görüntüleme ve uzak düğümlerle iletişim gibi özellikleri kullanabilir.
[Detaylı Bilgi](https://purg.tr/mqtt-bilgi)

## TAMesh MQTT Sunucusu

TAMesh topluluğu **kendi MQTT sunucusunu** kullanır. Sunucuya katılmak için aşağıdaki formu doldurarak başvuruda bulunmanız gerekir:

[Başvuru Formu](https://form.tamesh.org/)

!!! info "Başvuru süreci"
    Formu doldurduktan sonra başvurunuz değerlendirilir ve sunucuya erişim için gerekli bilgiler sizinle paylaşılır.

## MQTT Ayarları

Cihazınızda aşağıdaki MQTT ayarlarını yapılandırın:

| Ayar | Değer |
|---|---|
| Address | mqtt.tamesh.org |
| Encryption | ⛔ |
| JSON | ⛔ |
| TLS | ⛔ |
| Root Topic | msh |
| Proxy to Client | ✅ |
| Map Report | ✅/⛔ |
| Precise Location | ✅/⛔ |
| Reporting Interval | 900 |
