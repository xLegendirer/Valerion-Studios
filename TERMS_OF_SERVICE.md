# 💎 VALERION ECOSYSTEM — COMPREHENSIVE ENTERPRISE TERMS OF SERVICE
### (GENEL HİZMET KULLANIM, MİMARİ VE HUKUKİ ŞARTLAR SÖZLEŞMESİ)

**Doküman Kodu:** `DOC-VAL-TOS-2026-V7`  
**Sürüm:** `v7.0.0-ENTERPRISE-FULL`  
**Yürürlük Tarihi:** 17 Ağustos 2026  
**Son Güncelleme:** 17 Ağustos 2026  
**Hukuki Dayanak:** T.K.K.K. (6698 Sayılı KVKK), AB Genel Veri Koruma Yönetmeliği (GDPR - EU 2016/679), Discord Developer Terms of Service and Developer Policy, Roblox Terms of Use & Open Cloud API Policies, US Fair Credit Reporting Act (Analogous Virtual Terms).

---

## 1. GİRİŞ, TARAFLAR VE ANLAŞMANIN AKDİ

### 1.1. Sözleşmenin Tarafları
İşbu Hizmet Kullanım Sözleşmesi ("Sözleşme" veya "TOS"), **Valerion Studios / Valerion Network** ("Şirket", "Platform", "Biz", "Altyapı", "Sistem") ile Valerion Ekosistemi bünyesindeki Discord sunucularına katılan, altyapıda barındırılan bot servislerini kullanan, entegre Web Kontrol Panelini (`dashboard.html` / `manage.html`) ziyaret eden, komut çalıştıran veya bu altyapıyla dolaylı/doğrudan etkileşime giren tüm gerçek ve tüzel kişiler ("Kullanıcı", "Üye", "Siz", "Son Kullanıcı") arasında hukuki olarak bağlayıcı bir şekilde akdedilmiştir.

### 1.2. Hukuki Onay, Tek Komut Onayı ve Otomatik Kabul
* **1.2.1. İncelenmişlik Beyanı:** Valerion Ecosystem platformuna erişim sağlayarak, sunuculara katılarak, web paneline giriş yaparak veya altyapıda barındırılan 7 bottan herhangi birini etkileşime sokarak işbu Sözleşme'nin tüm maddelerini kabul etmiş sayılırsınız.
* **1.2.2. Tek Komut / Etkileşim İle Onay (Single-Command Consent):** Valerion Ekosistemi bünyesindeki herhangi bir bot üzerinde **TEK BİR SLASH (`/`) VEYA PREFİKS (`!`) KOMUTUNUN ÇALIŞTIRILMASI, SES KANALLARINA GİRİŞ YAPILMASI, ROBLOX HESAP BAĞLAMA İŞLEMİNİN (`/link`) GERÇEKLEŞTİRİLMESİ VEYA BUTON/MENÜ ETKİLEŞİMİNDE BULUNULMASI**, kullanıcının işbu Hizmet Şartları'nı, Gizlilik Politikasını, Topluluk Kurallarını ve Guard Güvenlik Politikası'nı tamamen okuduğu, anladığı ve **KOŞULSUZ OLARAK KABUL ETTİĞİ** anlamına gelir.
* **1.2.3. Onayın Bağlayıcılığı:** "Okumadım", "Görmedim" veya "Haberim Yoktu" beyanları hukuki geçersizlik teşkil etmez; ilk komut veya web paneli oturum açma eylemiyle birlikte onay veritabanı zaman damgaları (ISO 8601) ile eşleşerek bağlayıcı hale gelir.

### 1.3. Şartların Reddi Halinde Prosedür
İşbu Sözleşme'de yer alan şartlardan herhangi birini kabul etmiyorsanız, Valerion Ecosystem altyapısına bağlı tüm servislerin ve web panellerinin kullanımına derhal son vermeli, etkileşimli bot komutlarını çalıştırmayı bırakmalı ve bağlı bulunduğunuz topluluk sunucularından ayrılmalısınız.

---

## 2. SÖZLEŞMESEL TANIMLAR VE KAVRAMLAR

