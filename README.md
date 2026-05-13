# 📰 MakaleTara

**MakaleTara**, belirlediğiniz web sitelerinden makale ve haberleri çekerek tek bir ekranda toplayan, akıllı ve tamamen tarayıcı üzerinde (istemci tarafı) çalışan modern bir **Haber/Makale Toplayıcı (Aggregator)** uygulamasıdır.

Sunucuya ihtiyaç duymadan, belirlediğiniz sitelerin içeriklerini **RSS**, **Gelişmiş HTML Scraping** ve **Yapay Zeka (AI)** gücüyle aynı anda tarar ve düzenli kartlar halinde karşınıza getirir.

![Proje Durumu](https://img.shields.io/badge/Durum-Aktif-success)
![Lisans](https://img.shields.io/badge/Lisans-MIT-blue)
![Sürüm](https://img.shields.io/badge/Sürüm-1.0.0-orange)

---

## ✨ Özellikler

* **🚀 3 Katmanlı Çoklu Tarama:** Siteleri paralel olarak tarar. Sırasıyla RSS Akışları, HTML Scraping (WordPress/Drupal destekli) algoritmaları üzerinden makaleleri toplar.
* **🤖 Yapay Zeka (AI) Destekli İçerik Çıkarımı:** Siteler veri kazımayı (scraping) engelliyorsa, sayfayı okuması ve içerikleri çekmesi için Gemini, Groq veya OpenRouter gibi ücretsiz AI modelleri devreye girer.
* **🧠 Kapsamlı Mod (AI + RSS):** Hem klasik tarama araçlarını hem de yapay zekayı aynı anda çalıştırır; elde edilen sonuçları mükerrer olanları (aynı makaleleri) eleyerek birleştirir.
* **🌐 Otomatik Yabancı Dil Çevirisi:** İncelenen makaleler belirlediğiniz dilden (örneğin Türkçe) farklı bir dilde yayınlanıyorsa, Google Translate/Lingva API kullanılarak otomatik tespit edilir ve anında çevrilir. (Çevrilen başlıkların yanına belirteç konulur).
* **🏷️ Anahtar Kelime Filtreleme:** İlgilenmediğiniz haberleri ayıklayın. Sadece sizin belirlediğiniz kelimeleri barındıran haberler listelenebilir.
* **🛡️ Güçlü CORS Aşma Sistemi:** Sunucu tarafı olmayan uygulamalardaki en büyük engel olan CORS (Cross-Origin) hatasını, üç farklı fallback proxy (AllOrigins, CorsProxy, CodeTabs) kullanarak sorunsuzca aşar.
* **📱 Mobil Uyumlu Arayüz:** Modern, estetik ve tüm cihaz boyutlarında sorunsuz görünen bir tasarıma sahiptir.
* **🔒 %100 Gizlilik:** Tüm verileriniz, API anahtarlarınız ve kaydettiğiniz site listeleri tarayıcınızın `localStorage`'ında (yerel hafıza) şifrelenmeden ancak dışarıya sızdırılmadan sadece sizin bilgisayarınızda tutulur.

---

## 🚀 Nasıl Kullanılır?

MakaleTara tamamen yerel (local) çalışacak şekilde tasarlanmıştır. Herhangi bir indirme, sunucu kurma (Node.js vb.) işlemine gerek yoktur.

1. Bu depoyu bilgisayarınıza indirin (ZIP veya Git Clone ile).
2. İndirdiğiniz klasördeki `index.html` dosyasına çift tıklayarak tarayıcınızda açın.
3. Listeden takip etmek istediğiniz sitelerin bağlantılarını ekleyin veya çıkartın.
4. **"Tara"** butonuna basın!

### Yapay Zeka (AI) Kurulumu (İsteğe Bağlı)
Eğer RSS ve standart tarama yönteminin zorlandığı sitelerden haber almak istiyorsanız, **"⚙️ AI Ayarları"** menüsünü açarak ücretsiz API anahtarlarınızı ekleyebilirsiniz.
* **Google Gemini:** `aistudio.google.com` üzerinden alınır.
* **Groq (Llama):** `console.groq.com` üzerinden alınır.
* **OpenRouter:** `openrouter.ai` üzerinden alınır.

Girdiğiniz anahtarlar sisteminizde yerel olarak saklanacaktır.

---

## 🛠️ Kullanılan Teknolojiler

* **HTML5:** Anlamsal web iskeleti.
* **Vanilla CSS3:** CSS Değişkenleri (Custom Properties), modern animasyonlar ve Flex/Grid yapıları kullanılarak sıfırdan oluşturulmuş özel bir UI.
* **Vanilla JavaScript (ES6+):** Promise (Asenkron) yapıları, Web API'leri (DOM manipülasyonu, Fetch) kullanılarak tamamen saf (framework kullanmadan) JavaScript ile geliştirildi.

---

## 📝 Gelecek Planları (Roadmap)
- [ ] Belirli saatlerde otomatik arka plan taraması.
- [ ] Okunmuş/Okunmamış makale ayrımı.
- [ ] Makaleleri favorilere (yer imlerine) ekleme özelliği.

## 🤝 Katkıda Bulunma
MakaleTara açık kaynak kodlu bir projedir. Katkıda bulunmak isterseniz lütfen *Pull Request* gönderin veya karşılaştığınız sorunlar için bir *Issue* açın.
