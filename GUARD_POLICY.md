# 🛡️ VALERION NETWORK — COMPREHENSIVE ENTERPRISE GUARD & ENFORCEMENT POLICY
### (GÜVENLİK MİMARİSİ, OTOMATİK DENETİM VE İHTAR SİSTEMİ POLITİKASI)

**Doküman Kodu:** `DOC-VAL-GRD-2026-V6`  
**Sürüm:** `v6.0.0-ENTERPRISE-FULL`  
**Yürürlük Tarihi:** 10 Ağustos 2026  
**Son Güncelleme:** 10 Ağustos 2026  
**Hukuki Dayanak:** Valerion Network Terms of Service, Discord Security & Developer Policy, Automated Enforcement Framework.

---

## 1. MİSYON, GÜVENLİK FİLOZOFİSİ VE OTOMASYON

### 1.1. Otomatik Güvenlik Yaklaşımı
**Valerion Network** sunucu güvenliği ve topluluk düzeni, insani hata payını ve yetkili inisiyatifini en aza indiren **Valerion Server Guard (`DISCORD_TOKEN_SERVER`)** yapay zeka ve otomatik denetim motoru tarafından 7/24 esasına göre sağlanmaktadır.

### 1.2. Kapsam ve Çalışma Prensibi
Server Guard motoru; mesaj içeriklerini, kullanıcı katılma oranlarını, yetki değişikliklerini, kanal/rol silme eylemlerini ve etiket kullanımlarını mikro saniyeler düzeyinde analiz eder. Güvenlik duvarını ihlal eden eylemleri anında engelleyerek veritabanı tabanlı (`user_warns`) kademeli ceza sistemini çalıştırır.

---

## 2. OTOMATİK İHTAR (WARN) VE KADEMELİ CEZA EŞİK SİSTEMİ

Server Guard, tespit ettiği ihlalleri veritabanındaki `user_warns` tablosuna **İhtar Puanı** olarak işler. Biriken ihtar puanlarına göre sistem aşağıdaki cezaları otomatik olarak uygular:

```text
  [0-2 İhtar Puanı]  ---> 🟢 Normal Statü (Sistem Takibinde)
  [3-4 İhtar Puanı]  ---> 🔕 Otomatik 1 Saat Timeout (Yazı & Ses Engeli)
  [5-6 İhtar Puanı]  ---> ☣️ Otomatik Karantina (Rol Hafızalı İzole Alan)
  [7+ İhtar Puanı]   ---> 🚨 Otomatik Sunucu Banı (1 Saatlik Mesaj Temizliği)
