<p align="center">
  <img src=".github/assets/banner-tr.png" alt="voe — Web’i yapanlar için. Kullananlar için de." width="100%">
</p>

<p align="center">
  <b>Türkçe</b> · <a href="README.en.md">English</a>
</p>

<p align="center">
  <a href="https://github.com/dev-cagri/voe/releases/latest"><img alt="Son sürüm" src="https://img.shields.io/github/v/release/dev-cagri/voe?style=flat-square&label=s%C3%BCr%C3%BCm&color=1c1c21&labelColor=0b0b0d"></a>
  <img alt="macOS 12+" src="https://img.shields.io/badge/macOS-12%2B-1c1c21?style=flat-square&labelColor=0b0b0d&logo=apple&logoColor=white">
  <img alt="Apple Silicon" src="https://img.shields.io/badge/Apple%20Silicon-arm64-1c1c21?style=flat-square&labelColor=0b0b0d">
  <img alt="Chromium 156" src="https://img.shields.io/badge/Chromium-156-1c1c21?style=flat-square&labelColor=0b0b0d">
  <a href="https://github.com/dev-cagri/voe/releases"><img alt="İndirme" src="https://img.shields.io/github/downloads/dev-cagri/voe/total?style=flat-square&label=indirme&color=1c1c21&labelColor=0b0b0d"></a>
</p>

<p align="center">
  <a href="https://github.com/dev-cagri/voe/releases/latest/download/voe-mac-arm64.dmg"><b>macOS için indir</b></a>
  &nbsp;·&nbsp; <a href="#voe-mobil">iOS (TestFlight)</a>
  &nbsp;·&nbsp; <a href="https://github.com/dev-cagri/voe/releases">Tüm sürümler</a>
  &nbsp;·&nbsp; <a href="https://github.com/dev-cagri/voe/issues/new/choose">Geri bildirim</a>
</p>

<br>

**voe**, Chromium tabanlı, sade ve hızlı bir macOS tarayıcısı. Günlük gezinmeyi sakinleştirir; web geliştirenlerin her gün açıp kapattığı araçları da tarayıcının içine, tek tıka koyar. Cihaz öykünmesi, konsol hataları, yerel sunucular, JSON görüntüleyici ve çevrimdışı bir araç kutusu hazır gelir. Reklam ve izleyici engelleyici **voe Kalkanı** her zaman açıktır.

<p align="center">
  <img src=".github/assets/screen-newtab.png" alt="voe yeni sekme: noktalı ızgara, ortada logo ve arama, kısayollar ve çalışan yerel sunucular" width="100%">
</p>

> [!NOTE]
> Bu depo voe’nun **sürümlerini, sürüm notlarını ve geri bildirimleri** barındırır. voe ücretsizdir; kaynak kodu açık değildir.

---

## Geliştiriciler için

