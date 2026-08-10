# 📜 VALERION NETWORK — COMPREHENSIVE ENTERPRISE TERMS OF SERVICE
### (GENEL HİZMET KULLANIM, MİMARİ VE HUKUKİ ŞARTLAR SÖZLEŞMESİ)

**Doküman Kodu:** `DOC-VAL-TOS-2026-V6`  
**Sürüm:** `v6.0.0-ENTERPRISE-FULL`  
**Yürürlük Tarihi:** 10 Ağustos 2026  
**Son Güncelleme:** 10 Ağustos 2026  
**Hukuki Dayanak:** T.K.K.K. (6698 Sayılı KVKK), AB Genel Veri Koruma Yönetmeliği (GDPR - EU 2016/679), Discord Developer Terms of Service and Developer Policy, US Fair Credit Reporting Act (Analogous Virtual Terms).

---

## 1. GİRİŞ, TARAFLAR VE ANLAŞMANIN AKDİ

### 1.1. Sözleşmenin Tarafları
İşbu Hizmet Kullanım Sözleşmesi ("Sözleşme" veya "TOS"), **Valerion Studios / Valerion Network** ("Şirket", "Platform", "Biz", "Altyapı", "Sistem") ile Valerion Ekosistemi bünyesindeki Discord sunucularına katılan, altyapıda barındırılan bot servislerini kullanan, komut çalıştıran veya bu altyapıyla dolaylı/doğrudan etkileşime giren tüm gerçek ve tüzel kişiler ("Kullanıcı", "Üye", "Siz", "Son Kullanıcı") arasında hukuki olarak bağlayıcı bir şekilde akdedilmiştir.

### 1.2. Hukuki Onay, Tek Komut Onayı ve Otomatik Kabul
* **1.2.1. İncelenmişlik Beyanı:** Valerion Network platformuna erişim sağlayarak, sunuculara katılarak veya altyapıda barındırılan 6 bottan herhangi birini etkileşime sokarak işbu Sözleşme'nin tüm maddelerini kabul etmiş sayılırsınız.
* **1.2.2. Tek Komut / Etkileşim İle Onay (Single-Command Consent):** Valerion Ekosistemi bünyesindeki herhangi bir bot üzerinde **TEK BİR SLASH (`/`) VEYA PREFİKS (`!`) KOMUTUNUN ÇALIŞTIRILMASI, SES KANALLARINA GİRİŞ YAPILMASI VEYA BUTON/MENÜ ETKİLEŞİMİNDE BULUNULMASI**, kullanıcının işbu Hizmet Şartları'nı, Gizlilik Politikasını, Topluluk Kurallarını ve Guard Güvenlik Politikası'nı tamamen okuduğu, anladığı ve **KOŞULSUZ OLARAK KABUL ETTİĞİ** anlamına gelir.
* **1.2.3. Onayın Bağlayıcılığı:** "Okumadım", "Görmedim" veya "Haberim Yoktu" beyanları hukuki geçersizlik teşkil etmez; ilk komut kullanımıyla birlikte onay veritabanı zaman damgaları (ISO 8601) ile eşleşerek bağlayıcı hale gelir.

### 1.3. Şartların Reddi Halinde Prosedür
İşbu Sözleşme'de yer alan şartlardan herhangi birini kabul etmiyorsanız, Valerion Network altyapısına bağlı tüm servislerin kullanımına derhal son vermeli, etkileşimli bot komutlarını çalıştırmayı bırakmalı ve bağlı bulunduğunuz topluluk sunucularından ayrılmalısınız. Aksi takdirde altyapıda gerçekleştirdiğiniz her işlem işbu Sözleşme hükümleri çerçevesinde değerlendirilecektir.

---

## 2. SÖZLEŞMESEL TANIMLAR VE KAVRAMLAR