İşbu Sözleşme içerisinde yer alan terimler aksi açıkça belirtilmedikçe aşağıdaki anlamları ifade eder:
* **Ekosistem / Ağ:** Valerion Network bünyesindeki Web Kontrol Paneli, PostgreSQL veritabanı sunucuları ve 7 adet senkronize mikroservis botu (Valerion Link, System, Server, Voice, Club, Economy, Fun).
* **Sanal Varlık:** Ekosistem içerisinde kazanılan, satın alınan veya transfer edilen Coin, Mülk, Araç, Hisse, Kripto Para, Rozet ve VIP statüleri.
* **Global Blacklist (Ağ Kara Listesi):** Ekosisteme bağlı tüm botlarda ve web servislerinde geçerli olan, kullanıcının komut çalıştırma, web paneline erişim ve hesap bağlama haklarının sistem seviyesinde kalıcı olarak engellenmesi.
* **Bot Sahibi / Developer:** Altyapının tüm telif, kod ve mülkiyet haklarına sahip olan `VALERION` (ID: `832617684285915226`) yetkili hesabı.
* **Guard Motoru:** Sunucu güvenliğini, izinsiz eylemleri, spam, raid girişimlerini ve Roblox hesap güvenlik açıklarını denetleyen otomatik koruma yazılımı.

---

## 3. DAĞITIK MİKROSERVİS MİMARİSİ VE SERVİS KAPSAMI

Valerion Ecosystem, Discord Inc. ve Roblox Open Cloud API'leri üzerine inşa edilmiş, kendi aralarında senkronize çalışan dağıtık bir platformdur. Platform hizmetleri aşağıdaki 7 ana servis biriminin entegre çalışmasıyla sunulmaktadır:

* **3.1. Valerion Link Bot (`DISCORD_TOKEN_LINK`):** Roblox OAuth2 ve Bio doğrulama altyapısı, çoklu hesap yönetimi (`roblox_accounts`), dinamik rütbe ve rol eşleme (`link_role_binds`), otomatik takma ad formatlama ve web yönetim paneli entegrasyonu.
* **3.2. Valerion System Bot (`DISCORD_TOKEN_SYSTEM`):** Otorite hiyerarşisi (Level 0 ile Level 7 arası), VIP tanımlama/silme, OwO otomatik ödeme yakalama motoru, kullanıcı sicil kartları, loglama ve küresel bakım ayarlarını yöneten ana konsol.
* **3.3. Valerion Server Guard Bot (`DISCORD_TOKEN_SERVER`):** Enterprise düzeyde sunucu koruma duvarı, anti-raid, anti-spam, mass-mention engeli, izinsiz yetki yükseltme koruması, karantina yönetimi, tuzak kanal algılayıcı ve otomatik ihtar (warn) motoru.
* **3.4. Valerion Voice Bot (`DISCORD_TOKEN_VOICE`):** Ses aktiflik ve süre takibi, dinamik oda oluşturucu (`🔊 Lounge`), oda sahipliği kontrol panelleri ve yerel Lavalink / Wavelink yüksek kaliteli ses akış motoru.
* **3.5. Valerion Club Bot (`DISCORD_TOKEN_CLUB`):** VIP Lounge etkileşimleri, C-SUB abonelik hediye mekanizması, rozet vitrini, prestij düelloları ve elit topluluk ayrıcalıkları.
* **3.6. Valerion Economy Bot (`DISCORD_TOKEN_ECONOMY`):** Merkez bankacılığı, sanal borsa, gayrimenkul ve garaj yönetimi, şirket simülasyonu, vergi/hukuk sistemleri, karaborsa ve şans oyunları (Casino Engine).
* **3.7. Valerion Fun Bot (`DISCORD_TOKEN_FUN`):** Sosyal etkileşim araçları, mini oyunlar, anime/manga entegrasyonu, AFK modları ve topluluk mizah panelleri.

---

## 4. VERİTABANI SENKRONİZASYON VE SİNYALİZASYON PROTOKOLÜ (NOTIFY/LISTEN)

Platform servisleri, PostgreSQL ilişkisel veritabanı altyapısı üzerinde çalışan anlık sinyal dinleyicileri (`NOTIFY / LISTEN`) ile birbirine bağlıdır. Web paneli veya botlar üzerinden yapılan bir ayar değişikliği, rol bind güncellemesi veya kara liste ekleme işlemi veritabanında gerçekleştikten mikro saniyeler sonra sinyalizasyon hattı üzerinden diğer tüm botların RAM belleklerine (Cache) yansıtılır.

---

## 5. KULLANICI HESAPLARI, ROBLOX ENTEGRASYONU VE YAŞ SINIRI

