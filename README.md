# Bal E-Ticaret

**Bal ve arı ürünleri satışı için uçtan uca e-ticaret sitesi.** Üyelikten siparişe, stok takibinden e-posta bildirimlerine kadar tüm akış yayına hazır hale getirildi.

> Kaynak kod private. Bu depo projenin tanıtım sayfasıdır. İstek üzerine demo yapılabilir.

## Özellikler

**Mağaza**
- Ürün listeleme, ürün detayı, sepet, sipariş
- Üyelik, e-posta doğrulama, profil
- İl/ilçe seçimli adres formu
- KVKK gizlilik politikası, iade/iptal ve iletişim sayfaları
- SEO: `sitemap.xml`, `robots.txt`

**Yönetim paneli**
- 2FA'lı admin girişi
- Ürün, sipariş, kullanıcı ve yorum yönetimi

**Backend**
- MongoDB transaction ile atomik stok düşümü ve yarış durumu koruması
- Stok azalınca uyarı
- Sipariş onayı, admin bildirimi ve hoş geldin e-postaları (HTML şablonlar, işlemi bekletmeden gönderim)
- Winston ile loglama (dosya rotasyonlu), merkezi hata yakalama

**Güvenlik**
- JWT, bcrypt, Helmet
- Rate limiting (API, giriş, hesap oluşturma için ayrı limitler)
- Tüm uç noktalarda girdi doğrulama, NoSQL injection koruması
- Origin kontrollü CORS, ortam değişkeniyle merkezi yapılandırma

## Teknolojiler

Node.js · Express · MongoDB / Mongoose · JWT · bcrypt · Helmet · express-rate-limit · express-validator · express-mongo-sanitize · Nodemailer · Winston · HTML/CSS/JavaScript

<!-- Ekran görüntüleri: screenshots/ klasörüne ekleyip aşağıdaki satırları açın
![Ana sayfa](screenshots/home.png)
-->
