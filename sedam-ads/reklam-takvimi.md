# Sedam Müzik — Reklam Takvimi

Güncelleme: **5 Ekim 2026**
Veri kaynağı: Genel bakış kartları ZIP — `Gün_ve_saat(Saat)` (20 Eyl – 5 Eki 2026, 12 aktif gün)
Kampanya: `Sedam - Arama - Eylul 2026` (ID 24268863002)

Uygulama: Kampanyalar → `Sedam - Arama - Eylul 2026` → Ayarlar → Reklam takvimi → Düzenle

---

## Uygulanacak tablo

6 satır, hepsi **"Her gün"**. 23:00-07:00 listede yok = kapalı.

| # | Saat | Mevcut | **Yeni** |
|---|---|---|---|
| 1 | 07:00 – 12:00 | -%5 | **-%40** |
| 2 | 12:00 – 14:00 | 0 | **-%20** |
| 3 | 14:00 – 16:00 | +%15 | **0** |
| 4 | 16:00 – 19:00 | +%25 | **+%10** |
| 5 | 19:00 – 21:00 | +%10 | **+%15** |
| 6 | 21:00 – 23:00 | **-%20** | **+%15** |

---

## Neden — `21-23` gerçek zirveyken kısılıyordu

Saatlik gösterim (12 aktif gün):

| Saat | 07 | 08 | 09 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Göstr. | 23 | 18 | 16 | 41 | 31 | 66 | 58 | 86 | 104 | 99 | 105 | 141 | **161** | 90 | 106 | 89 |

Ham gösterime bakmak hata olur: her bant **kendi teklif düzeltmesinin baskısı altında** oluştu.
Kısılan bant az gösterim alır, bu da "demek ki talep yok" yanılgısı üretir. Düzeltmeden
arındırmak için gözlem `(1 + düzeltme)`'ye bölünür:

| Bant | Göstr. | Saat | Gözlenen/saat | Mevcut | **Arındırılmış talep/saat** |
|---|---|---|---|---|---|
| 07-12 | 129 | 5 | 25,8 | -%5 | **27,2** |
| 12-14 | 124 | 2 | 62,0 | 0 | **62,0** |
| 14-16 | 190 | 2 | 95,0 | +%15 | **82,6** |
| 16-19 | 345 | 3 | 115,0 | +%25 | **92,0** |
| 19-21 | 251 | 2 | 125,5 | +%10 | **114,1** |
| **21-23** | 195 | 2 | 97,5 | **-%20** | **121,9** ← zirve |

İki ters durum:
- **`21-23` arındırılmış talebin zirvesi ama `-%20` yiyor.** Müzik kursu arayan veli akşam
  geç saatte araştırıyor; kampanya tam o saatte frene basıyor.
- **`07-12` talebin dörtte birini üretiyor ama neredeyse düzeltmesiz** (`-%5`). Beş saatlik
  en geniş bant, en az talep.

Yeni değerlerin talep ağırlıklı ortalaması **+%1,6** — toplam TBM'i şişirmez, sadece parayı
saatler arasında yeniden dağıtır.

---

## Gün katmanı — bu tur EKLENMEDİ

| Gün | Göstr. | Geçerli gün | Gün başına |
|---|---|---|---|
| Pazartesi | 275 | 2 | 137,5 |
| Salı | 254 | 2 | 127,0 |
| Pazar | 215 | 2 | 107,5 |
| Cumartesi | 101 | **1** | 101,0 |
| Çarşamba | 174 | 2 | 87,0 |
| Perşembe | 149 | 2 | 74,5 |
| Cuma | 66 | **1** | 66,0 |

İki gerekçe:

1. **Cuma ve Cumartesi'nin birer geçerli günü var** — 2-3 Ekim'de ödeme sorunu yüzünden
   yayın durmuştu. Tek günlük örnekle gün düzeltmesi yazmak 21 Eylül'ün demografi hatasını
   tekrarlamak olur.
2. **Ads'te ayrı gün katmanı yok.** Gün ve saat düzeltmesi birlikte isteniyorsa çarpımları
   tek satıra yazılır: 7 gün × 6 bant = **42 satır**. İnce veri için pahalı bir işlem.

Not: Perşembe (74,5) ve Çarşamba (87) ikişer günlük veriyle istikrarlı biçimde ortalamanın
altında. 22 Ekim kapanış raporunda tekrar bakılacak.

---

## Uygulama tuzakları

- **Tablo sanallaştırılmış** — satırlar görünür alana gelmeden DOM'a girmez. "Her gün" olarak
  girilen 6 bant tabloda 7 × 6 = 42 satıra açılır.
- **Toplu düzenleme:** satırları seç → mavi çubuk → `Düzenle → Teklif ayarlamalarını
  değiştirin` → Artır/Azalt + yüzde → Uygula.
- **Uygula sonrası tablo bozuk render edebilir** — sayfayı yenile, panik yapma.
- Düzeltmeler kampanya seviyesinde, reklam grubu seviyesinde değil.
- Değişiklik 24 saat içinde etkisini gösterir.

---

İlgili: `cihaz-bid-ayarlari.md` · `session-log-2026-10-05.md`
