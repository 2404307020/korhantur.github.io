Sayfa: Rezervasyon

Kaynak: c:\Users\korha\OneDrive\Masaüstü\3.html

Amaç:
`3.html`'teki "Reservation Request" formunun örneğini kullanarak, `index.html` için erişilebilir ve doğrulanabilir bir rezervasyon formu prompt'u hazırlayın.

Çıkarılacak Öğeler (attachment'tan):
- Form alanları listesi (fullname, email, tour select, date, notes) ve placeholder metinleri.
- Gönder butonu metni (Submit Request).

Kabul Kriterleri:
- Tüm inputlar `name` ve uygun `type` ile verilmiş olmalı (örn. `type="email"`, `type="date"`).
- Gerekli alanlarda `required` kullanılmalı.
- Form `action="#"` veya basit JS handler ile demo çalışmalı.
- Başarılı/başarısız durumda kullanıcıya mesaj gösterilmeli.

Uygulama:
- `index.html` içinde `id="reservation"` bölümünü bu formla doldurun ve birkaç demo gönderim test edin.
Kullanıcıların tur rezervasyonu taleplerini kolayca gönderebilecekleri, erişilebilir bir form oluşturun. Form alanları: tam ad (`name="fullname"`), e-posta (`type="email"`), seçilen tur (`name="tour"`), katılım tarihi (`type="date"`), ve ek notlar (`textarea`).

Kabul Kriterleri:
- Tüm alanlar uygun `name` ve `type` ile tanımlanmalı; zorunlu alanlar `required` olmalı.
- E-posta alanı `type="email"` ve temel HTML doğrulaması yapılmalı.
- Form gönderimi demo amaçlı `action="#"` veya JS ile yerel olarak işlenecek şekilde ayarlanmalı.
- Başarılı/başarısız gönderim için kullanıcıya görsel geri bildirim gösterin.

Kullanım:
Formu `id="reservation"` bölümüne yerleştirin, test için birkaç örnek gönderim yapın.