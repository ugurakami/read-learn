# 📖 Read & Learn

İngilizce kitap okuyarak kelime öğrenmek için tasarlanmış, **tek dosyalık**, mobil uyumlu bir web uygulaması. Project Gutenberg'den indirdiğiniz herhangi bir klasik romanla çalışır.

---

## ✨ Özellikler

- 📚 **Herhangi bir kitap** — Project Gutenberg `.txt` dosyası yükle
- 👆 **Tıkla-çevir** — kelimeye dokun, anında Türkçe karşılığını gör
- 🔊 **Telaffuz** — Web Speech API ile kelimeyi dinle
- 💾 **Kelime defteri** — beğendiğin kelimeleri kaydet (`localStorage`)
- 🧠 **Quiz modu** — flashcard tarzı tekrar
- 🎯 **Odak modu** — sadece kaydedilmiş kelimeleri vurgula
- 📊 **Paragraf istatistiği** — her paragrafta kaç kayıtlı kelime geçtiğini gör
- 🔥 **Zor kelime işareti** — quiz'de bilemediklerin metinde kırmızı çizgiyle işaretlenir
- 💬 **Cümle bağlamında çeviri** — kelimenin içinde bulunduğu cümleyi de çevir
- 📱 **Mobil uyumlu** — iPhone/Android'de "Ana ekrana ekle" ile uygulama gibi çalışır
- 🎨 **Koyu tema** — göz yormayan okuma deneyimi

---

## 🚀 Hızlı Başlangıç

### 1. Kitabı indir

[Project Gutenberg](https://www.gutenberg.org/) → bir kitap seç (ör. *Alice in Wonderland*, *Sherlock Holmes*, *Great Gatsby*) → **"Plain Text UTF-8"** formatında indir.

### 2. Dosyaları hazırla

Proje klasörüne şu iki dosyayı koy:

index.html
book.txt ← Gutenberg'den indirdiğin metin
text


> 💡 Gutenberg başlık/son uyarılarını **silmek zorunda değilsin** — uygulama bunları otomatik temizler.

### 3. Yerel test

`fetch()` için HTTP sunucusu gerekir. Python ile:

```bash
cd proje-klasörü
python -m http.server 8000

Tarayıcıda: http://localhost:8000
4. Yayına al

GitHub Pages, Netlify Drop veya Vercel ile ücretsiz yayınla. Detaylar için DEPLOY.md.
5. Telefona kur

    Android (Chrome): Menü → "Ana ekrana ekle"

    iPhone (Safari): Paylaş → "Ana Ekrana Ekle"

📖 Okuma Stratejisi (Öneri)

Bu uygulama tek seferlik okuma için değil, 3 aşamalı tekrarlı okuma için tasarlandı:
🥇 1. Okuma — "Anlama"

    Hikâyeyi takip et, akışı bozmadan oku

    Her sayfada en fazla 3-5 kelime kaydet

    Sadece anlamı bozan, kritik kelimeleri seç

🥈 2. Okuma — "Kelime Avı" (1-2 hafta sonra)

    Odak modunu aç 🎯

    Sadece kaydettiğin kelimeler vurgulanır, diğerleri soluklaşır

    Yeni kelime kaydetme — sadece pekiştir

    Paragraf rozetleriyle ilerlemeni takip et

🥉 3. Okuma — "Yapı ve Kalıp" (1 ay sonra)

    Deyimlere, phrasal verb'lere, bağlaçlara odaklan

    Her bölümden 1-2 cümleyi kendi kelimelerinle yeniden yaz

🧠 Quiz — Her Hafta 1-2 Kez

    Defterindeki kelimelerden flashcard quiz

    Bilemediklerin metinde kırmızı çizgi ile işaretlenir 🔥

    Bir sonraki okumada o kelimelere özellikle dikkat et

🎛️ Arayüz Rehberi
Buton	İşlev
🎯 Odak	Sadece kayıtlı kelimeleri vurgula (2. okuma için)
🧠 Quiz	Flashcard quiz başlat (min. 5 kelime)
📚 Defter	Kaydettiğin tüm kelimeleri listele
🔊 Dinle	Kelimenin telaffuzunu dinle
💾 Kaydet	Kelimeyi deftere ekle
💬 Cümle bağlamında	Kelimenin içinde bulunduğu cümleyi çevir
🛠️ Teknik Detaylar
Bileşen	Teknoloji
Framework	Yok (vanilla HTML/CSS/JS)
Çeviri API	MyMemory (ücretsiz, anahtarsız)
Ses	Web Speech API (speechSynthesis)
Depolama	localStorage (cihaza özel)
Tasarım	Mobile-first, safe-area destekli
Boyut	~25 KB (tek dosya, harici bağımlılık yok)
Sınırlar

    MyMemory günlük limiti: ~5000 karakter (kelime değil). Normal okuma için fazlasıyla yeterli.

    localStorage cihaza özeldir — telefon ve bilgisayar ayrı defter tutar.

    Gizli mod: Tarayıcının gizli modunda kayıtlar kapanınca silinir.

📁 Dosya Yapısı
text

read-learn-pro/
├── index.html       # Tüm uygulama (HTML + CSS + JS)
├── book.txt         # Okunacak kitap (Project Gutenberg)
├── README.md        # Bu dosya
└── DEPLOY.md        # Yayınlama rehberi

🤝 Katkı

Bu proje kişisel öğrenme için tasarlandı ama önerilere açık. 
📜 Lisans

MIT — dilediğin gibi kullan, değiştir, paylaş.

Kitaplar Project Gutenberg'den gelir ve kendi lisanslarına tabidir (genellikle public domain).
🙏 Teşekkür

    Project Gutenberg — ücretsiz klasikler

    MyMemory — ücretsiz çeviri API'si

    Web Speech API — tarayıcı yerel telaffuz

İyi okumalar! 📚

---

