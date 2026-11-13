# Sürüm notları

## 0.2.9

- **Yeni sekme yeniden düzenlendi:** kısayollar logonun hemen altında, kartlar onların altında; kartlar aynı boyda, düzgün bir ızgarada.
- **Dokuz yeni kart:** Haberler (Hacker News, BBC Türkçe, Webrazzi, GitHub Blog ya da kendi RSS/Atom adresin), Son depremler (Türkiye ve çevresi, en yakın ile göre), Namaz vakitleri, Dünya saatleri, Takvim (hicri tarihle), Geri sayım, Notlar (kartın içine yaz, otomatik kaydedilir), Yapılacaklar ve Okuma listesi.
- **Hava durumunda birden çok şehir:** Vakit şehrinin yanına istediğin şehirleri ekle; Türkiye'deki iller anında, dünyadaki tüm şehirler aramayla bulunur.
- **Sürükle-bırak:** kartı herhangi bir yerinden tutup sürükle; diğer kartlar akıcı biçimde yer açar, Esc iptal eder. Kart menüsünde "Sola taşı / Sağa taşı" da var.
- **Şifre otomatik doldurma listesi yenilendi:** sayfanın açık/koyu rengine uyar, alanın genişliğinde açılır, yazdıkça süzülür ve eşleşen kısmı vurgular; ↑ ↓ ile gezinip Enter ile doldurursun, Esc kapatır. Aşağıda yer yoksa yukarı açılır; altta "Şifreleri yönet" bağlantısı var.

## 0.2.8

- Yeni sekme artık ekrana sığıyor; gereksiz dikey kaydırma kaldırıldı (boşluklar derli toplandı).

## 0.2.7

- Senkron sayfasında “Diğer cihazlardaki sekmeler” bölümünde site simgesi kocaman görünüyordu; düzeltildi.

## 0.2.6

- **Yeni bir bilgisayarı kamerayla eşleştir:** Senkron sayfasında **“Kamerayla tara”** ile, telefonundaki ya da başka bir bilgisayardaki **Cihaz ekle** QR kodunu okutup zincire katıl — artık uzun eşleştirme bağlantısını cihazlar arasında taşımana gerek yok. Bağlantıyı yapıştırma seçeneği de duruyor. (Mobilde eşleştirme QR'ı okutma zaten vardı.)
- **İçe aktarmada yardım:** Bir tarayıcı bulunup da verisine erişilemezse (ör. voe'ya **Tam Disk Erişimi** verilmemişse), içe aktarma sayfası artık bunu söyleyip ayarları açan bir düğme gösterir. voe'yu dmg içinden değil, **Uygulamalar** klasöründen çalıştırın.

## 0.2.5

- **Chrome’dan (ve Edge, Brave, Vivaldi, Opera, Chromium’dan) tek adımda içe aktarma:** ⋮ → **Tarayıcıdan İçe Aktar…** ya da Şifreler sayfasındaki şerit, kurulu tarayıcıları ve her birindeki öğe sayısını (yer imi, şifre, kart, adres, geçmiş) bulur; neyin aktarılacağını seçip tek düğmeyle taşır. voe ilk açılışta da önerir.
  - **Şifreler ve kayıtlı kartlar** çözülürken macOS bir kez izin ister; bu olmadan diğer türler yine aktarılır. Çözme tamamen bu cihazda olur, hiçbir veri dışarıya gönderilmez.
  - **Yer imleri, adresler ve geçmiş** (son 180 gün) izne gerek olmadan aktarılır. Daha önce aktarılanlar tekrar eklenmez.
- **Kayıtlı kartlar ve adresler:** Şifreler sayfasına kart ve adres bölümleri eklendi. Kart numaraları diskte şifreli saklanır; görmek ya da kopyalamak için Touch ID istenir, pano 60 sn sonra temizlenir.

## 0.2.4

- **Yeni sekmede kendi kartların:** “+ Kart ekle” ile
  - **Piyasa** — Dolar, Euro, Sterlin, Gram altın, Ons altın, Bitcoin, Ethereum, BIST 100, S&P 500, Nasdaq ya da kendi Yahoo sembolün; fiyat, günlük değişim ve küçük gün içi grafik (Yahoo Finance, dakikada bir yenilenir).
  - **Siteler** — “İş”, “Sunucular” gibi adlandırdığın hızlı erişim listeleri.
  - **Hava durumu** — Vakit’te seçili şehir için sıcaklık, durum, en yüksek / en düşük (Open-Meteo).
  - Kartlar sürükleyerek sıralanır, ⋯ menüsünden düzenlenir ya da kaldırılır. Veriler yalnızca eklediğin kartlar için istenir; kartlar diskte şifreli saklanır.
- Yeni sekmedeki arama kutusu kaldırıldı: arama ve adresler üstteki adres çubuğundan.

## 0.2.3

- **İndirilenler kartı:** araç çubuğundaki indirme düğmesi Chrome’daki gibi son indirmeleri gösteren bir kart açar: ilerleme ve kalan süre, duraklat / devam et / iptal, tamamlananı aç ya da Finder’da göster, altta “Tüm indirilenler”. Yeni indirme başladığında kart birkaç saniyeliğine kendiliğinden açılır.
- **Geçersiz sertifikalı sitelere bilerek girme:** hata sayfasında “Gelişmiş” → sertifika ayrıntıları ve “Yine de … sitesine git (güvenli değil)”. İzin yalnızca o site ve o sertifika için, voe kapanana kadar geçerlidir; adres çubuğu “Güvenli değil” gösterir. Kendinden imzalı sertifika kullanan yönetim panelleri ve yerel sunucular için.

## 0.2.2

- Adres çubuğunda sade bir gösterge: kilidin köşesindeki küçük nokta, o sitede **site adının da gizli** olduğunu (ECH) gösterir. Kilide tıklayınca tek satırla açıklanır; üzerine gelince ayrıntı görünür.

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