İşbu Sözleşme içerisinde yer alan terimler aksi açıkça belirtilmedikçe aşağıdaki anlamları ifade eder:
* **Ekosistem / Ağ:** Valerion Network bünyesinde çalışan 6 adet senkronize mikroservis botunu (System, Server, Voice, Club, Economy, Fun), veritabanı sunucularını ve ilgili Discord topluluk alanlarını.
* **Sanal Varlık:** Ekosistem içerisinde kazanılan, satın alınan veya transfer edilen Coin, Mülk, Araç, Hisse, Kripto Para, Rozet ve VIP statülerini.
* **Global Blacklist (Ağ Kara Listesi):** Ekosisteme bağlı tüm botlarda geçerli olan, kullanıcının komut çalıştırma ve erişim haklarının sistem seviyesinde kalıcı olarak engellenmesini.
* **Bot Sahibi / Developer:** Altyapının tüm telif, kod ve mülkiyet haklarına sahip olan `VALERION` (ID: `832617684285915226`) yetkili hesabını.
* **Guard Motoru:** Sunucu güvenliğini, izinsiz eylemleri, spam ve raid girişimlerini denetleyen otomatik güvenlik yazılımını.

---

## 3. DAĞITIK MİKROSERVİS MİMARİSİ VE SERVİS KAPSAMI

### 3.1. Mikroservis Mimarisi
Valerion Network, Discord Inc. API'si ve bağımsız sunucu altyapıları üzerine inşa edilmiş, kendi aralarında senkronize çalışan dağıtık bir bot ekosistemidir. Platform hizmetleri aşağıdaki 6 ana servis biriminin entegre çalışmasıyla sunulmaktadır:

* **3.1.1. Valerion System Bot (`DISCORD_TOKEN_SYSTEM`):** Otorite hiyerarşisi (Level 0 ile Level 7 arası), VIP tanımlama/silme, OwO otomatik ödeme yakalama motoru, kullanıcı sicil kartları, loglama ve küresel bakım ayarlarını yöneten ana konsol.
* **3.1.2. Valerion Server Guard Bot (`DISCORD_TOKEN_SERVER`):** Enterprise düzeyde sunucu koruma duvarı, anti-raid, anti-spam, mass-mention engeli, izinsiz yetki yükseltme koruması, karantina yönetimi, tuzak kanal (trap channel) algılayıcı ve otomatik ihtar (warn) motoru.
* **3.1.3. Valerion Voice Bot (`DISCORD_TOKEN_VOICE`):** Ses aktiflik ve süre takibi, dinamik oda oluşturucu (`🔊 Lounge`), oda sahipliği kontrol panelleri ve yerel Lavalink (Port 2289) / Wavelink yüksek kaliteli ses akış motoru.
* **3.1.4. Valerion Club Bot (`DISCORD_TOKEN_CLUB`):** VIP Lounge etkileşimleri, C-SUB abonelik hediye mekanizması, rozet vitrini (`user_badges`), prestij düelloları ve elit topluluk ayrıcalıkları.
* **3.1.5. Valerion Economy Bot (`DISCORD_TOKEN_ECONOMY`):** Merkez bankacılığı, sanal borsa, gayrimenkul ve garaj yönetimi, şirket/İK simülasyonu, vergi/hukuk sistemleri, karaborsa ve şans oyunları (Casino Engine).
* **3.1.6. Valerion Fun Bot (`DISCORD_TOKEN_FUN`):** Sosyal etkileşim araçları, mini oyunlar, MyAnimeList entegrasyonu, AFK modları ve topluluk mizah panelleri.

---

## 4. VERİTABANI SENKRONİZASYON VE SİNYALİZASYON PROTOKOLÜ (NOTIFY/LISTEN)

### 4.1. Anlık Sinyal Dinleme Hattı
Platform servisleri, PostgreSQL ilişkisel veritabanı altyapısı üzerinde `config_update` kanalı üzerinden çalışan anlık sinyal dinleyicileri (`NOTIFY / LISTEN`) ile birbirine bağlıdır.