### 5.1. Discord ve Roblox Hesap Eşleşmesi
Tüm hizmetler kullanıcıların benzersiz Discord Hesap ID'leri (`BIGINT`) ve Valerion Link üzerinden doğrulanan Roblox kimlikleri (`roblox_id`) üzerinden yürütülür. Hesabınız üzerinden gerçekleştirilen tüm işlemlerden doğrudan hesap sahibi sorumludur.

### 5.2. Yaş Kısıtlaması ve Dijital Rıza
Kullanıcılar, Discord ve Roblox platformlarının hizmet şartları uyarınca en az 13 yaşında olduklarını beyan ederler. 13 yaşın altında olduğu tespit edilen kullanıcıların hesapları Ağ Kara Listesine alınarak servis erişimleri engellenir.

---

## 6. SİSTEM GÜVENLİĞİ, YASAKLI EYLEMLER VE KÖTÜYE KULLANIM

Valerion Ecosystem altyapısının kararlılığını ve güvenliğini korumak amacıyla bot yazılımlarını sabote etmek, sanal ekonomide haksız avantaj sağlamak, Roblox OAuth2 altyapısını kötüye kullanmak veya sunucu huzurunu bozmak kesinlikle yasaktır.

---

## 7. YAZILIM AÇIKLARI VE EXPLOIT SUİSTİMALİ PROSEDÜRÜ

Bot kodlarında, OAuth2 akışlarında veya veritabanı senkronizasyonlarında tespit edilen mantık hatalarını (bug) kişisel çıkar veya haksız bakiye/yetki sağlama amacıyla kullanmak yasaktır. Tespit edilen açıklar derhal geliştiricilere bildirilmelidir.

---

## 8. OTOMASYON, MAKRO VE SELF-BOT KULLANIM YASAĞI

Slash komutlarını otomatik yürütmek, sanal ekonomide haksız kazanç sağlamak veya OAuth2 süreçlerini manipüle etmek amacıyla makro, yazılım, script veya Discord Self-Bot istemcileri kullanmak yasaktır.

---

## 9. AĞ VE SUNUCU SALDIRILARI (DoS/DDoS/SPAM) KORUMASI

Bot istemcilerine, Lavalink ses sunucularına veya veritabanı uç noktalarına yönelik aşırı yükleme yapacak komut spam'leri, DoS/DDoS girişimleri veya API suistimalleri yasal işlem sebebidir.

---

## 10. KÜRESEL AĞ YAPTIRIMLARI VE GLOBAL BLACKLIST (AĞ KARA LİSTESİ)

Kural ihlali gerçekleştiren, sistem açıklarını kullanan veya ağır topluluk ihlali yapan kullanıcılar herhangi bir ihbarda bulunulmaksızın **Valerion Ecosystem bünyesindeki 7 botun tamamından ve Web Kontrol Panelinden (Global Blacklist)** kalıcı olarak yasaklanır; tüm sanal varlıkları ve VIP hakları feshedilir.

---

## 11. SANAL EKONOMİ, FİNANSAL KOŞULLAR VE MÜLKİYET REJİMİ

Valerion Economy, Club ve System botlarında yer alan "Coin", "Banka Bakiyesi", "Hisse", "Gayrimenkul" veya "VIP Üyelikler" tamamen sanal simülasyon öğeleridir; **gerçek para karşılığına, nakdi değere veya yasal mülkiyet hakkına sahip değildir** ve hiçbir koşulda nakite dönüştürülemez.

---

## 12. TİCARET YASAĞI (REAL MONEY TRADING - RMT)

Sistem içi sanal varlıkların veya VIP hesapların gerçek para karşılığında (RMT) satılması veya takas edilmesi yasaktır; tespiti halinde tarafların tüm varlıkları sıfırlanır ve Global Blacklist uygulanır.

---

## 13. VIP ÜYELİKLER VE HİYERARŞİ

Platform üzerinde sunulan VIP statüleri hiyerarşik olup Level 1 (VIP) ile Level 7 (VALERION) arasında değişen yetki seviyelerine dayanır.

---

## 14. OWO OTOMATİK ÖDEME VE ROBLOX OAUTH2 DOĞRULAMA SİSTEMİ

OwO ödemeleri veya Valerion Link OAuth2 süreçleri, platformun otomatik doğrulama motorları tarafından onaylanarak anında veritabanına işlenen dijital hizmetler kapsamındadır.

---

## 15. KESİN İADE MÜMKÜNSÜZLÜĞÜ POLİTİKASI (NO-REFUND POLICY)

