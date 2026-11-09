# 📰 News Site

HTML ve CSS ile hazırlanmış, duyarlı (responsive) bir haber sitesi arayüzü. Proje; ana sayfa, makale detay sayfası ve mobil uyumlu tasarım içerir. JavaScript veya herhangi bir framework kullanılmamıştır.

## ✨ Özellikler

- Sayfa kaydırılırken üstte sabit kalan (sticky) navigasyon çubuğu
- Arka plan görselli, öne çıkan haber alanı (header / hero)
- 3 sütunlu "Latest News" kart düzeni (CSS Grid)
- Makale detay sayfası: yazar/tarih bilgisi, kategori etiketi, yan panel (Join Us ve Categories)
- 4 sütunlu footer (logo, abonelik formu, bağlantılar, sosyal medya)
- Mobil uyumluluk: tablet ve telefon ekranları için ayrı `mobile.css`
- CSS değişkenleri ile kolay renk ve genişlik yönetimi
- Yardımcı (utility) sınıflar: `.btn`, `.card`, `.bg-primary`, `.py-2`, `.mb-4` vb.

## 🛠️ Kullanılan Teknolojiler

| Teknoloji | Kullanım |
|-----------|----------|
| HTML5 | Sayfa yapısı |
| CSS3 (Grid, Flexbox, Custom Properties) | Tasarım ve yerleşim |
| [Font Awesome 5.9.0](https://fontawesome.com/) | Sosyal medya ve arayüz ikonları |
| [Google Fonts](https://fonts.google.com/) | Lato ve Varela Round yazı tipleri |

## 📁 Proje Yapısı

HTML dosyaları kök dizinde, CSS ve görseller ise kodda belirtilen yollara uygun olacak şekilde klasörlerde durmalıdır:

```
news-site/
├── index.html          # Ana sayfa
├── about.html          # Hakkında sayfası
├── article.html        # Makale detay sayfası
├── css/
│   ├── style.css       # Ana stil dosyası
│   └── mobile.css      # Mobil / tablet stilleri
└── img/
    ├── logo.png
    ├── rowing.jpeg     # Header arka plan görseli
    ├── img-1.webp
    ├── img-2.webp
    └── img-3.webp
```

> ⚠️ `index.html` ve `article.html` içindeki yollar `css/style.css` ve `img/...` şeklindedir. Dosyaları yukarıdaki klasör yapısına yerleştirmezseniz stiller ve görseller yüklenmez.

## 🚀 Kurulum ve Çalıştırma

1. Projeyi indirin veya klonlayın:
   ```bash
   git clone https://github.com/Busrazeynep/news-site.git
   cd news-site
   ```
2. Dosyaları yukarıdaki klasör yapısına göre düzenleyin.
3. `index.html` dosyasını tarayıcıda açın.

Ek bir kurulum veya derleme adımı gerekmez. İsterseniz VS Code'daki **Live Server** eklentisiyle de çalıştırabilirsiniz.

> Font Awesome ve Google Fonts CDN üzerinden yüklendiği için ilk açılışta internet bağlantısı gerekir.

## 🎨 Renk Paleti

`style.css` içindeki `:root` değişkenleri:

| Değişken | Renk | Kullanım |
|----------|------|----------|
| `--primary-color` | `#e76f51` | Ana vurgu rengi, aktif menü, butonlar |
| `--secondary-color` | `#2a9d8f` | Kategori etiketleri, yan panel |
| `--light-color` | `#f8f9fa` | Sayfa arka planı |
| `--dark-color` | `#6c757d` | Metin bağlantıları, footer |
| `--max-width` | `1100px` | İçerik maksimum genişliği |

## 📱 Duyarlı Tasarım (Responsive)

`mobile.css`, `index.html` ve `article.html` içinde `max-width: 768px` medya sorgusuyla yüklenir.

| Ekran genişliği | Davranış |
|-----------------|----------|
| > 768px | 3 sütunlu haber kartları, yatay navbar, sosyal ikonlar görünür |
| ≤ 768px | Navbar ortalanır, sosyal ikonlar gizlenir, kartlar 2 sütuna düşer |
| ≤ 600px | Header, kartlar ve footer tek sütuna düşer; makale sayfası tek sütun olur |

## 📄 Sayfalar

- **Ana Sayfa (`index.html`)**: Öne çıkan haber ve 6 kartlık "Latest News" bölümü
- **Makale (`article.html`)**: Makale içeriği, kategori etiketi ve yan paneller
- **Hakkında (`about.html`)**: Şu an boş, içerik eklenecek
- **Blog / Contact**: Navbar'da bağlantıları var, ancak `contact.html` henüz oluşturulmadı

## 🔧 Geliştirme Notları

- Görsellerde `alt` özellikleri boş bırakıldı; erişilebilirlik için anlamlı açıklamalar eklenebilir.
- Footer'daki bağlantılar ve sosyal medya ikonları şimdilik boş (`href=""` / `#`).
- Abonelik formu henüz bir backend'e bağlı değil.

## 📜 Lisans

Bu proje eğitim amaçlı hazırlanmıştır. Dilediğiniz gibi inceleyebilir ve geliştirebilirsiniz.