### 4.2. RAM Önbellekleme (Cache Efficiency)
Bir bot üzerinde yapılan bakım modu güncellemesi, yetki değişikliği veya kara liste ekleme işlemi veritabanında gerçekleştikten mikro saniyeler sonra sinyalizasyon hattı üzerinden diğer 5 botun RAM belleklerine (Cache) yansıtılır. Böylece ağ genelinde gecikmesiz güvenlik denetimi sağlanır.

---

## 5. KULLANICI HESAPLARI, YETKİNLİK VE YAŞ SINIRI BEYANLARI

### 5.1. Discord Hesap Eşleşmesi
Tüm hizmetler kullanıcıların benzersiz Discord Hesap ID'leri (`BIGINT`) üzerinden yürütülür.
* **5.1.1.** Hesabınız üzerinden gerçekleştirilen tüm mesajlaşma, bakiye transferi, şirket yönetimi, ses odası eylemleri ve Guard kural ihlalleri doğrudan ilgili hesap sahibinin sorumluluğundadır.
* **5.1.2.** Üçüncü şahısların hesabınızı kullanması, hesabınızın çalınması veya yetkisiz erişime uğraması sonucu doğabilecek hak kayıpları ve cezalardan Valerion Network sorumlu tutulamaz.

### 5.2. Yaş Kısıtlaması ve Dijital Rıza
* **5.2.1.** Kullanıcılar, Discord Inc. Hizmet Şartları uyarınca en az 13 yaşında (veya bulundukları ülkenin yerel mevzuatına göre gerekli minimum dijital rıza yaş sınırında) olduklarını beyan ve taahhüt ederler.
* **5.2.2.** 13 yaşın altında olduğu tespit edilen kullanıcıların hesapları, çocuk koruma politikalarımız gereği derhal ve bildirim yapılmaksızın **Ağ Kara Listesine (Global Blacklist)** alınarak servis erişimleri engellenir.

---

## 6. SİSTEM GÜVENLİĞİ, YASAKLI EYLEMLER VE KÖTÜYE KULLANIM (ANTI-ABUSE)

Valerion Network altyapısının kararlılığını, adil kullanım dengesini ve sunucu güvenliğini korumak amacıyla aşağıda belirtilen eylemler **kesin bir dille yasaklanmıştır**:

* **6.1.** Bot yazılımlarını veya sunucu altyapısını sabote etmeye yönelik her türlü eylem.
* **6.2.** Sanal ekonomi veya VIP sistemlerinde adil olmayan avantajlar sağlamaya çalışmak.
* **6.3.** Sunucu düzenini veya diğer üyelerin huzurunu sistemli şekilde bozmak.

---

## 7. YAZILIM AÇIKLARI, HAK SINIRI VE EXPLOIT SUİSTİMALİ PROSEDÜRÜ

### 7.1. Exploit Yasağı
Bot kodlarında, Python asenkron döngülerinde, Wavelink ses sürücülerinde veya PostgreSQL veritabanı senkronizasyonlarında tespit edilen mantık hatalarını (bug) kişisel çıkar veya haksız bakiye/yetki sağlama amacıyla kullanmak kesinlikle yasaktır.

### 7.2. Bildirim Yükümlülüğü
Tespit edilen sistem açıkları derhal yetkililere bildirilmelidir. Açıkları suistimal eden veya başkalarıyla paylaşarak yayan kullanıcıların tüm sanal varlıkları, bakiyeleri ve rolleri kalıcı olarak sıfırlanır.

---

## 8. OTOMASYON, MAKRO VE SELF-BOT KULLANIM YASAĞI

### 8.1. Makro ve Yazılım Yasağı
Slash komutlarını otomatik yürütmek, sanal ekonomide haksız kazanç sağlamak, casino oyunlarını otomatikleştirmek veya ses süresi kasmak amacıyla makro, yazılım, script veya Discord Self-Bot istemcileri kullanmak yasaktır.

