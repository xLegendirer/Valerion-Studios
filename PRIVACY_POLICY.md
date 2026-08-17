# 🔒 VALERION ECOSYSTEM — PRIVACY POLICY (GİZLİLİK POLİTİKASI)

**Doküman Kodu:** `DOC-VAL-PRIV-2026-V7`  
**Son Güncelleme:** 17 Ağustos 2026  
**Yürürlük Tarihi:** 17 Ağustos 2026  
**Sürüm:** v7.0.0-ENTERPRISE  

---

## 1. GİRİŞ VE VERİ SORUMLUSU
Valerion Ecosystem ("Platform"), kullanıcılarımızın kişisel verilerinin ve gizliliğinin korunmasına azami özen göstermektedir. İşbu Gizlilik Politikası, platformumuza bağlı Discord sunucularında, alt bot servislerimizde (Valerion Link, System, Server, Voice, Club, Economy, Fun) ve entegre Web Kontrol Panelimizde (`dashboard.html` / `manage.html`) toplanan, işlenen ve saklanan verilerin kapsamını ve kullanım amaçlarını açıklamaktadır[cite: 1].

Platform verilerimiz PostgreSQL ilişkisel veritabanı altyapısı üzerinde güvenli ve SSL/TLS şifreli bağlantılar ile saklanmaktadır[cite: 1].

---

## 2. TOPLANAN VERİLER VE VERİ KATEGORİLERİ
Valerion Ecosystem altyapısı, sistemlerin doğru çalışması, rütbe ve rol eşitlemelerinin yapılması ve güvenlik denetimlerinin sağlanması amacıyla yalnızca gerekli minimum verileri toplar[cite: 1]:

### 2.1. Discord Kimlik ve Profil Verileri
* **Discord User ID (BIGINT):** Kullanıcıyı platform genelinde benzersiz bir şekilde tanımlamak, yetki seviyelerini (Level 0 - Level 7) belirlemek, VIP rollerini ve web oturumlarını yönetmek için saklanır[cite: 1].
* **Sunucu, Rol ve Kanal ID'leri:** Guard log kanallarını, kilit istisnalarını, dinamik ses odası sahipliklerini, rank bind rol eşleşmelerini ve audit log kanallarını haritalandırmak için tutulur[cite: 1].

### 2.2. Roblox Entegrasyon ve Doğrulama Verileri (`roblox_accounts` & `link_role_binds`)
* **Roblox User ID & Kullanıcı Adı:** Kullanıcının Discord hesabıyla eşleştirdiği Roblox kimliklerini saklamak için tutulur[cite: 1].
* **Doğrulama Metodu (`OAuth2` / `Bio`):** Hesabın hangi güvenli protokol ile doğrulandığı bilgisi[cite: 1].
* **Aktif Hesap Durumu (`is_primary`):** Kullanıcının çoklu hesap mimarisinde rol ve isim senkronizasyonu için aktif olarak seçtiği hesabı belirtir[cite: 1].
* **Roblox Grup ve Rütbe Bilgileri:** Açık Roblox API'leri üzerinden anlık olarak çekilen grup kimlikleri ve sayısal rütbe değerleri (1-255)[cite: 1].
* *Önemli Not:* Discord veya Roblox hesap şifreleriniz **asla talep edilmez, kaydedilmez ve saklanmaz**. Kimlik doğrulamaları resmi OAuth2 protokolü üzerinden geçici yetkilendirme jetonları ile yürütülür[cite: 1].

### 2.3. Etkileşim, Güvenlik ve Aktivite Verileri
* **Ses Aktiflik Verileri (`voice_stats`):** Kullanıcıların dinamik ve genel ses kanallarında geçirdikleri toplam süre (dakika cinsinden), son katılım zamanı ve kazanılan ses deneyim seviyeleri[cite: 1].
* **İhtar ve Ceza Sicili (`user_warns` & `user_notes`):** Sunucu düzenini ihlal eden üyelerin ihtar puanları, otomatik ceza eşikleri ve yetkililer tarafından eklenen iç notlar[cite: 1].
* **Karantina Rol Hafızası (`quarantine_history`):** Karantinaya alınan üyelerin sunucu içi rolleri, karantina kaldırıldığında iade edilmek üzere JSON formatında saklanır[cite: 1].

### 2.4. Finansal ve Envanter Verileri
* **Sanal Ekonomi Kayıtları (`economy`):** Cüzdan bakiyesi, banka hesabı, kredi skorları, vergi borçları ve şirket sahiplik verileri[cite: 1].
* **Dijital Varlık Portföyü (`portfolio`, `vehicles` & `properties`):** Kullanıcının satın aldığı sanal hisse, kripto, araç, gayrimenkul ve rozet verileri[cite: 1].

### 2.5. Sistem, Web Oturum ve Güvenlik Logları (`system_logs` & `bot_blacklist`)
* Web paneli oturum kimlikleri (7 günlük HttpOnly çerezler), yönetici tarafından yürütülen işlem kayıtları (yetki ekleme, bakım modu değişiklikleri, kara liste işlemleri) ve bunların zaman damgaları (ISO 8601)[cite: 1].

