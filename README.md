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


## Ekran görüntüleri

<table>
  <tr>
    <td align="center"><a href="screenshots/02-urunler-mobil.png"><img src="screenshots/02-urunler-mobil.png" width="260"></a><br><sub>urunler mobil</sub></td>
    <td align="center"><a href="screenshots/02-urunler.png"><img src="screenshots/02-urunler.png" width="260"></a><br><sub>urunler</sub></td>
    <td align="center"><a href="screenshots/02b-urun-listesi-mobil.png"><img src="screenshots/02b-urun-listesi-mobil.png" width="260"></a><br><sub>urun listesi mobil</sub></td>
  </tr>
  <tr>
    <td align="center"><a href="screenshots/02b-urun-listesi.png"><img src="screenshots/02b-urun-listesi.png" width="260"></a><br><sub>urun listesi</sub></td>
    <td align="center"><a href="screenshots/03-urun-detay-mobil.png"><img src="screenshots/03-urun-detay-mobil.png" width="260"></a><br><sub>urun detay mobil</sub></td>
    <td align="center"><a href="screenshots/03-urun-detay.png"><img src="screenshots/03-urun-detay.png" width="260"></a><br><sub>urun detay</sub></td>
  </tr>
  <tr>
    <td align="center"><a href="screenshots/04-sepet-mobil.png"><img src="screenshots/04-sepet-mobil.png" width="260"></a><br><sub>sepet mobil</sub></td>
    <td align="center"><a href="screenshots/04-sepet.png"><img src="screenshots/04-sepet.png" width="260"></a><br><sub>sepet</sub></td>
    <td align="center"><a href="screenshots/05-odeme.png"><img src="screenshots/05-odeme.png" width="260"></a><br><sub>odeme</sub></td>
  </tr>
  <tr>
    <td align="center"><a href="screenshots/06-siparislerim.png"><img src="screenshots/06-siparislerim.png" width="260"></a><br><sub>siparislerim</sub></td>
    <td align="center"><a href="screenshots/07-giris.png"><img src="screenshots/07-giris.png" width="260"></a><br><sub>giris</sub></td>
    <td align="center"><a href="screenshots/08-kayit.png"><img src="screenshots/08-kayit.png" width="260"></a><br><sub>kayit</sub></td>
  </tr>
  <tr>
    <td align="center"><a href="screenshots/09-siparis-takip.png"><img src="screenshots/09-siparis-takip.png" width="260"></a><br><sub>siparis takip</sub></td>
    <td align="center"><a href="screenshots/10-admin-siparisler.png"><img src="screenshots/10-admin-siparisler.png" width="260"></a><br><sub>admin siparisler</sub></td>
    <td align="center"><a href="screenshots/11-admin-urunler.png"><img src="screenshots/11-admin-urunler.png" width="260"></a><br><sub>admin urunler</sub></td>
  </tr>
  <tr>
    <td align="center"><a href="screenshots/12-admin-kullanicilar.png"><img src="screenshots/12-admin-kullanicilar.png" width="260"></a><br><sub>admin kullanicilar</sub></td>
    <td align="center"><a href="screenshots/13-admin-yorumlar.png"><img src="screenshots/13-admin-yorumlar.png" width="260"></a><br><sub>admin yorumlar</sub></td>
    <td align="center"><a href="screenshots/14-admin-kategoriler.png"><img src="screenshots/14-admin-kategoriler.png" width="260"></a><br><sub>admin kategoriler</sub></td>
  </tr>
</table>