### 8.2. Otomatik Tespit
Otomasyon kullandığı tespit edilen hesaplar Guard algoritmaları tarafından tespit edilerek veri tabanından silinir ve erişimleri kısıtlanır.

---

## 9. AĞ VE SUNUCU SALDIRILARI (DoS/DDoS/SPAM) KORUMASI

### 9.1. Hizmet Engelleyici Saldırılar
Bot istemcilerine, Lavalink ses sunucularına (Port 2289) veya veritabanı uç noktalarına yönelik aşırı yükleme yapacak şekilde komut spam'i (Flood) yapmak, DoS/DDoS girişimlerinde bulunmak veya API uç noktalarını tersine mühendislikle suistimal etmek yasaktır.

### 9.2. Yasal İşlem
Bu tür eylemler yalnızca platform erişim engelini değil, aynı zamanda yasal bilişim suçu takibini de beraberinde getirir.

---

## 10. KÜRESEL AĞ YAPTIRIMLARI VE GLOBAL BLACKLIST (AĞ KARA LİSTESİ)

### 10.1. Global Blacklist Mekanizması
Valerion Network, 6 botun tamamını kapsayan merkezi bir **Bot Kara Liste (`bot_blacklist`)** veritabanına sahiptir.

### 10.2. Yaptırım Kapsamı
Kural ihlali gerçekleştirdiği tespit edilen, sistem açıklarını kullanan, ağ güvenliğini tehdit eden veya ağır topluluk ihlali yapan Kullanıcılar:
* **10.2.1.** Herhangi bir ihbarda bulunulmaksızın **Valerion Ekosistemi bünyesindeki 6 botun tamamından (Global Blacklist)** kalıcı olarak yasaklanır.
* **10.2.2.** Kara listeye alınan bir kullanıcı `/sistem-yardım`, `/vip-satınal` veya eğlence komutları dahil hiçbir komutu çalıştıramaz.
* **10.2.3.** Kara listeye alınan kullanıcının tüm VIP hakları, sanal bakiyeleri, mülkleri, rozetleri ve yetkileri tazminatsız olarak feshedilir ve veritabanından silinir.

---

## 11. SANAL EKONOMİ, FİNANSAL KOŞULLAR VE MÜLKİYET REJİMİ

### 11.1. Sanal Varlıkların Hukuki Statüsü
* **11.1.1.** Valerion Economy, Club ve System botlarında yer alan "Coin", "Banka Bakiyesi", "Hisse Senedi", "Kripto Varlık", "Gayrimenkul", "Araç" veya "VIP Üyelikler" tamamen sanal simülasyon öğeleridir.
* **11.1.2.** Bu varlıklar **gerçek para (fiat currency) karşılığına, nakdi değere veya yasal mülkiyet hakkına sahip değildir**.
* **11.1.3.** Sanal varlıklar hiçbir koşulda gerçek paraya dönüştürülemez, satılamaz, reel finansal borsalarla eşleştirilemez ve nakit olarak talep edilemez.

---

## 12. TİCARET YASAĞI (REAL MONEY TRADING - RMT)

Kullanıcıların sistem içi sanal Coin'leri, şirketleri, araçları veya VIP hesapları gerçek para karşılığında (Real Money Trading - RMT) 3. şahıslara devretmesi, satması veya takas etmesi kesinlikle yasaktır. Tespiti halinde ilgili tüm hesaplar sıfırlanır ve Global Blacklist uygulanır.

---

## 13. VIP ÜYELİKLER, HİYERARŞİ VE DİJİTAL HAKLAR

### 13.1. Otorite Hiyerarşisi
Platform üzerinde sunulan VIP statüleri hiyerarşik olup aşağıdaki düzeylerden oluşur:
- Level 7: VALERION (Bot Sahibi)
- Level 6: SERVER OWNER (Sunucu Sahibi)
- Level 5: CVIP (Custom / Corporate VIP)
- Level 4: SSSVIP (Super Super Super VIP)
- Level 3.5: C-SUB (Abonelik Hediye Statüsü)
- Level 3: SSVIP (Super Super VIP)
- Level 2: SVIP (Super VIP)
- Level 1: VIP (VIP Üye)