<table>
  <tr>
    <td width="50%" valign="top">
      <img src=".github/assets/dev-panel.png" alt="Geliştirici paneli">
      <h3>Geliştirici paneli <code>⇧⌘E</code></h3>
      Araç çubuğundaki <code>&lt;/&gt;</code> düğmesi her sekme için bir panel açar. Sayfanın konsol hatalarını listeler. Kullanılan çatıları (React, Next.js, Vue, Svelte, Astro, Vite, Tailwind…), sunucuyu ve barındırmayı (Cloudflare, Vercel, Netlify…), HTTP durumunu, protokolü ve güvenlik başlıklarını (HSTS, CSP, çerçeve koruması, nosniff…) gösterir.
    </td>
    <td width="50%" valign="top">
      <img src=".github/assets/dev-iphone.png" alt="iPhone öykünmesi">
      <h3>Cihaz ve ağ öykünmesi <code>⇧⌘M</code></h3>
      Tek tıkla iPhone, Pixel ya da iPad. Sayfa gerçekten o genişliğe iner ve ortalanır. User-Agent, dokunma ve piksel oranı da değişir; istersen yatay çevirebilirsin. Açık ya da koyu tema, Hızlı 3G, Yavaş 3G ya da çevrimdışı ağ seçilebilir. Önbellek, JavaScript, “hareketi azalt”, yazdırma görünümü, öğe çerçeveleri ve sayfayı yerinde düzenleme anahtarlarla açılıp kapanır. Hepsi yalnızca o sekmeyi etkiler, kapatınca iz bırakmaz.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src=".github/assets/json-viewer.png" alt="JSON görüntüleyici">
      <h3>JSON görüntüleyici</h3>
      API yanıtları katlanabilir, aranabilir bir ağaç olarak açılır; 10 MB’lık bir belge bile anında görünür. Bir anahtara tıklayınca yolu (<code>data.items[3].name</code>) kopyalanır. Büyük tam sayılar basamak kaybetmez ve “Ham” görünüme tek tıkla geçilir.
    </td>
    <td width="50%" valign="top">
      <img src=".github/assets/toolbox.png" alt="Araç Kutusu">
      <h3>Araç Kutusu <code>⌥⌘T</code></h3>
      <code>voe://toolbox</code> içinde dokuz araç var: JSON biçimlendirme ve doğrulama, JWT çözücü, Base64, URL kodlama ve ayrıştırma, Unix zaman damgası, UUID v4/v7, Hash (SHA, MD5, HMAC), renk dönüştürme ve WCAG kontrastı, Regex. Hepsi çevrimdışı çalışır; yapıştırdığın token sayfadan dışarı çıkmaz.
    </td>
  </tr>
</table>

- **Yerel sunucular.** voe, bu Mac’te çalışan geliştirme sunucularını kendiliğinden bulur: Vite, Next.js, Nuxt, Astro, SvelteKit, Angular, Storybook, Django, Flask, FastAPI, Rails, Laravel, Express… Bunları yeni sekmede, adres çubuğunda (`local` ya da `:5173` yazınca) ve komut paletinde sayfa başlıklarıyla gösterir.
- **Telefonda test et.** `localhost` sayfasında QR düğmesine bas: adres Mac’in yerel ağ IP’sine çevrilir, aynı Wi-Fi’deki telefon sayfayı açar. Sunucu yalnızca localhost’u dinliyorsa voe bunu fark eder ve `vite --host` gibi çözümü gösterir.
- **Hata sayacı.** Yerel geliştirme sayfalarında JavaScript hatası olunca `</>` düğmesinde kırmızı bir sayaç belirir.
- **Tek tıkla temizlik.** “Site verilerini sil” düğmesi o sitenin çerezlerini, depolamasını ve service worker’larını silip sayfayı yeniler. Sert yenileme ve sayfa kaynağı da bir tık uzakta.
- **Tam Chromium DevTools** her zaman `⌥⌘I` ile açılır.

## Gizlilik: neye baktığın yalnızca seni ilgilendirir

İnternet sağlayıcın ve aynı ağdakiler, sıradan bir tarayıcıda hangi sitelere girdiğini görebilir. voe bunu varsayılan olarak kapatır:

- **Şifreli DNS (DNS-over-HTTPS).** Açtığın sitelerin adları şifreli sorulur. **Katı mod** düz DNS’e hiç düşmez. Sağlayıcı olarak Cloudflare, Quad9, Mullvad, AdGuard ya da kendi sunucun seçilebilir.
- **Şifreli site adı (ECH).** Destekleyen sitelerde bağlandığın alan adı, şifreli bağlantının başında bile görünmez.
- **Önce HTTPS.** Adresler her zaman şifreli bağlantıyla açılır. Site desteklemiyorsa devam etmeden önce sorulur.
- **Verilerin cihazda şifreli.** Geçmiş, yer imleri, okuma listesi, oturum ve şifreler diskte AES-256-GCM ile saklanır; anahtar macOS Anahtar Zinciri’ndedir.
- **İzleyici engelleme, GPC ve WebRTC koruması.** voe Kalkanı izleyicileri durdurur. Sitelere “verimi satma” sinyali gider ve yerel IP adresin sızmaz.
- **Gizlilik denetimi.** Ayarlar’daki tek bir düğme hepsini canlı olarak doğrular.

