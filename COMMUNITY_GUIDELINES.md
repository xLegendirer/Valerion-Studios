# 💎 VALERION ECOSYSTEM — COMPREHENSIVE ENTERPRISE COMMUNITY & VIP GUIDELINES
### (TOPLULUK STANDARTLARI, VIP HİYERARŞİSİ VE EDEB POLİTİKASI)

**Doküman Kodu:** `DOC-VAL-COM-2026-V7`  
**Sürüm:** `v7.0.0-ENTERPRISE-FULL`  
**Yürürlük Tarihi:** 17 Ağustos 2026  
**Son Güncelleme:** 17 Ağustos 2026  
**Hukuki Dayanak:** Discord Community Guidelines, Roblox Community Standards & Terms of Use, Valerion Ecosystem Terms of Service, Fair Use & Etiquette Framework.

---

## 1. MİSYON, VİZYON VE TOPLULUK FİLOZOFİSİ

### 1.1. Amacımız
**Valerion Ecosystem** ("Platform", "Topluluk"), bünyesindeki Discord sunucularında, entegre Web Kontrol Panelinde (`dashboard.html` / `manage.html`) ve 7 senkronize bot mikroservisinde (**Valerion Link, System, Server, Voice, Club, Economy, Fun**) elit, seviyeli, adil, kurumsal ve güvenli bir dijital sosyal ekosistem sunmayı amaçlar.

### 1.2. Kapsam
İşbu Topluluk & VIP Kuralları; metin kanallarında, dinamik ses odalarında, VIP Lounge alanlarında, Roblox rütbe/hesap bağlama süreçlerinde, ekonomi/borsa simülasyonlarında ve bot komut kullanımlarında tüm üyelerin uymakla yükümlü olduğu temel ilke ve standartları belirler.

---

## 2. GENEL TOPLULUK VE SOHBET STANDARTLARI

Sunucu içi tüm yazılı, görsel ve sesli iletişim kanallarında aşağıdaki kurallara uyulması zorunludur:

### 2.1. Nefret Söylemi, Taciz ve Ayrımcılık Yasağı
* **2.1.1.** Irk, etnik köken, din, mezhep, cinsiyet, cinsel yönelim, engellilik durumu veya siyasi görüş üzerinden kişileri hedef göstermek, aşağılamak, nefret söyleminde bulunmak veya taciz etmek kesinlikle yasaktır.
* **2.1.2.** Üyelere veya yönetim ekibine yönelik tehdit, şantaj, ifşa (doxxing) veya siber zorbalık girişimleri doğrudan sunucudan ve ekosistem genelinden kalıcı olarak uzaklaştırılma (**Global Blacklist**) ile sonuçlanır.

### 2.2. Reklam, Tanıtım ve Spam Yasağı
* **2.2.1.** Sunucu içi kanallarda, ses odası başlıklarında, kullanıcı takma adlarında veya üyelere gönderilen Özel Mesajlarda (DM) izinsiz başka Discord sunucusu, sosyal medya hesabı, satış platformu veya ticari reklam paylaşmak yasaktır.
* **2.2.2.** Kanallarda sohbet akışını bozacak şekilde mesaj tekrarı yapmak (Spam), anlamsız karakter dizileri harmanlamak, aşırı büyük harf (Caps Lock) kullanmak veya 10'dan fazla emoji içeren mesajlar göndermek Guard sistemi tarafından filtrelenir ve ihtar puanı yazılır.

### 2.3. NSFW ve Uygunsuz İçerik Yasağı
* Sohbet kanallarında, Roblox profil açıklamalarında veya profil görsellerinde cinsel içerik, vahşet (gore), yasa dışı maddeleri teşvik eden öğeler veya telif ihlali barındıran medyalara yer verilemez.

---

## 3. ROBLOX ENTEGRASYONU, HESAP BAĞLAMA VE RÜTBE EDEBİ

Valerion Link altyapısı üzerinden Roblox hesaplarını Discord hesaplarıyla eşleştiren üyeler aşağıdaki kurallara riayet etmekle yükümlüdür:

### 3.1. Kimlik Doğrulama ve Çoklu Hesap Kullanımı
* **3.1.1.** Üyeler yalnızca kendilerine ait olan meşru Roblox hesaplarını `/link` (OAuth2 veya Bio yöntemi) ile bağlayabilir. Başka bir kullanıcıya ait hesabı yetkisiz doğrulamaya çalışmak doğrudan dolandırıcılık sayılır.
* **3.1.2.** Çoklu hesap bağlama özelliği (`/roblox-hesaplarim`) sunucu içi rütbe ve rol suiistimali amacıyla kullanılamaz. Aktif hesap (`is_primary`) değiştirildiğinde roller ve takma ad yeni hesaba göre anında yeniden eşitlenir.

### 3.2. Yasaklı Hesaplar ve Grup Zorunluluğu (Force Join)
* **3.2.1.** Roblox platformu üzerinde kalıcı veya geçici olarak yasaklanmış (`isBanned: true`) hesaplar güvenlik filtresine takılır ve ekosisteme bağlanamaz.
* **3.2.2.** Sunucu yönetiminin grup zorunluluğu getirdiği durumlarda, ana Roblox grubundan ayrılan üyelerin doğrulanmış (`Verified`) statüleri ve gruba bağlı özel yetki rolleri otomatik olarak geri çekilir.

---

## 4. VIP HİYERARŞİSİ VE AYRICALIKLARIN KULLANIMI

Valerion Ekosisteminde üyelere tanınan VIP yetkileri PostgreSQL altyapısıyla (`vips_v2`) takip edilen hiyerarşik bir otorite yapısına dayanır:

```text
👑 Level 7: VALERION (Bot Sahibi)
👑 Level 6: SERVER OWNER (Sunucu Sahibi)
💎 Level 5: CVIP (Custom / Corporate VIP)
🌟 Level 4: SSSVIP (Super Super Super VIP)
⚡ Level 3.5: C-SUB (Abonelik Hediye Statüsü)
💥 Level 3: SSVIP (Super Super VIP)
🔹 Level 2: SVIP (Super VIP)
▫️ Level 1: VIP (VIP Üye)
