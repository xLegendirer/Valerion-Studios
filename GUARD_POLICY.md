# 🛡️ VALERION ECOSYSTEM — COMPREHENSIVE ENTERPRISE GUARD & ENFORCEMENT POLICY
### (GÜVENLİK MİMARİSİ, OTOMATİK DENETİM VE İHTAR SİSTEMİ POLİTİKASI)

**Doküman Kodu:** `DOC-VAL-GRD-2026-V7`  
**Sürüm:** `v7.0.0-ENTERPRISE-FULL`  
**Yürürlük Tarihi:** 17 Ağustos 2026  
**Son Güncelleme:** 17 Ağustos 2026  
**Hukuki Dayanak:** Valerion Ecosystem Terms of Service, Discord Developer Terms & Policy, Roblox Open Cloud Security Standards, Automated Enforcement Framework.

---

## 1. MİSYON, GÜVENLİK FİLOZOFİSİ VE OTOMASYON

### 1.1. Otomatik Güvenlik Yaklaşımı
**Valerion Ecosystem** sunucu güvenliği, veri bütünlüğü ve topluluk düzeni; insani hata payını ve yetkili inisiyatifini en aza indiren **Valerion Server Guard (`DISCORD_TOKEN_SERVER`)** ve **Valerion Link Security Engine** tarafından 7/24 esasına göre gerçek zamanlı olarak sağlanmaktadır.

### 1.2. Kapsam ve Çalışma Prensibi
Güvenlik mimarisi; mesaj içeriklerini, kullanıcı giriş frekanslarını, yetki değişikliklerini, kanal/rol oluşturma-silme eylemlerini, webhook manipülasyonlarını ve Roblox OAuth2 yetkilendirme doğrulamalarını mikrosaniyeler düzeyinde analiz eder. Güvenlik duvarını ihlal eden eylemleri anında engelleyerek geri alır (Rollback) ve veritabanı tabanlı (`user_warns`) kademeli yaptırım sistemini devreye sokar.

---

## 2. OTOMATİK İHTAR (WARN) VE KADEMELİ CEZA EŞİK SİSTEMİ

Server Guard, tespit ettiği ihlalleri PostgreSQL veritabanındaki `user_warns` tablosuna **İhtar Puanı** olarak işler. Biriken ihtar puanlarına göre sistem aşağıdaki cezaları otomatik olarak uygular:

```text
  [0-2 İhtar Puanı]   ---> 🟢 Normal Statü (Sistem Takibinde)
  [3-4 İhtar Puanı]   ---> 🔕 Otomatik 1 Saat Timeout (Yazı & Ses Engeli)
  [5-6 İhtar Puanı]   ---> ☣️ Otomatik Karantina (Rol Hafızalı İzole Alan)
  [7+ İhtar Puanı]    ---> 🚨 Otomatik Sunucu Banı (1 Saatlik Mesaj Temizliği + Global Blacklist İncelemesi)
