# Google Ads Uygulama Kontrol Listesi
Tarih: 19 Mayıs 2026
Kampanya: YENİ

---

## HEMEN YAP (Bugün — 30 dakika)

### 1. Display Ağını Duraklat
- [ ] Google Ads → Kampanyalar → YENİ
- [ ] Ayarlar → Ağlar sekmesi
- [ ] "Google Display Ağı dahil et" kutusunun **isaretini kaldir**
- [ ] Kaydet

**Neden:** Display ağı genel CTR'ı %5.10'dan %2.87'ye düşürdü. Search CTR'ı aslında hala %5+ seviyesinde.
**Beklenen etki:** CTR hemen %5+ seviyesine döner, bütçe sadece kaliteli Search trafiğine akar.

---

### 2. Reklam Takvimi — Gece Kapatma
- [ ] Kampanyalar → YENİ → Ayarlar → Reklam takvimi → Düzenle
- [ ] 23:00-07:00 için teklif düzeltme: **-100%** (= kapalı)
- [ ] Kaydet

**Neden:** Gece 03:00-06:00 arası en düşük gösterim (32-63 gösterim) — tamamen boşa gidiyor.
**Beklenen etki:** Gündüz bütçesi artar, gece harcama sıfırlanır.

---

### 3. Cihaz Bid Adjustment
- [ ] Kampanyalar → YENİ → Cihazlar sekmesi
- [ ] Cep telefonları: **-20%**
- [ ] Masaüstü bilgisayarlar: **+15%**
- [ ] Tabletler: **-80%**
- [ ] Kaydet

**Neden:** Harcamanın %94.8'i mobilde — dengelenmesi gerekiyor. Desktop kayıt formu doldurma için daha uygun.
**Beklenen etki:** 2 hafta içinde mobil pay %70-75'e düşer.

---

## BU HAFTA (2-3 gün)

### 4. Negatif Kelime Listesini Uygula
- [ ] Google Ads → Araçlar → Paylaşılan Kitaplık → Negatif Anahtar Kelime Listeleri
- [ ] Yeni liste oluştur: "Sedam Negatif Listesi"
- [ ] `sedam-ads/negatif-anahtar-kelimeler.md` dosyasındaki kelimeleri yapistir
- [ ] Listeyi kaydet
- [ ] Kampanyalar → YENİ → Anahtar Kelimeler → Negatif Anahtar Kelimeler → Liste Ekle
- [ ] "Sedam Negatif Listesi"ni seç → Uygula

**Neden:** Alakasız aramalar (ISMEK, ücretsiz, Ankara, Kadıköy vb.) bütçeyi tüketiyor.

---

### 5. Demografik Bid Adjustment
- [ ] Kampanyalar → YENİ → Demografi sekmesi
- [ ] Yaş: 35-44 satırı → **+20%**
- [ ] Yaş: 25-34 satırı → **+10%**
- [ ] Yaş: 65+ satırı → **-30%**
- [ ] Cinsiyet: Kadın → **+10%**
- [ ] Kaydet

**Neden:** Kadın 35-44 en yüksek gösterim payı (%18.10) — okul çağı çocuk anneleri.
**Detay:** `sedam-ads/cihaz-bid-ayarlari.md` dosyasına bak.

---

### 6. Saat Bazlı Bid Adjustment
- [ ] Kampanyalar → YENİ → Reklam takvimi
- [ ] 14:00-16:00: **+15%**
- [ ] 16:00-19:00: **+25%**
- [ ] 19:00-21:00: **+10%**
- [ ] 09:00-12:00: **-10%**
- [ ] 21:00-23:00: **-20%**
- [ ] Kaydet

**Neden:** Peak saat 17:00 (1,017 gösterim) — bu saatte rekabetçi olmak kritik.
**Detay:** `sedam-ads/reklam-takvimi.md` dosyasına bak.

---

### 7. RSA Reklam Metinlerini Güncelle
- [ ] Kampanyalar → YENİ → Reklam grupları → Reklamlar
- [ ] Mevcut RSA → Düzenle
- [ ] Başlık ekle: **"Çocuğunuz İçin Müzik Kursu"** (30 karakter)
- [ ] Başlık ekle: **"Güvenli Çocuk Müzik Okulu"** (28 karakter)
- [ ] Başlık ekle: **"5 Yaşından İtibaren Müzik"** (27 karakter)
- [ ] Açıklama ekle: **"Çocuğunuz için profesyonel müzik eğitimi. Piyano, gitar, keman. İlk ders ücretsiz."** (86 karakter)
- [ ] Kaydet

**Neden:** Kadın 35-44 segmenti için çocuk/ebeveyn odaklı başlıklar eklenmemiş.
**Detay:** `sedam-ads/reklam-metni-generator.md` dosyasına bak.

---

## 2 HAFTA SONRA (2 Haziran 2026)

### 8. Enhanced Conversions Dogrula
- [ ] Araçlar → Dönüşümler → Ayarlar
- [ ] Enhanced Conversions durumunu kontrol et
- [ ] "Test modunda" ise → "Aktif" yap
- [ ] Form gönderimi + WhatsApp + Telefon dönüşümlerinin kayıt edildiğini doğrula

---

### 9. Bütçe Artışı
- [ ] Display kapatıldıktan ve Search CTR %4.5+ olunca:
- [ ] Kampanyalar → YENİ → Günlük bütçe
- [ ] ₺100 → **₺150/gün** olarak güncelle
- [ ] 1 hafta sonra Search perfomansı %15+ iyileştiyse → ₺200/gün değerlendir

---

### 10. Arama Terimleri Kontrolü
- [ ] Raporlar → Arama terimleri → Son 14 gün filtrele
- [ ] Dönüşüm getirmeyen ve alakasız terimleri bul
- [ ] Negatif kelime listesine ekle
- [ ] "fiyat" arama terimi dönüşüm getirdi mi kontrol et — getirmediyse negatif yap

---

### 11. Gün Bid Adjustment
- [ ] Kampanyalar → YENİ → Reklam takvimi → Gün görünümü
- [ ] Salı: **+15%**
- [ ] Pazartesi + Perşembe + Cumartesi: **+5%**
- [ ] Pazar: **-10%**
- [ ] Kaydet

---

## BASARI KRITERLERİ (2 Haziran 2026 Audit)

| Metrik | Mevcut | Hedef |
|--------|--------|-------|
| CTR | %2.87 (karışık) | %4.5+ (Search only) |
| Optimizasyon puanı | %58.8 | %75+ |
| Mobil harcama payı | %94.8 | %70-75 |
| Cost per conversion | ₺357 | ₺150 altı |
| Aylık dönüşüm | 2 (7 günlük veri) | 10+ |

---

## Sonraki Audit İçin Gerekli CSV Exportları

Google Ads → Raporlar → özelleştirilmiş rapor:
- [ ] Kampanyalar raporu (maliyet, tıklama, dönüşüm, CTR)
- [ ] Cihazlar raporu
- [ ] Demografi raporu (yaş + cinsiyet)
- [ ] Arama terimleri raporu (son 30 gün)
- [ ] Gün ve saat raporu

**Karar noktası:** 30 dönüşüme ulaşınca → Target CPA Smart Bidding değerlendir
