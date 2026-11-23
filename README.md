# Rize Barosu Adli Yardım Görev Çizelgesi

Rize Barosu Adli Yardım Komisyonu'nun görev dağıtımı için hazırlanmış telefon uyumlu bir web uygulaması.

- **Sıra:** Görev, kıdemi en düşük aktif avukattan başlar. Dönemde en az görev alan önce gelir; eşitlikte kıdemi en düşük olan seçilir. Merkez-Çayeli ve Pazar listeleri ayrı tutulur.
- **Herkes görür:** Bağlantıyı açan herkes güncel listeyi, sırayı, bütün görev kayıtlarını ve istatistikleri görür. Giriş gerekmez.
- **Yetkililer düzenler:** Görev verme, atlama, iade, kayıt düzenleme ve avukat durumu değiştirme işlemleri yalnızca erişim anahtarıyla giriş yapanlara açıktır. Her değişiklik `data.json` dosyasına, yapanın adıyla birlikte kaydedilir. Değişiklik geçmişi uygulamada ve GitHub'da tutulur.
- **Çevrimdışı çalışır:** Ana ekrana eklenebilir. İnternet yokken son görülen veriyi gösterir.

## Yönetici erişim anahtarı nasıl alınır

1. GitHub'da **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token** yolunu izleyin.
2. **Repository access:** "Only select repositories" seçeneğini işaretleyip yalnızca bu depoyu seçin.
3. **Permissions → Repository permissions → Contents:** "Read and write" olarak ayarlayın.
4. Oluşan anahtarı uygulamada **Yönetim** sekmesine adınızla birlikte girin.

Anahtar yalnızca girildiği cihazda saklanır. Bir yetkiliyi çıkarmak için o kişinin anahtarını GitHub'dan iptal etmeniz yeterlidir.

## Dosyalar

| Dosya | İçerik |
| --- | --- |
| `index.html` | Uygulamanın kendisi |
| `data.json` | Avukat listesi, görev kayıtları, değişiklik geçmişi (tek doğru kaynak) |
| `sw.js`, `manifest.webmanifest`, `icon*` | Ana ekrana ekleme ve çevrimdışı çalışma |

Kıdem bilgileri Rize Barosu'nun 23.11.2026 tarihli kıdeme göre sicil listesinden alınmıştır.
