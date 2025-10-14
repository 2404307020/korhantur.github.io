# Copilot Kullanım Talimatları (Türkçe)

Bu dosya, depoda bulunan `prompts/` klasöründeki yönergeleri kullanarak GitHub Copilot veya Copilot Chat ile etkili çalışmanız için kısa ve uygulanabilir talimatlar içerir.

Hedef
- Bu proje tek sayfalık bir GitHub Pages sitesi sağlar (`index.html`). `prompts/` içindeki her dosya sayfa bölümlerini (ana sayfa, turlar, rezervasyon, galeri, hakkında, iletişim) tanımlar ve içeriğin nasıl çıkarılıp yerleştirileceğini belirtir.

Kullanım (Kısa)
1. `prompts/` klasörünü açın ve istediğiniz bölümün `.md` dosyasını bulun (ör. `about.md`).
2. Dosyadaki talimatları okuyun — bu talimatlar hangi metinlerin, başlıkların, resimlerin ve form alanlarının çıkarılacağını belirtir.
3. Copilot'a hangi bölümün güncelleneceğini açıkça belirtin; örneğin aşağıdaki kod bloğunu kullanabilirsiniz:

```text
Lütfen "prompts/about.md" içeriğini kullanarak index.html dosyasında yer alan about bölümünü güncelle.
```

Detaylı İpuçları (En İyi Uygulamalar)
- Kısa, tek amaçlı istekler verin. Örnek:

```text
Sadece gallery bölümünü 3 resimlik bir grid ile güncelle. Her resme uygun kısa "alt" metni ekle.
```

- Çıkarma kuralları net olmalı: Başlık, alt başlık, paragraf ve görsel URL'lerini belirtin.
- Değişiklikleri küçük parçalara bölün: Birden fazla büyük değişiklik yerine her seferinde tek bir bölüm isteyin.
- Lokal test: `index.html`'i tarayıcınızda açın; sayfa görünümünü ve form davranışını kontrol edin.

Formlar ve Veriler
- Rezervasyon formu şu alanları içerir: `fullname`, `email`, `tour`, `date`, `notes`.
- Gerçek göndermeler için bir backend veya form servis sağlayıcısı gerekli. Copilot, front-end kısmını oluşturabilir ama e-posta veya saklama için sunucu kodu eklemeniz gerekir.

Deploy (GitHub Pages)
1. `index.html` dosyasını repo kökünde tutun.
2. GitHub üzerinde bu repository için Pages ayarlarını açın ve kaynak olarak `main` veya `master` dalı ve `root` dizini seçin.
3. Değişiklikleri push ettikten sonra sayfa birkaç dakika içinde yayımlanacaktır.

Geri Al ve Sürüm Kontrolü
- Büyük değişikliklerden önce bir commit oluşturun. Copilot tarafından yapılan otomatik değişiklikleri inceleyin ve beğenmezseniz git ile geri alın.

Hatalar ve Düzeltmeler
- Eğer Copilot istenmeyen değişiklik yaparsa, ilgili bölümünü `index.html` içinde eski haline geri alın ve daha kısıtlı bir prompt ile tekrar isteyin.

Yerel Önizleme (Windows PowerShell)
```powershell
# Değişiklikleri kaydettiğiniz dizinde
start .\index.html
```

Sık Kullanılan Prompt Örnekleri

```text
prompts/tours.md içeriğini kullanarak tours bölümüne 4 tur kartı ekle. Her kart; görsel, başlık, kısa açıklama, 'Detaylar' ve 'Rezervasyon' düğmesi içermeli.

prompts/reservation.md'yi kullanarak rezervasyon formunu güncelle. Form alanları ve doğrulamalar eksiksiz olmalı.
```

Notlar
- Bu dosya, geliştiricilerin ve Copilot'un aynı yönergeler üzerinden çalışmasını kolaylaştırmak için hazırlandı. Talimatlarda değişiklik yaptığınızda `prompts/` içindeki ilgili dosyanın içerğini güncelleyin.

İyi çalışmalar!

---
Not: Bu dosya, proje ilerledikçe genişletilmeli (ör. stil rehberi, erişilebilirlik checklist, test talimatları).