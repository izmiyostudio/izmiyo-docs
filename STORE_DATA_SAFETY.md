# Mağaza Veri Güvenliği Taslağı

Bu belge mevcut MVP manifestoları ve uygulama davranışı temel alınarak hazırlanmıştır. Konsola girilmeden önce release APK/AAB ile son kez doğrulanmalıdır.

## Mevcut ortak beyan

- Uygulamalar hesap açtırmaz ve giriş bilgisi toplamaz.
- Veri cihazda tutulur; uygulama sunucusuna aktarım ve bulut veritabanı yoktur.
- Reklam SDK'sı, analitik, crash reporting ve üçüncü taraf izleme yoktur.
- Mevcut MVP manifestolarında konum, kamera, mikrofon, kişi listesi ve dosya izni istenmez.
- Kullanıcı verileri uygulama silinince işletim sistemi davranışına bağlı olarak kaldırılabilir.
- Gizlilik talepleri: izmiyostudio@gmail.com

## Uygulamaya özel yerel veri

- Parça Defteri: parça adı, kategori, adet, raf/kutu, notlar, favoriler ve stok durumu.
- Görevdaş: aile/çocuk modu, görevler, ödüller, puanlar ve tamamlanma durumu.
- Saha Akış: bölge, iş emri, müşteri/ekipman notu, durum ve offline kuyruk.
- Dilekçe Cepte: dilekçe alanları, kurum, taslaklar ve PDF üretim verisi.
- OrtakSes: program/oda seçimi, yerel tepkiler, demo sohbet ve favoriler.

## Kritik güncelleme notları

Canlı sohbet, gerçek konum, fotoğraf, hesap, reklam, abonelik veya bulut senkronizasyonu eklenirse Play Data Safety ve App Store Privacy cevapları yeniden doldurulmalıdır. Görevdaş çocuk modu nedeniyle hedef kitle ve aile politikaları ayrıca incelenmelidir.
