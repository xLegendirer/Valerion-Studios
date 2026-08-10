# 🛡️ VALERION NETWORK — GUARD & ENFORCEMENT POLICY (GÜVENLİK VE CEZA POLİTİKASI)

**Son Güncelleme:** 10 Ağustos 2026  
**Yürürlük Tarihi:** 10 Ağustos 2026  
**Sürüm:** v2.4.0-GRD  

---

## 1. GÜVENLİK FİLOZOFİSİ VE OTOMASYON
Valerion Network sunucu güvenliği, insan müdahalesine olan ihtiyacı minimize eden **Valerion Server Guard** yapay zeka ve otomatik denetim motoru tarafından 7/24 esasına göre sağlanmaktadır. 

Server Guard, sunucu içi eylemleri mikro saniyeler düzeyinde analiz eder, yetkisiz sınır aşımlarını engeller ve kademeli ceza protokollerini devreye sokar.

---

## 2. OTOMATİK İHTAR (WARN) VE CEZA EŞİK SİSTEMİ
Kullanıcıların gerçekleştirdiği kural ihlalleri veritabanında `user_warns` tablosuna **İhtar Puanı** olarak işlenir. İhtar puanları biriktikçe sistem otomatik olarak aşağıdaki cezaları uygular:

```text
  [0-2 İhtar Puanı]  ---> 🟢 Normal Statü (Sistem Takibinde)
  [3-4 İhtar Puanı]  ---> 🔕 Otomatik 1 Saat Timeout (Ses & Yazı Engeli)
  [5-6 İhtar Puanı]  ---> ☣️ Otomatik Karantina (Roller Saklanır & Çekilir)
  [7+ İhtar Puanı]   ---> 🚨 Otomatik Sunucu Banı (1 Saatlik Mesaj Temizliği)
