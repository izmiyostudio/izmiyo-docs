# Supabase Karar Notu

## Sonuç

Mevcut MVP sürümlerinde Supabase kullanılmayacak. Hesap, canlı senkronizasyon, uzak veritabanı ve gerçek zamanlı topluluk özellikleri etkin değil; bu nedenle Supabase eklemek gereksiz maliyet ve ek gizlilik yükü oluşturur.

## Uygulama bazında

- Parça Defteri: Şimdilik gerekmez. İleride cihazlar arası senkronizasyon ve ekip stoğu gelirse düşünülebilir.
- Görevdaş: Şimdilik gerekmez. Aile paylaşımı, ebeveyn hesabı ve çoklu cihaz gelirse gerekir.
- Saha Akış: MVP için gerekmez. Gerçek ekip, rol bazlı erişim, iş emri senkronizasyonu ve yönetici paneli aşamasında gerekir.
- Dilekçe Cepte: Gerekmez. Hassas belge verilerini sunucuya taşımamak daha güvenlidir. Şablon güncellemesi için ayrı, anonim içerik servisi değerlendirilebilir.
- OrtakSes: Demo MVP için gerekmez. Gerçek kullanıcı, canlı oda, sohbet, moderasyon, takip ve bildirim açılınca backend gerekir; Supabase uygun adaydır ancak telif ve moderasyon mimarisi ayrıca tasarlanmalıdır.

## Supabase'e geçiş tetikleyicileri

1. Kullanıcı hesabı veya cihazlar arası senkronizasyon.
2. Gerçek zamanlı sohbet/oda veya takip sistemi.
3. Yönetici paneli ve rol bazlı erişim.
4. Sunucu doğrulamalı premium/abonelik veya erişim kodu.
5. Push bildirimleri ve güvenli dosya depolama.

Geçiş yapılırsa RLS politikaları, Edge Functions, rate limit, KVKK saklama süresi, silme/export akışı ve mağaza veri beyanları birlikte hazırlanmalıdır. Anonim anahtar uygulamaya gömülebilir; service-role anahtarı kesinlikle gömülmemelidir.
