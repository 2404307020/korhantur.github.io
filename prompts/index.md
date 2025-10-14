# prompts/index.md

Amaç: Repo kökündeki `index.html` dosyasını güncellemek veya buradan yapılandırılmış içerik çıkarmak için kullanılacak Copilot prompt'u ve kuralları.

Kullanım talimatı (özet):
- Bu dosyayı Copilot'a verin ve hangi bölümü değiştirmek istediğinizi açıkça belirtin (örn. `#about`, `#tours`, `#reservation`).
- İstediğiniz değişikliği kısa ve net bir cümleyle ifade edin. Örnek: "Sadece #about bölümünü verilen About metniyle değiştir." veya "#gallery bölümüne 3 yeni resim ekle ve her birine uygun alt metin ver." 

Çıkarma / Güncelleme Kuralları (zorunlu):
1. Başlıklar: H1/H2/H3 içerikleri korunacak veya açıkça değiştirilecekse yeni içerik verilecektir.
2. Paragraflar: Uzun paragrafları 2-3 kısa cümleye indirgeyin; resmi veya vurgu gerekiyorsa belirtin.
3. Görseller: Her görsel için tam URL ve kısa `alt` metni verin. (Örn: `https://.../img1.jpg | alt: "Kapadokya balon turu"`)
4. Formlar: `name` ve `type` alanları korunacak; ekstra doğrulama gerektiğinde belirtin.

Stil ve Erişilebilirlik Kuralları:
- Tüm görsellerde `alt` olmalı.
- Form alanlarına `aria-label` veya görünür `label` ekleyin.
- CTA butonları (Rezervasyon, Detaylar) kontrastlı ve erişilebilir olmalı.

Örnek kısa prompt'lar (kopyala-yapıştır):

1) About bölümünü güncelle:

```text
prompts/index.md kullan: "Sadece #about bölümünü şu metinle değiştir: \nKorgezi, Türkiye'nin benzersiz kültür ve doğasını deneyimleten turlar sunar. Misyonumuz sürdürülebilir ve güvenli seyahatler sağlamaktır."
```

2) Gallery'ye resim ekle:

```text
prompts/index.md kullan: "#gallery bölümüne 3 resim ekle. Her resim için URL ve 5-7 kelimelik alt metin ver: \n1) https://example.com/img1.jpg | alt: 'Pamukkale travertenleri' \n2) https://example.com/img2.jpg | alt: 'Kapadokya balonlar' \n3) https://example.com/img3.jpg | alt: 'Ege sahil gün batımı'"
```

3) Rezervasyon formunu doğrula:

```text
prompts/index.md kullan: "Rezervasyon formunu required alanlarla (fullname, email, tour, date) bırak; email için HTML5 doğrulaması ekle ve gönder düğmesini 'Gönder' olarak değiştir." 
```

NOT: Her istekte yalnızca bir bölüm güncelleyin. Büyük değişiklikler için önce bir commit alınız.