---

## 14. OWO OTOMATİK ÖDEME YAKALAMA VE DOĞRULAMA SİSTEMİ

OwO bakiyesi veya onaylanmış diğer sistem içi yöntemlerle alınan VIP paketleri, OwO otomatik ödeme motoru (`PENDING_ORDERS`) tarafından doğrulanarak anında veritabanına (`vips_v2`) işlenen ve ifa edilen dijital hizmetler kapsamındadır.

---

## 15. KESİN İADE MÜMKÜNSÜZLÜĞÜ POLİTİKASI (NO-REFUND POLICY)

### 15.1. Dijital İfa
Satın alınan tüm VIP paketleri, dijital kartlar ve C-SUB hakları hesabınıza tanımlandığı andan itibaren **iade edilemez, iptal edilemez ve bakiye olarak geri istenemez**.

### 15.2. Ceza Durumunda VIP Hakları
Herhangi bir kural ihlali (Guard engeli, Blacklist, Karantina, Otomatik Ban) sebebiyle sunucudan veya bot altyapısından uzaklaştırılan kullanıcıların kalan VIP süreleri dondurulmaz, devredilemez ve ücret/bakiye iadesi yapılmaz.

---

## 16. C-SUB ABONELİK HEDİYE MEKANİZMASI VE İPTAL ŞARTLARI

`CVIP` seviyesindeki üyelere tanınan C-SUB hediye etme hakkı kişiye özeldir. Hediye edilen kullanıcının topluluk veya güvenlik kurallarını ihlal etmesi durumunda, yetkililer veya hediye eden CVIP üyesi aboneliği iptal edebilir.

---

## 17. GUARD (KORUMA) MİMARİSİ VE OTOMATİK İHTAR (WARN) MOTORU

Server Guard botu, sunucu içi eylemleri izleyerek kural ihlali yapan kullanıcılara otomatik ihtar puanı ekler (`user_warns`):
* **3 İhtar Puanı:** Kullanıcıya 1 saatlik otomatik Timeout (Ses ve Yazı Mute) uygulanır.
* **5 İhtar Puanı:** Kullanıcının mevcut tüm rolleri veritabanına (`quarantine_history`) saklanarak çekilir ve kullanıcı Otomatik Karantinaya alınır.
* **7 İhtar Puanı:** Kullanıcı sunucudan otomatik olarak Banlanır ve son 1 saatlik mesaj geçmişi temizlenir.

---

## 18. OTOMATİK TUZAK KANALLAR (TRAP CHANNELS) VE CEZAİ HÜKÜMLER

Yöneticiler tarafından belirlenen tuzak kanallara (`/guard-trap-kanal`) yazılan her türlü mesaj, hesabın otomatik spam/self-bot olduğu kabul edilerek mesaj anında silinir ve hesap **otomatik olarak banlanır**.

---

## 19. ANTI-NUKE, YETKİ YÜKSELTME VE SUNUCU SABOTAJ KORUMASI

Whitelist (Güvenli Liste) içerisinde bulunmayan bir yetkili, başka bir üyeye `Administrator` veya `Manage Roles` yetkisi vermeye çalıştığında Guard anında müdahale eder. Verilen rol geri alınır ve yetkiyi veren yetkilinin tüm rolleri sıfırlanır.

---

## 20. SES KANALLARI, DİNAMİK ODA YÖNETİMİ VE ÖZEL İZİNLER

Dinamik ses kanallarında (`🔊 Lounge`) oda sahipliği odayı oluşturan kişiye aittir. Ancak oda isimlerinde ve ses yayınlarında topluluk kurallarına aykırı hareket edilemez.

---

## 21. FİKRİ MÜLKİYET, TELİF HAKLARI VE KOD KORUMA REJİMİ

