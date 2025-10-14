# About prompt

Use this to update the about section.
 # prompts/about.md

Amaç: `index.html` içindeki `#about` bölümünü güncellemek için Copilot tarafından kullanılacak açık, adım adım bir prompt ve eklenmesi istenen içerik.

Yapılacaklar (özet):
- `#about` bölümünü aşağıdaki metin ile değiştirin.
- Bölüme bir kısa intro, misyon, ekip özetleri ve iki müşteri yorumu ekleyin.
- HTML yapısını koruyun (başlık, paragraflar, grid kartları). Erişilebilir `aria-labelledby` ve anlamlı `alt`'lar ekleyin.

Eklenecek içerik (kopyala ve yapıştırılacak):

<section id="about">
	<div class="max-w-6xl mx-auto p-6">
	<h2 class="text-2xl font-semibold mb-4">Hakkımızda</h2>
	<p class="text-slate-600 mb-4">Korgezi, Türkiye'nin benzersiz kültürel ve doğal güzelliklerini keşfetmeyi kolaylaştıran bir tur platformudur. Misyonumuz güvenli, sürdürülebilir ve unutulmaz deneyimler sunmaktır.</p>
	<div class="grid gap-6 md:grid-cols-2">
	<div>
	<h3 class="font-semibold">Misyonumuz</h3>
	<p class="text-slate-600">Yerel kültürü koruyarak ziyaretçilere kaliteli ve unutulmaz deneyimler sunmak. Her tur yerel rehberlerle planlanır ve sorumlu turizm ilkelerine bağlı kalır.</p>
	</div>
	<div>
	<h3 class="font-semibold">Ekipten Örnekler</h3>
	<div class="mt-2 space-y-3">
		  <div class="p-3 bg-white rounded shadow">
			<p class="font-bold">Meryem Y. — Kurucu & Operasyon</p>
			<p class="text-sm text-slate-600 mt-1">Sektörde 10+ yıl deneyimli; operasyon, kalite ve müşteri deneyimi uzmanı.</p>
		  </div>
		  <div class="p-3 bg-white rounded shadow">
			<p class="font-bold">Ali D. — Tur Koordinatörü</p>
			<p class="text-sm text-slate-600 mt-1">Rota planlama ve yerel rehberlerle koordinasyondan sorumludur.</p>
		  </div>
	</div>
	</div>
	</div>
	<div class="mt-6">
	<h3 class="font-semibold">Müşteri Yorumları</h3>
	<blockquote class="p-4 bg-gray-50 rounded mt-2">"Korgezi ile Kapadokya turu hayatımın en güzel anılarından biri oldu. Rehberimiz çok bilgiliydi." — Ayşe K.</blockquote>
	<blockquote class="p-4 bg-gray-50 rounded mt-2">"Rezervasyon süreci hızlı ve sorunsuzdu. Tavsiye ederim." — Mehmet T.</blockquote>
	</div>
	</div>
</section>

Kabul Kriterleri (Acceptance criteria):
- `#about` bölümü `index.html` içinde tamamen değişmiş veya güncellenmiş olmalı.
- Başlıklar ve paragraflar görüntülenmeli, mobilde düzgün akış sağlamalıdır.
- Ekip kartları aria ve semantik etiketlerle korunmalıdır.

Not: Bu isteği çalıştırmadan önce lütfen mevcut `index.html`'in bir commit ile kaydedildiğinden emin olun; büyük değişiklikleri geri almak daha kolay olur.
Sayfa: Hakkımızda

Kaynak: c:\Users\korha\OneDrive\Masaüstü\5.html

Amaç:
`5.html` içeriğini kullanarak `index.html` için detaylı, profesyonel ve Türkçe bir "Hakkımızda" prompt'u oluşturun. Bu prompt; kısa giriş, misyon, vizyon, ekip tanıtımı, sertifikalar/sürdürülebilirlik ve müşteri yorumlarını kapsamalıdır.

Çıkarılacak Öğeler (attachment'tan):
- Kısa kurumsal giriş paragrafı.
- Misyon ve vizyon metinleri.
- Ekip üyeleri (isim, pozisyon, 1 satırlık bio) — en az 2 örnek.
- Müşteri yorumları (isim, tarih, kısa metin) — en az 2 örnek.

Kabul Kriterleri:
- Metin Türkçe, profesyonel ve akıcı olmalı.
- Bölüm `id="about"` ile işaretlenmiş olmalı.
- Ekip kartlarında görsel varsa `alt` metni olmalı.

Uygulama:
- `index.html` içindeki `about` bölümünü bu prompta göre güncelleyin ve tarayıcıda kontrol edin.

Kurum kimliğinizi, misyonunuzu ve ekibinizi tanıtacak profesyonel bir Hakkımızda bölümü hazırlayın. Kısa giriş, misyon, vizyon, ekip (en az 2 kişi) ve müşteri yorumları (en az 2) içermelidir.

Yapılacaklar:

Kabul Kriterleri:- Kısa giriş paragrafı (1-2 cümle) — marka kimliği ve hedefi vurgulanmalı.

- Metin Türkçe ve kurumsal-profesyonel bir üslupta olmalı.- Misyon ve vizyon başlıkları altında net, kısa cümleler ekleyin.

- Ekip kartlarında isim, pozisyon ve 1 satırlık bio bulunmalı.- Ekipten en az 2 kişi (isim, pozisyon, 1 satırlık bio) gösterin.

- Müşteri yorumları isim + kısa metin + tarih ile sağlanmalı.- Sertifikalar/ortaklıklar hakkında kısa bir ifade ekleyin.

- Bölüm `id="about"` ile işaretlenmiş olmalı.- Sürdürülebilirlik ve yerel topluluk desteği hakkında kısa bir açıklama ekleyin.

- En az iki müşteri yorumu gösterin (isim, tarih, kısa metin).

Kullanım:

`index.html` içindeki `about` bölümünü bu içerikle güncelleyin ve görsel kontrollerini yapın.Ayrıntılar / Kabul Kriterleri:
- Metin Türkçe ve profesyonel bir üslupta olmalı.
- İçerik 6-10 kısa paragrafta ve okunması kolay başlıklar/alt başlıklar ile düzenlenmeli.
- Ekip kartları ve müşteri yorumları `div` ile ayrılmalı; görseller varsa `alt` metinleri olmalı.
- Bölüm sayfa içinde `id="about"` ile işaretlenmiş olmalı.

Kullanım: Bu promptu uyguladıktan sonra ilgili dosyada (ör. `index.html`) bölümü güncelleyin ve tarayıcıda görsel kontrolünü yapın.

---

NOT: Bu dosya resetlendi — lütfen yeni Hakkımızda metinlerini buraya ekleyin.