Satın alınan tüm VIP paketleri, dijital kartlar ve C-SUB hakları hesabınıza tanımlandığı andan itibaren **iade edilemez, iptal edilemez ve bakiye olarak geri istenemez**. Ceza alan kullanıcıların VIP süreleri iade edilmez.

---

## 16. C-SUB ABONELİK HEDİYE MEKANİZMASI

`CVIP` seviyesindeki üyelere tanınan C-SUB hediye etme hakkı kişiye özeldir. Hediye edilen kullanıcının kuralları ihlal etmesi durumunda abonelik iptal edilebilir.

---

## 17. GUARD MİMARİSİ VE OTOMATİK İHTAR (WARN) MOTORU

Server Guard botu, kural ihlali yapan kullanıcılara otomatik ihtar puanı ekler (`user_warns`). 3 ihtar puanında Timeout, 5 ihtar puanında Rol Hafızalı Karantina, 7 ihtar puanında ise Otomatik Sunucu Banı uygulanır.

---

## 18. OTOMATİK TUZAK KANALLAR (TRAP CHANNELS)

Tuzak kanallara yazılan her türlü mesaj, hesabın otomatik spam/self-bot olduğu kabul edilerek mesaj anında silinir ve hesap otomatik olarak banlanır.

---

## 19. ANTI-NUKE VE YETKİ YÜKSELTME KORUMASI

Whitelist içinde bulunmayan bir yetkilinin izinsiz `Administrator` vermeye çalışması Guard tarafından engellenir; işlem geri alınır ve yetkiyi verenin rolleri sıfırlanır.

---

## 20. SES KANALLARI VE DİNAMİK ODA YÖNETİMİ

Dinamik ses kanallarında oda sahipliği odayı oluşturan kişiye aittir; oda isimlerinde ve yayınlarda topluluk kurallarına uyulması zorunludur.

---

## 21. FİKRİ MÜLKİYET VE KOD KORUMA REJİMİ

Valerion Ecosystem altyapısına ait tüm yazılım kaynak kodları, C++, Python bot modülleri, PostgreSQL şemaları, web paneli arayüz tasarımları ve ticari unvanlar **Valerion Studios**'a aittir; izinsiz kopyalanamaz ve tersine mühendisliğe tabi tutulamaz.

---

## 22. HİZMET SEVİYESİ TAAHHÜDÜ (SLA) VE GARANTİ REDDİ

Valerion Ecosystem, hizmetlerin %100 kesintisiz, hatasız veya siber saldırılardan tamamen muaf olacağını garanti etmez; hizmetler "OLDUĞU GİBİ" (AS IS) sunulur.

---

## 23. SORUMLULUK SINIRLAMASI (LIMITATION OF LIABILITY)

Discord/Roblox API güncellemeleri, küresel internet arızaları, Render/Hosting altyapı problemleri veya veritabanı bakımları nedeniyle yaşanabilecek veri kayıplarından Şirketimiz sorumlu tutulamaz.

---

## 24. VERİ GİZLİLİĞİ VE GÜVENLİĞİ

Kullanıcı verileri, platformun `PRIVACY_POLICY.md` dokümanında belirtilen esaslara uygun olarak SSL/TLS şifreli PostgreSQL altyapısında saklanır ve işlenir.

---

## 25. MÜCBİR SEBEPLER (FORCE MAJEURE)

Siber saldırılar, Discord veya Roblox API'lerinin tamamen erişime kapanması, altyapı çöküntüleri, doğal afetler veya yasal düzenlemeler mücbir sebep sayılır.

---

## 26. SÖZLEŞMENİN DEĞİŞTİRİLMESİ VE GÜNCELLENMELER

Valerion Ecosystem, işbu Sözleşme şartlarını dilediği zaman güncelleme hakkını saklı tutar. Güncellenmiş koşullar yayınlandığı andan itibaren geçerlidir.

---

## 27. FESİH VE BÖLÜNEBİLİRLİK

Sözleşme'nin herhangi bir maddesinin geçersiz sayılması diğer maddelerin geçerliliğini etkilemez.

---

## 28. UYGULANACAK HUKUK VE YETKİLİ YARGI

İşbu Sözleşme'nin uygulanmasında Türkiye Cumhuriyeti Kanunları geçerlidir. İletişim ve destek talepleri için Valerion Studios resmi Discord kanalları veya `VALERION` (`832617684285915226`) yetkilisi ile iletişim kurulabilir.

---
*© 2026 Valerion Studios. Tüm hakları saklıdır.*