### 21.1. Telif Hakları
Valerion Network altyapısına ait tüm yazılım kaynak kodları, C++ ve Lua komut mimarileri, Python bot modülleri, PostgreSQL veritabanı şemaları, özel algoritma tasarımları, grafik materyalleri, logo ve ticari unvanlar **Valerion Studios** ve ilgili geliştiricilerine aittir.

### 21.2. İzinsiz Kullanım Yasağı
Yazılı izin alınmaksızın kodların kopyalanması, tersine mühendislik uygulanması, başka projelerde izinsiz kullanılması veya yeniden dağıtılması telif hakları mevzuatai uyarınca yasal işlem sebebidir.

---

## 22. HİZMET SEVİYESİ TAAHHÜDÜ (SLA) VE GARANTİ REDDİ

Valerion Network, hizmetlerin %100 kesintisiz, hatasız veya siber saldırılardan tamamen muaf olacağını garanti etmez. Hizmetler "OLDUĞU GİBİ" (AS IS) esasında sunulmaktadır.

---

## 23. SORUMLULUK SINIRLAMASI (LIMITATION OF LIABILITY)

Discord API güncellemeleri, küresel internet altyapı arızaları, fiziksel sunucu (Render/Hosting) problemleri, veritabanı bakımları veya Lavalink ses motoru güncellemeleri nedeniyle yaşanabilecek veri kayıpları, bakiye zararları veya hizmet kesintilerinden Şirketimiz sorumlu tutulamaz.

---

## 24. VERİ GİZLİLİĞİ, BÜTÜNLÜĞÜ VE SAKLAMA ŞARTLARI

Kullanıcı verileri, platformumuzun `PRIVACY_POLICY.md` dokümanında belirtilen esaslara uygun olarak saklanır ve işlenir. Veritabanı bağlantıları SSL/TLS protokolleri ile korunmakta olup yetkisiz erişimlere karşı izole edilmiştir.

---

## 25. MÜCBİR SEBEPLER (FORCE MAJEURE)

Hacker saldırıları, siber savaşlar, Discord API'sinin tamamen erişime kapanması, küresel sunucu altyapı çöküntüleri, doğal afetler veya yasal düzenlemeler gibi Valerion Network'ün makul kontrolü dışındaki durumlar mücbir sebep olarak kabul edilir. Bu sürede hizmetlerin aksamasından Platform sorumlu tutulamaz.

---

## 26. SÖZLEŞMENİN DEĞİŞTİRİLMESİ, GÜNCELLENMESİ VE BİLDİRİMLER

Valerion Network, işbu Sözleşme şartlarını, VIP paket fiyatlarını, ceza politikalarını ve bot özelliklerini dilediği zaman, tek taraflı olarak güncelleme ve değiştirme hakkını saklı tutar. Güncellenmiş koşullar bu dokümanda yayınlandığı andan itibaren yürürlüğe girer.

---

## 27. FESİH, SÖZLEŞMENİN BÖLÜNEBİLİRLİĞİ VE FERAGAT EDİLEMEZLİK

İşbu Sözleşme'nin herhangi bir maddesinin yetkili mahkemelerce geçersiz veya uygulanamaz bulunması halinde, bu durum Sözleşme'nin diğer maddelerinin geçerliliğini etkilemez.

---

## 28. UYGULANACAK HUKUK, YETKİLİ YARGI VE İLETİŞİM KANALLARI

### 28.1. Uygulanacak Hukuk
İşbu Sözleşme'nin uygulanmasından ve yorumlanmasından doğabilecek her türlü uyuşmazlığın çözümünde Türkiye Cumhuriyeti Kanunları uygulanır.

### 28.2. İletişim Kanalları
Hizmet şartları, güvenlik bildirimleri veya veri yönetimi talepleriniz için Valerion Studios resmi Discord sunucusu veya bot geliştiricisi `VALERION` (`832617684285915226`) ile iletişime geçebilirsiniz.

---
*© 2026 Valerion Studios. Tüm hakları saklıdır.*