---

## 3. VERİLERİN İŞLENME AMAÇLARI VE HUKUKİ SEBEPLERİ
Toplanan veriler aşağıdaki teknik ve operasyonel amaçlar doğrultusunda işlenmektedir[cite: 1]:

1. **Hizmetin Sunulması & Senkronizasyon:** Roblox grup rütbelerine göre Discord rollerinin otomatik dağıtılması, takma adların şablonlara göre formatlanması, VIP statülerinin doğrulanması ve ses odalarının yönetilmesi[cite: 1].
2. **Sunucu Güvenliği (Guard Engine):** Mass-mention, reklam, raid, spam, izinsiz bot/webhook oluşturma ve yetkisiz rol/kanal manipülasyonlarının engellenmesi[cite: 1].
3. **Yasaklı Hesap Koruması:** Roblox üzerinde yasaklanmış (`isBanned: true`) hesapların tespit edilerek sunucu güvenliğini tehdit etmesinin önlenmesi[cite: 1].
4. **Anlık Dağıtık Senkronizasyon:** PostgreSQL `NOTIFY/LISTEN` mekanizması aracılığıyla kara liste, önbellek ve bakım modu durumlarının 7 bot ve web servisi arasında canlı (0ms gecikme ile) güncellenmesi[cite: 1].
5. **İstatistik ve Sıralama:** Ses aktifliği ve sanal ekonomi liderlik tablolarının (Top 10) oluşturulması[cite: 1].

---

## 4. VERİLERİN SAKLANMASI VE GÜVENLİĞİ
* **Saklama Süreleri:** Kullanıcı verileri, kullanıcı sunucuda bulunduğu veya platform servislerini kullandığı sürece saklanır. Kara liste, güvenlik denetimi ve ceza sicil kayıtları ekosistem güvenliği amacıyla kalıcı olarak tutulabilir[cite: 1].
* **Veri Güvenliği Önlemleri:** Veritabanı bağlantıları SSL/TLS protokolleri ile korunmakta olup yetkisiz üçüncü şahısların erişimine kapalıdır. API anahtarları, gizli anahtarlar (`CLIENT_SECRET`) ve bot tokenları ortam değişkenleri (`.env`) içerisinde izole edilmiştir[cite: 1].

---

## 5. ÜÇÜNCÜ TARAF SERVİSLER İLE VERİ PAYLAŞIMI
Valerion Ecosystem, kullanıcı verilerini hiçbir koşulda üçüncü taraf şirketlere, veri simsarlarına, reklam ağlarına veya pazarlama ajanslarına **satmaz, kiralamaz veya paylaşmaz**[cite: 1].

Teknik altyapının sürdürülebilmesi adına yalnızca aşağıdaki resmi teknoloji sağlayıcılarının uç noktaları ile güvenli veri iletişimi gerçekleştirilir[cite: 1]:
* **Discord Inc. API & OAuth2:** Bot etkileşimleri, yetkilendirmeler ve sunucu olaylarının yürütülmesi[cite: 1].
* **Roblox Open Cloud & Users API:** Kimlik doğrulama, avatar görselleri ve grup rütbe verilerinin sorgulanması[cite: 1].
* **PostgreSQL / Render / Supabase:** Şifrelenmiş veritabanı ve web servis barındırma altyapısı[cite: 1].
* **Lavalink Uç Noktaları:** Ses akışlarının işlenmesi[cite: 1].

---

## 6. KULLANICI HAKLARI VE VERİ SİLME TALEPLERİ
Kullanıcılar platformumuz üzerinde aşağıdaki haklara sahiptir[cite: 1]:
* **Veri Sorgulama:** `/roblox-profil`, `/roblox-hesaplarim`, `/sistem-araçları` veya `/finans` komutlarıyla veritabanında kayıtlı verilerini inceleme[cite: 1].
* **Roblox Bağlantısını Kaldırma:** Discord üzerinden `/unlink` komutunu kullanarak veya Web Kontrol Paneli (`dashboard.html`) üzerinden tek tıkla bağlı tüm Roblox kimliklerini ve veritabanı kayıtlarını anında silme[cite: 1].
* **Veri Silme Talebi (Unutulma Hakkı):** Valerion Ecosystem üzerindeki tüm profil verilerinizin kalıcı olarak silinmesini istiyorsanız, sunucu yönetimi veya bot geliştiricisi ile iletişime geçerek verilerinizin veritabanından tamamen kaldırılmasını talep edebilirsiniz (kara liste ve güvenlik sicil kayıtları güvenlik istisnası kapsamındadır)[cite: 1].

---

## 7. İLETİŞİM VE DESTEK
Gizlilik Politikası veya kişisel verilerinizin işlenmesiyle ilgili soru, görüş ve talepleriniz için resmi Discord sunucumuz üzerinden destek kanallarından geliştirici ekibimize ulaşabilirsiniz[cite: 1].
