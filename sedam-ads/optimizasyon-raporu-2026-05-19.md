# Sedam Müzik Google Ads Optimizasyon Raporu
Tarih: 19 Mayıs 2026
Dönem: 19 Nisan - 18 Mayıs 2026 (30 günlük veri)
Kampanya: YENİ

---

## 1. Kritik Bulgular

### Display Ağı Sorunu (HEMEN MÜDAHALE)

| Ağ | Harcama | Tıklama | Ort. CPC |
|----|---------|---------|----------|
| Google Arama | ₺1,960.74 | 173 | ₺11.33 |
| Görüntülü Reklam (Display) | ₺409.10 | 96 | ₺4.26 |

- Önceki dönemde ölçülen CTR %5.10 iken bu dönem %2.87'ye düştü
- Display ağı CTR'ı doğası gereği düşüktür ve genel metriği bozuyor
- Display ayrı bütçe + ayrı kreatif gerektirir; Search ile aynı kampanyada tutmak verimsiz
- **Öneri:** Display'i duraklat veya ayrı kampanyaya al

---

### Cihaz Dağılımı (KRİTİK)

| Cihaz | Harcama | Pay | Tıklama |
|-------|---------|-----|---------|
| Cep telefonları | ₺2,246.09 | %94.8 | 249 |
| Bilgisayarlar | ₺101.07 | %4.3 | 15 |
| Tabletler | ₺22.68 | %0.9 | 5 |

- Bütçenin neredeyse tamamı mobilde — cihaz teklifi ayarlanmadan bütçe optimum kullanılmıyor
- Desktop tıklamaları mobil kadar yüksek CVR verebilir (müzik kursu kayıt formu masaüstünde daha kolay dolduruluyor)
- **Öneri:** Mobil -%20, Desktop +%15, Tablet -%80

---

### Zaman Analizi

**Saat bazlı gösterim (tüm hafta ortalaması):**

| Saat | Gösterim | Yorum |
|------|----------|-------|
| 17:00 | 1,017 | ZİRVE |
| 18:00 | 1,004 | Yüksek |
| 16:00 | 865 | Yüksek |
| 15:00 | 738 | Orta-Yüksek |
| 14:00 | 516 | Orta |
| 03:00 | 63 | Çok düşük |
| 04:00 | 32 | En düşük |

**Gün bazlı gösterim:**

| Gün | Gösterim |
|-----|----------|
| Salı | 2,230 |
| Cumartesi | 1,404 |
| Pazartesi | 1,441 |
| Perşembe | 1,383 |
| Çarşamba | 1,048 |
| Cuma | 983 |
| Pazar | 873 |

- Gece 00:00-07:00 arası reklam gösterimi bütçeyi boşa harcıyor
- Peak saatler: 15:00-19:00 (özellikle 16:00-18:00)
- **Öneri:** Gece kapatma + saat bazlı bid adjustment

---

### Demografik Analiz

**Yaş ve cinsiyet gösterim dağılımı:**

| Segment | Gösterim | Pay |
|---------|----------|-----|
| Kadın 35-44 | ~1,337 | %18.10 (ZİRVE) |
| Kadın 25-34 | ~924 | %12.51 |
| Erkek 25-34 | ~841 | %11.39 |
| Kadın 18-24 | ~1,089 | %14.74 |
| Erkek 35-44 | ~826 | %11.18 |
| Kadın 45-54 | ~631 | %8.54 |

- Kadın 35-44 en yüksek gösterim: Bu segment okul çağı çocuğu olan annelere karşılık gelir
- Çocuk müzik eğitimi kararlarını çoğunlukla anneler veriyor — reklam metni bu segmente yönelik değil
- **Öneri:** Kadın 35-44 +%20, Kadın 25-34 +%10 demografik bid

---

### Optimizasyon Puanı

- Mevcut puan: **%58.8** (Düşük — Google standart olarak %80+ önerir)
- Ana eksikler: Reklam takvimi yok, cihaz bid yok, demo bid yok

---

## 2. Öncelik Sırası

### Bugün Yap (30 dakika)
1. **Display ağını duraklat** — Kampanya ayarları → Ağlar → Display işaretini kaldır
2. **Gece reklamlarını kapat** — Reklam takvimi → 23:00-07:00 = kapalı
3. **Cihaz bid** — Mobil -%20, Desktop +%15, Tablet -%80

### Bu Hafta (2-3 gün)
4. **Demografik bid** — Kadın 35-44 +%20, Kadın 25-34 +%10, 65+ -%30
5. **Saat bid** — 16:00-19:00 +%25, 14:00-16:00 +%15
6. **Negatif kelime listesini uygula** — sedam-ads/negatif-anahtar-kelimeler.md
7. **RSA metin güncellemesi** — Anne/çocuk odaklı 3-4 başlık ekle

### 2 Hafta Sonra
8. **Enhanced Conversions** — Test modundan aktif moda geçir
9. **Bütçe artışı** — Display kapatılınca ₺150/gün'e çık
10. **Arama terimleri kontrolü** — Yeni negatif kelime ekle

---

## 3. Başarı Kriterleri (2 Haziran 2026 Audit)

| Metrik | Şu anki | Hedef |
|--------|---------|-------|
| CTR (Search only) | %5.10 → %2.87 karışık | %5+ (Search) |
| Optimizasyon puanı | %58.8 | %75+ |
| Mobil harcama payı | %94.8 | %70-75 |
| Cost per conversion | ₺357 | ₺150 altı |
| Aylık dönüşüm | 2 (7 günlük veri) | 10+ |

---

## 4. Sonraki Audit

**Tarih:** 2 Haziran 2026
**Gerekli export:** Kampanyalar + Cihazlar + Demografi + Arama Terimleri CSV
**Karar noktası:** 30 dönüşüme ulaşınca Target CPA (Smart Bidding) değerlendir
