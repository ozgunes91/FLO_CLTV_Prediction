> **Not:** Bu proje, Miuul Veri Bilimci Bootcamp kapsamında eğitim amacıyla geliştirilmiştir. Olasılıksal CLTV modellemesini sentetik perakende verisi ile uygulamalı olarak göstermeyi hedeflemektedir.

# 📄 Proje Raporu: FLO CLTV Tahminleme

## Amaç
Olasılıksal modeller kullanarak müşteri yaşam boyu değerini (CLTV) tahmin etmek. Böylece FLO, pazarlama stratejilerini müşteri değerine göre optimize ederek kaynaklarını daha verimli kullanabilir.

## Yöntem
- Veri Temizleme: Aykırı değerler, çeyrekler arası eşiklere göre baskılandı.
- Özellik Mühendisliği: Toplam sipariş ve harcama hesaplandı; haftalık recency, frequency, T ve monetary değişkenleri üretildi.
- Modelleme:
  - BG/NBD modeli ile 3 ve 6 ay için beklenen satın alma tahminleri yapıldı.
  - Gamma-Gamma modeli ile ortalama gelir tahmini hesaplandı.
  - 6 aylık CLTV değerleri elde edildi.
- Segmentasyon: CLTV skoruna göre müşteriler A–D gruplarına ayrıldı (çeyrekliklere göre).

## Temel Bulgular
- CLTV değerleri müşteri bazında büyük farklılıklar göstermektedir.
- En üst %5’lik müşteri dilimi (CLTV > 424 TL), ortalama **592.73 TL**’lik yaşam boyu değeriyle diğer gruplardan belirgin şekilde ayrılmaktadır.
- A segmentindeki müşteriler ortalama **~385 TL** CLTV değerine sahiptir; yüksek alışveriş sıklığı ve harcama eğilimleri gösterir.

## Stratejik Öneriler
- **A Segmenti:** Kişiselleştirilmiş sadakat kampanyaları ve özel teklifler ile bu grubun bağlılığı artırılmalıdır.
- **B Segmenti:** Hedefli kampanyalarla çapraz satış ve üst satış (upsell) stratejileri uygulanabilir.
- **C Segmenti:** Bu müşteriler için terk riski yüksektir. Anlık teklifler veya hatırlatma kampanyaları ile yeniden kazanım denenebilir.
- **D Segmenti:** Düşük potansiyelli bu gruba maliyetsiz otomatik kampanyalar dışında kaynak ayrılmamalıdır.

## Sonuç
Bu tür analizler, benzer perakende uygulamalarında daha veriye dayalı pazarlama kararları alınmasına katkı sağlayabilir.