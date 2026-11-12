# Sürüm notları

## 0.2.1

- voe artık Apple’ın Developer ID imzasıyla imzalanıyor ve Apple tarafından **notarize ediliyor**: “Mac’inizi korumak için engellendi” uyarısı ve “Yine de Aç” adımı yok.
- Kamera, mikrofon ve konum izinleri macOS’un korumalı çalışma ortamına (hardened runtime) uygun hâle getirildi.

## 0.2.0 — gizlilik ve senkron

**Gizlilik: internet sağlayıcın neye baktığını görmez**
- Şifreli DNS (DNS-over-HTTPS) varsayılan açık; katı mod düz DNS’e hiç düşmez. Sağlayıcı seçilebilir (Cloudflare, Quad9, Mullvad, AdGuard, Google, özel).
- Şifreli site adı (ECH): destekleyen sitelerde bağlanılan alan adı da gizli.
- Önce HTTPS: her adres şifreli bağlantıyla açılır; HTTPS sunmayan ya da sertifikası geçersiz sitelerde önce sorulur.
- Yerel veriler diskte şifreli (AES-256-GCM, anahtar Anahtar Zinciri’nde): geçmiş, yer imleri, okuma listesi, oturum, ayarlar.
- Global Privacy Control sinyali ve WebRTC IP koruması.
- Ayarlar’da canlı **Gizlilik denetimi**.

**Senkron: uçtan uca şifreli, hesapsız**
- Yer imleri (klasörleriyle), şifreler, geçmiş, açık sekmeler, okuma listesi ve ayarlar Mac ile telefon arasında eşitlenir.
- QR koduyla eşleşme; sunucu yalnızca şifreli blokları görür. “Diğer cihazlardaki sekmeler” ⋮ menüsünde ve komut paletinde.

**Diğer**
- Yeni sekmede yazılanlar doğrudan adres çubuğuna gider.

## 0.1.0 — ilk sürüm

**Geliştiriciler için**
- Geliştirici paneli (`⇧⌘E`): konsol hataları, cihaz öykünmesi (iPhone, Pixel, iPad; döndürme), tema ve ağ hızı öykünmesi, önbellek ve JavaScript anahtarları, hareketi azalt, yazdırma görünümü, öğe çerçeveleri, sayfayı düzenleme, sayfa künyesi (yığın, barındırma, güvenlik başlıkları), site verilerini silme.
- Yerel sunucular: çalışan geliştirme sunucuları yeni sekmede, adres çubuğunda ve komut paletinde.
- Telefonda test et: `localhost` sayfaları yerel ağ adresiyle QR koduna dönüşür; erişim denetlenir.
- JSON görüntüleyici: katlanabilir ağaç, arama, yol kopyalama, büyük tam sayılar.
- Araç Kutusu (`⌥⌘T`): JSON, JWT, Base64, URL, zaman damgası, UUID, Hash, renk, Regex.
- Yerel sayfalarda konsol hatası sayacı.

**Tarayıcı**
- voe Kalkanı (reklam, izleyici ve çerez uyarısı engelleme), komut paleti, canlı sekme sürükleme, sekme grupları, bölünmüş ekran, sekme uyutma, okuma modu ve okuma listesi, odak oturumu, telefona gönder, ekran görüntüsü, resim içinde resim, hız ölçer, şifre yöneticisi, Chrome eklentileri, Vakit ve zikirmatik.
- Yeni sekmede imleç adres çubuğunda; ortadaki arama kutusuna tıklayınca yazılanlar adres çubuğuna gider.
- Otomatik güncelleme denetimi (GitHub sürümleri; Ayarlar’dan kapatılabilir).
