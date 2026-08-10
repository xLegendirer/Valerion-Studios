# 🔒 VALERION NETWORK — PRIVACY POLICY (GİZLİLİK POLİTİKASI)

**Son Güncelleme:** 10 Ağustos 2026  
**Yürürlük Tarihi:** 10 Ağustos 2026  
**Sürüm:** v2.4.0-PRIV  

---

## 1. GİRİŞ VE VERİ SORUMLUSU
Valerion Network ("Platform"), kullanıcılarımızın kişisel verilerinin ve gizliliğinin korunmasına azami özen göstermektedir. İşbu Gizlilik Politikası, platformumuza bağlı Discord sunucularında ve alt bot servislerimizde (System, Server, Voice, Club, Economy, Fun) toplanan, işlenen ve saklanan verilerin kapsamını ve kullanım amaçlarını açıklamaktadır.

Platform verilerimiz PostgreSQL ilişkisel veritabanı altyapısı üzerinde güvenli ve şifreli bağlantılar ile saklanmaktadır.

---

## 2. TOPLANAN VERİLER VE VERİ KATEGORİLERİ
Valerion Network altyapısı, sistemlerin doğru çalışması ve güvenlik denetimlerinin sağlanması amacıyla yalnızca gerekli minimum verileri toplar:

### 2.1. Kimlik ve Profil Verileri
* **Discord User ID (BIGINT):** Kullanıcıyı platform genelinde benzersiz bir şekilde tanımlamak, yetki seviyelerini (Level 0 - Level 7) belirlemek ve VIP rollerini senkronize etmek için saklanır.
* **Sunucu ve Kanal ID'leri:** Guard log kanallarını, kilit istisnalarını ve dinamik ses odası sahipliklerini eşleştirmek için tutulur.

### 2.2. Etkileşim ve Aktivite Verileri
* **Ses Aktiflik Verileri (`voice_stats`):** Kullanıcıların ses kanallarında geçirdikleri toplam süre (dakika cinsinden), son katılım zamanı ve kazanılan ses seviyeleri saklanır.
* **İhtar ve Ceza Sicili (`user_warns` & `user_notes`):** Sunucu düzenini ihlal eden üyelerin ihtar puanları, otomatik ceza eşikleri ve yetkililer tarafından eklenen iç notlar kaydedilir.
* **Karantina Rol Hafızası (`quarantine_history`):** Karantinaya alınan üyelerin sunucu içi rolleri, karantina kaldırıldığında iade edilmek üzere JSON formatında saklanır.

### 2.3. Finansal ve Envanter Verileri
* **Sanal Ekonomi Kayıtları (`economy`):** Cüzdan bakiyesi, banka hesabı, kredi skorları, vergi borçları ve şirket sahiplik verileri.
* **Dijital Varlık Portföyü (`portfolio` & `vehicles` & `properties`):** Kullanıcının satın aldığı sanal hisse, kripto, araç, emlak ve rozet verileri.

### 2.4. Sistem ve Güvenlik Logları (`system_logs` & `bot_blacklist`)
* Yönetici tarafından yürütülen işlem kayıtları (yetki ekleme, bakım modu değişiklikleri, kara liste işlemleri) ve bunların zaman damgaları (ISO 8601).

---

## 3. VERİLERİN İŞLENME AMAÇLARI VE HUKUKİ SEBEPLERİ
Toplanan veriler aşağıdaki teknik ve operasyonel amaçlar doğrultusunda işlenmektedir:

1. **Hizmetin Sunulması:** VIP statülerinin doğrulanması, sanal bakiye transferlerinin yapılması ve ses odalarının yönetilmesi.
2. **Sunucu Güvenliği (Guard Engine):** Mass-mention, reklam, raid, spam ve izinsiz yetki yükseltme eylemlerinin tespiti ve engellenmesi.
3. **Anlık Senkronizasyon:** PostgreSQL `NOTIFY/LISTEN` mekanizması aracılığıyla kara liste ve bakım modu durumlarının 6 bot arasında canlı olarak güncellenmesi.
4. **İstatistik ve Sıralama:** Ses aktifliği ve sanal bakiye liderlik tablolarının (Top 10) oluşturulması.

---

## 4. VERİLERİN SAKLANMASI VE GÜVENLİĞİ
* **Saklama Süreleri:** Kullanıcı verileri, Kullanıcı sunucuda bulunduğu veya platform servislerini kullandığı sürece saklanır. Kara liste ve ceza sicil kayıtları güvenlik amacıyla kalıcı olarak tutulabilir.
* **Veri Güvenliği Önlemleri:** Veritabanı bağlantıları SSL/TLS protokolleri ile korunmakta olup veritabanı erişimi yetkisiz üçüncü şahıslara kapalıdır. API anahtarları ve tokenlar ortam değişkenleri (`.env`) içerisinde izole edilmiştir.

---

## 5. ÜÇÜNCÜ TARAF SERVİSLER İLE VERİ PAYLAŞIMI
Valerion Network, kullanıcı verilerini hiçbir koşulda üçüncü taraf şirketlere, reklam ağlarına veya pazarlama ajanslarına **satmaz, kiralamaz veya paylaşmaz**.

Ancak altyapı hizmeti aldığımız aşağıdaki teknoloji sağlayıcılarının sunucuları üzerinden teknik veri akışı gerçekleşmektedir:
* **Discord Inc. API:** Bot etkileşimlerinin yürütülmesi.
* **Lavalink / YouTube Uç Noktaları:** Ses ve müzik akışlarının işlenmesi.
* **PostgreSQL / Supabase:** Şifrelenmiş veritabanı barındırma hizmeti.

---

## 6. KULLANICI HAKLARI VE VERİ SİLME TALEPLERİ
Kullanıcılar platformumuz üzerinde aşağıdaki haklara sahiptir:
* **Veri Sorgulama:** `/sistem-araçları araç: ID / Kullanıcı Derin Arama` veya `/finans` komutlarıyla veritabanındaki kayıtlı verilerini inceleme.
* **Veri Silme Talebi (Right to be Forgotten):** Valerion Network üzerindeki tüm verilerinizin silinmesini istiyorsanız, sunucu yönetimi üzerinden veya bot geliştiricisine başvurarak verilerinizin veritabanından tamamen kaldırılmasını talep edebilirsiniz. (Sicil ve kara liste kayıtları güvenlik istisnası kapsamındadır).
