# Efe Oto Servis

Mobil uyumlu, bağımsız HTML/CSS/JavaScript ön konsept.

## İşletme bilgileri
`dist/config.js` içindeki `whatsappNumber` alanına ülke kodu dahil yalnızca rakamlardan oluşan gerçek numarayı ekleyin. `phoneDisplay`, `address`, `hours` isteğe bağlıdır. Gerçek numara girildiğinde randevu mesajının WhatsApp bağlantısı ve iletişim alanı etkinleşir. Numara yoksa mesaj hazırlanabilir ve kopyalanabilir; gönderim taklit edilmez.

## İçerik
Hizmetler kullanıcı briefi doğrultusunda örnek içeriktir; işletmeyle doğrulanmalıdır. Galeri ve atölye görselleri yapay zekâ ile üretilmiş temsili görsellerdir. Gerçek tamamlanmış iş kayıtları sağlanmadı. Site bunları açıkça örnek olarak etiketler.

Castrol SVG: https://www.castrol.com/apps/settings/wcm/designs/refresh/castrol/images/reignite/logo.svg
Shell SVG: https://www.shell.com/etc.clientlibs/amidala/clientlibs/theme-base/resources/favicon/favicon.svg
Logolar ürün markalarını belirtir; yetkili servis/ortaklık iddiası içermez.

## Randevu
Form alanları istemcide doğrulanır. Tarih bir tercihtir; müsaitlik veya rezervasyon garantisi yoktur. Randevu servis ekibinin WhatsApp yanıtıyla teyit edilir. Veriler sitede saklanmaz. WhatsApp bağlantısını ziyaretçi kendisi açıp gönderir.

## Sunum
`dist` klasörünü statik sunucuyla servis edin. Sunucu tarafı bağımlılık, üyelik veya veritabanı yoktur.