## Senkron: uçtan uca şifreli, hesapsız

Yer imleri (klasörleriyle), şifreler, geçmiş, açık sekmeler, okuma listesi ve ayarlar Mac’in ve telefonun arasında eşitlenir. Hesap ya da e-posta yoktur. Masaüstündeki **Senkron** sayfasında QR kodunu telefonla okutman yeterli.

Her kayıt cihazda **AES-256-GCM** ile şifrelenir. Sunucu yalnızca anlamsız şifreli blokları görür: URL, başlık ya da şifre göremez. Anahtar yalnızca senin cihazlarında durur. Kaybolan bir cihazın erişimini **Senkronu sıfırla** ile tek adımda kesebilirsin.

## Her gün için

| | |
|---|---|
| **voe Kalkanı** | Reklam ve izleyici engelleme, çerez uyarılarını gizleme, site bazında kapatma, yeni sekmede istatistikler |
| **Komut paleti** `⌘K` | Sekmeler, komutlar, yer imleri ve geçmiş tek kutuda; Türkçe karakterlere duyarsız arama |
| **Sekmeler** | Chrome’daki gibi canlı sürükleme (ayır, başka pencereye birleştir), renkli sekme grupları, bölünmüş ekran `⌥⌘S` |
| **Sekme uyutma** | Kullanılmayan sekmelerin belleği boşaltılır; tıklayınca kaldığı yerden açılır |
| **Okuma** | Okuma modu `⌥⌘R` ve çevrimdışı okuma listesi `⇧⌘D` |
| **Odak oturumu** | Pomodoro süresince dikkat dağıtan siteler sakin bir sayfada bekletilir |
| **Telefona gönder** | Sayfanın QR kodu cihazda üretilir; voe mobil ya da kamera ile okut |
| **Ekran görüntüsü** | `⇧⌘2` görünür alan, `⌥⇧⌘2` tam sayfa |
| **Şifreler** | Anahtar Zinciri ile şifreli saklama, otomatik doldurma, Touch ID ile gösterme |
| **Eklentiler** | Chrome Web Mağazası’ndan kurulum |
| **Hız ölçer** | Adres çubuğunda sayfa yükleme süresi; DNS’ten indirmeye ayrıntılı döküm |
| **Tarayıcıdan içe aktar** | Chrome, Edge, Brave, Vivaldi, Opera ve Chromium’dan yer imleri, şifreler, kayıtlı kartlar, adresler ve geçmişi tek adımda — her şey cihazda kalır |
| **Vakit** | Sıradaki ezan vaktine kalan süre, hicri tarih ve zikirmatik (cihazda hesaplanır) |

## voe mobil

<p align="center">
  <img src=".github/assets/mobile-newtab.png" alt="voe mobil yeni sekme" width="23%">
  <img src=".github/assets/mobile-scroll.png" alt="Kaydırınca çekilen araç çubukları" width="23%">
  <img src=".github/assets/mobile-address.png" alt="Adres düzenleyici" width="23%">
  <img src=".github/assets/mobile-vakit.png" alt="Vakit ve zikirmatik" width="23%">
</p>

iOS sürümü **TestFlight** beta aşamasında, Android sürümü hazırlanıyor. Masaüstüyle aynı sade tasarımda gelir:
- Adres çubuğu üstte; kaydırınca araç çubukları çekilir.
- Sekme ızgarası ve gizli sekmeler var.
- voe Kalkanı ve okuma modu var.
- “Masaüstünden Al” ile masaüstündeki “Telefona Gönder” QR kodunu okutup sayfayı açabilirsin.

## Kurulum

1. **[voe-mac-arm64.dmg](https://github.com/dev-cagri/voe/releases/latest/download/voe-mac-arm64.dmg)** dosyasını indir, aç ve **voe**’yu **Uygulamalar** klasörüne sürükle.
2. voe, Apple’ın Developer ID imzasıyla imzalanmış ve Apple tarafından **notarize edilmiştir**; ilk açılışta yalnızca “internetten indirildi, açılsın mı?” sorusu çıkar.
3. İstersen **Ayarlar → Varsayılan tarayıcı** bölümünden voe’yu varsayılan tarayıcın yap. Chrome, Edge, Brave gibi tarayıcılardaki yer imlerini, şifreleri, kartları, adresleri ve geçmişi **⋮ → Tarayıcıdan İçe Aktar…** ile tek adımda taşıyabilirsin.

**Gereksinimler:** macOS 12 Monterey ya da üzeri, Apple Silicon (M1 ve sonrası).

## Güncellemeler

voe açılışta ve 6 saatte bir bu deponun [son sürümüne](https://github.com/dev-cagri/voe/releases/latest) bakar. İstek yalnızca uygulama sürümünü içerir. Yeni sürüm varsa ⋮ menüsünde haber verir; **İndir** dersen `.dmg` voe’nun kendi indirme yöneticisine düşer. Hiçbir şey kendiliğinden kurulmaz. Bu denetim **Ayarlar → Güncellemeler** bölümünden kapatılabilir.

## Klavye kısayolları

| Kısayol | Ne yapar | Kısayol | Ne yapar |
|---|---|---|---|
| `⌘K` | Komut paleti | `⇧⌘E` | Geliştirici paneli |
| `⌘L` | Adres çubuğu | `⇧⌘M` | iPhone öykünmesi aç/kapat |
| `⇧⌘T` | Kapatılan sekmeyi geri aç | `⌥⌘T` | Araç Kutusu |
| `⌥⌘S` | Bölünmüş ekran | `⌥⌘I` | Chromium DevTools |
| `⇧⌘F` | Odak modu | `⌥⌘U` | Sayfa kaynağı |
| `⌥⌘R` | Okuma modu | `⇧⌘R` | Önbelleği atlayarak yenile |
| `⇧⌘D` | Okuma listesine ekle | `⇧⌘2` / `⌥⇧⌘2` | Ekran görüntüsü / tam sayfa |

## Veri ve telemetri

- Telemetri yok: kullanım istatistiği, çökme raporu ya da reklam kimliği toplanmaz.
- Veriler yalnızca cihazlarında durur. Senkron açıksa sunucuya yalnızca uçtan uca şifreli kayıtlar gider.
- Yerel sunucu taraması, Araç Kutusu, JSON görüntüleyici ve QR kodları tamamen cihazda çalışır.
- voe kendiliğinden yalnızca üç bağlantı kurar: Kalkan filtre listelerinin güncellenmesi, yer imlerinin site simgeleri ve güncelleme denetimi. Güncelleme denetimi GitHub’a gider, yalnızca sürüm bilgisini içerir ve kapatılabilir.

## Geri bildirim

Hata mı buldun, bir fikrin mi var? [Yeni bir kayıt aç](https://github.com/dev-cagri/voe/issues/new/choose). Hata bildirirken voe sürümünü (**⋮ → voe Hakkında**) ve macOS sürümünü yazman yeterli.

## Lisans

voe ücretsizdir; kaynak kodu açık değildir. Ayrıntılar için [LICENSE](LICENSE) dosyasına bak. voe; [Electron](https://www.electronjs.org/) ve Chromium (MIT/BSD), [Ghostery adblocker](https://github.com/ghostery/adblocker) (MPL-2.0), [Mozilla Readability](https://github.com/mozilla/readability) (Apache-2.0), [electron-chrome-extensions](https://github.com/samuelmaddock/electron-browser-shell) (MIT), [adhan-js](https://github.com/batoulapps/adhan-js) (MIT), [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) (MIT) ve [Sora](https://github.com/sora-xor/sora-font) (OFL-1.1) gibi açık kaynak projelere dayanır; bu projelerin lisansları kendi koşullarıyla geçerlidir.

<p align="center"><sub>© 2026 voe</sub></p>
