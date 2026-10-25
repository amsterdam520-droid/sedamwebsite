# Sedam Müzik — Eylül 2026 Kayıt Sezonu Google Ads Planı
Tarih: 19 Eylül 2026
Durum: Kampanya Haziran 2026'dan beri kapalı (3 ay duraklama)
Son veri: `audit-2026-06-02.md` — 30 günde 2.945,52 TL / 358 tıklama / 36 dönüşüm / 81,82 TL dönüşüm başı

---

## 0. Durum Özeti

Kayıt penceresi 15 Eylül - 22 Ekim (afişte duyurulan son kayıt tarihi). Bugün 19 Eylül — pencerenin ilk haftası kaçtı, kalan 33 gün yılın en değerli trafiği. Kampanya 3 aydır kapalı olduğu için Smart Bidding geçmişi bayat; doğrudan Hedef EBM ile açmak öğrenme fazını uzatır ve ilk günlerde bütçeyi yakar. Plan: kademeli açılış.

**Bütçe:** 150 TL/gün → 175 TL/gün → 200 TL/gün (aşamalı)
**Ana dönüşüm:** WhatsApp (Haziran'da 36 dönüşümün 29'u)
**Kapalı kalacak:** Display ağı, Performance Max

---

## 1. YAYINA ALMADAN ÖNCE (bugün, ~45 dakika)

### 1.1 Dönüşüm takibi doğrulaması — ATLAMA

Haziran'da tıkla-ara dönüşümü 18 gün boyunca sessizce ölü kaldı ve bunu ancak audit'te fark ettik. Aynısı olmasın.

- [ ] `index.html` içinde gtag kodu ve 3 dönüşüm ID'si yerinde mi (form, WhatsApp, tıkla-ara)
- [ ] sedammuzik.com canlı sitede kontrol: `gtag` yüklü mü, `dataLayer` dolu mu, `gtag_report_conversion` fonksiyonu tanımlı mı
- [ ] Web3Forms form gönderimi çalışıyor mu (test formu gönder)
- [ ] Google Ads → Hedefler → Dönüşümler: WhatsApp **Birincil**, Form **Birincil**, Sesli arama **İkincil**
- [ ] Gelişmiş dönüşümler (Enhanced Conversions) test modundan **aktif** moda alındı mı
- [ ] Dönüşüm eylemlerinin hiçbirinde "Etkin değil" / "Son 7 gün kayıt yok" kalıcı uyarısı yok

### 1.2 Negatif anahtar kelime listesi güncellendi mi

- [ ] `negatif-anahtar-kelimeler.md` içindeki **Bölüm 8 — Eylül 2026 sezon negatifleri** hesap seviyesi listeye eklendi
  Yol: Araçlar → Paylaşılan kitaplık → Negatif anahtar kelime listeleri → mevcut liste → Düzenle

### 1.3 Hesap ayarları

- [ ] Kampanya → Ayarlar → Ağlar: **Arama ortakları KAPALI**, **Görüntülü ağ KAPALI**
- [ ] Konum hedefleme tipi: **"Hedef konumlarımdaki kişiler"** (varsayılan "ilgi duyan kişiler" bölge dışı israf yapıyor)
  Yol: Ayarlar → Konumlar → Konum seçenekleri
- [ ] Dil: Türkçe + (varsayılan olarak gelen) İngilizce kalabilir

---

## 2. KAMPANYA YAPISI

Tek Arama kampanyası, reklam grubu başına tek tema. Tüm anahtar kelimeler **sıralı eşleme** (`"..."`) ile başlayacak; geniş eşleme sezon başında kontrolsüz harcar.

| # | Reklam grubu | Anahtar kelimeler (sıralı eşleme) |
|---|---|---|
| 1 | Marka | "sedam müzik", "sedam müzik merkezi", "sedam avcılar" |
| 2 | Çocuk / Sezon | "çocuk müzik kursu", "müzik kursu avcılar", "çocuklar için müzik dersi", "çocuğum için müzik kursu", "avcılar müzik okulu" |
| 3 | Gitar | "gitar kursu avcılar", "gitar dersi avcılar", "gitar kursu", "elektro gitar dersi" |
| 4 | Piyano | "piyano kursu avcılar", "piyano dersi avcılar", "piyano kursu", "çocuk piyano dersi" |
| 5 | Keman | "keman kursu avcılar", "keman dersi", "çocuk keman kursu" |
| 6 | Bağlama | "bağlama kursu avcılar", "bağlama dersi", "saz kursu" |
| 7 | Nefesli + Yaylı (düşük hacim) | "klarnet kursu", "yan flüt kursu", "flüt dersi" |
| 8 | Yetişkin | "yetişkinler için müzik kursu", "yeni başlayanlar gitar kursu", "yetişkin piyano dersi" |

**Grup 2 (Çocuk/Sezon) Eylül'ün en değerli grubu** — en yüksek bid ve en iyi reklam metni buraya.

- [ ] 8 reklam grubu oluşturuldu
- [ ] Her grupta yalnız o temanın anahtar kelimeleri var (tema karışımı kalite skorunu düşürür)
- [ ] Marka grubu ayrı ve düşük bid ile (ucuz savunma)

---

## 3. TEKLİF STRATEJİSİ — KADEMELİ AÇILIŞ

| Aşama | Gün | Strateji | Günlük bütçe |
|---|---|---|---|
| 1. Isınma | 0-7 | Tıklama Sayısını En Üst Düzeye Çıkar, **maks. TBM 18 TL** tavanı | 150 TL |
| 2. Öğrenme | 8-21 | Dönüşümleri En Üst Düzeye Çıkar (hedef EBM'siz) | 175 TL |
| 3. Optimizasyon | 22+ | Hedef EBM = **70 TL** | 200 TL |

- [ ] Aşama 1 ile yayına alındı
- [ ] Öğrenme fazında (ilk 7-10 gün) bid/hedef **değiştirilmeyecek** — bu dönemin metrikleri yanıltıcıdır
- [ ] Aşama 3'e geçiş şartı: son 30 günde en az 30 dönüşüm. Yoksa Aşama 2'de kal.

Maks. TBM tavanı 18 TL, Haziran'daki 13,46 TL ortalama TBM'in üstünde bırakıldı — sezonda rekabet arttığı için tavanı oraya sıkıştırmak gösterim kaybettirir.

---

## 4. HEDEFLEME VE TEKLİF DÜZELTMELERİ

Haziran verisinden geliyor, doğrulanmış. Kampanya seviyesinde uygulanacak (reklam grubu değil).

### 4.1 Konum
Yol: Ayarlar → Konumlar

| Konum | Düzeltme | Gerekçe (Haziran) |
|---|---|---|
| Avcılar | **+%20** | 16 dönüşüm, 47 TL/dönüşüm, %17,39 oran — en iyi |
| Küçükçekmece | +%5 | Orta performans |
| Beylikdüzü | %0 | Nötr |
| Esenyurt | **-%10** | 116 TL/dönüşüm — en pahalı |

### 4.2 Cihaz
Yol: Kampanya → Cihazlar

| Cihaz | Düzeltme |
|---|---|
| Mobil | -%20 |
| Masaüstü | +%15 |
| Tablet | -%80 |

Haziran'da harcamanın %94,8'i mobildeydi; bu düzeltme bütçeyi dengeleyip masaüstü form doldurmalarını açıyor.

### 4.3 Demografi
Yol: Kitleler → Demografi

| Segment | Düzeltme | Gerekçe |
|---|---|---|
| Kadın 35-44 | **+%20** | En yüksek gösterim payı (%18,1) — okul çağı çocuğu olan anneler |
| Kadın 25-34 | +%10 | İkinci segment |
| 65+ | +%10 | Sürpriz: en ucuz dönüşüm (31,85 TL), en yüksek oran (%22,22) |
| 45-54 | +%10 | 64 TL/dönüşüm |
| 18-24 | +%5 | 98 TL/dönüşüm — pahalı |
| Bilinmiyor | **-%50** | 321 TL/dönüşüm |

### 4.4 Gün ve saat
Yol: Ayarlar → Reklam takvimi

**Saat:**
- 23:00-07:00 → **KAPALI** (-%100)
- 16:00-19:00 → **+%25** (gösterim zirvesi, 17:00 = 1.017 gösterim)
- 14:00-16:00 → +%15
- 09:00-12:00 → -%10
- 21:00-23:00 → -%20
- Diğer saatler → %0

**Gün:**
- Cumartesi +%20 · Pazar +%15 · Salı +%5 · Çarşamba -%15 · diğerleri %0

**Eylül'e özel test:** Okul çıkış saati 15:00-17:00 aralığına ek +%10. 2 hafta sonra veriye bakıp kalıcı yapılacak veya geri alınacak.

- [ ] Konum düzeltmeleri girildi
- [ ] Cihaz düzeltmeleri girildi
- [ ] Demografi düzeltmeleri girildi
- [ ] Reklam takvimi (saat + gün) girildi
- [ ] Gece 23:00-07:00 kapalı doğrulandı

---

## 5. REKLAM METİNLERİ

Tam metin seti: `rsa-metinleri-eylul-2026.md`

- [ ] Her reklam grubuna **2 adet RSA** eklendi (Google A/B için minimum 2 ister)
- [ ] Her RSA'da 15 başlık + 4 açıklama dolu (eksik varlık = düşük reklam gücü)
- [ ] Sezon başlığı **Konum 1'e sabitlendi** (pin): "Eylül Kayıt Dönemi Başladı"
- [ ] Görünen URL yolu: `sedammuzik.com/Avcilar/Muzik-Kursu`
- [ ] Reklam gücü en az "İyi" (Mükemmel'i kovalamak için pin'leri kaldırma — sezon mesajı sabit kalsın)

---

## 6. REKLAM VARLIKLARI (ASSET)

Yol: Varlıklar → Varlık ekle

- [ ] **Site bağlantıları (4 adet):** Kurslarımız · Eğitmenlerimiz · Ücretsiz Deneme Dersi · İletişim
- [ ] **Açıklama metni (callout):** İlk Ders Ücretsiz · Uzman Eğitmenler · Bireysel Program · Avcılar Merkez · 5 Yaştan İtibaren · Hafta Sonu Dersleri
- [ ] **Yapılandırılmış snippet:** Başlık "Kurslar" → Gitar, Piyano, Keman, Bağlama, Klarnet, Yan Flüt
- [ ] **Promosyon varlığı:** "Eylül Kayıt Dönemi — Ücretsiz Deneme Dersi", bitiş tarihi 22 Ekim 2026 (afişteki son kayıt tarihiyle aynı olmalı)
- [ ] **Arama (call) uzantısı:** mevcut, 07:00-23:00 ile sınırlandı
- [ ] **Konum uzantısı:** Google Business Profile hesaba bağlı mı — yerel aramada kritik
- [ ] **Görsel varlığı:** afiş promptundan çıkan 1200x628 + `google-ads-gorseller/kare/` içindeki mevcut enstrüman görselleri

---

## 7. TAKVİM

| Tarih | Gün | İş |
|---|---|---|
| 19 Eylül | 0 | Dönüşüm doğrulaması → negatifler → yapı + metinler → 150 TL ile YAYINA AL |
| 22 Eylül | 3 | Arama terimleri ilk taraması. Bariz israf terimler negatife. |
| 26 Eylül | 7 | Aşama 2'ye geç (Dönüşüm Maksimizasyonu), bütçe 175 TL |
| 3 Ekim | 14 | Mini audit: dönüşüm maliyeti, grup bazlı performans, saat/konum verisi |
| 10 Ekim | 21 | Aşama 3'e geç (Hedef EBM 70 TL) — 30 dönüşüm şartı sağlandıysa. Bütçe 200 TL |
| 22 Ekim | 33 | Sezon kapanış audit'i. Bütçe kademeli normale çekilir. |

**Haftalık rutin (her Pazartesi):** Arama terimleri raporu → yeni negatifler → `negatif-anahtar-kelimeler.md` güncelle.

---

## 8. BAŞARI KRİTERLERİ

| Metrik | Haziran 2026 | Eylül hedefi |
|---|---|---|
| Dönüşüm başı maliyet | 81,82 TL | **< 70 TL** |
| Aylık dönüşüm | 36 | **70+** |
| Search CTR | %5,1 → %2,87 (Display karışık) | **%5+** |
| Ortalama TBM | 13,46 TL | 13-16 TL (sezonda artması normal) |
| Optimizasyon puanı | %58,8 | **%75+** |
| Mobil harcama payı | %94,8 | %70-80 |

---

## 9. YAPMAYACAKLARIMIZ (bilinçli kararlar)

- **Display ağı açılmayacak.** Haziran: 846 TL harcama, 0 dönüşüm.
- **Performance Max kurulmayacak.** Günlük bütçe 250 TL'yi aşmadan PMax bütçeyi arama kampanyasından çalar. Ekim ortasında yeniden değerlendirilecek.
- **Geniş eşleme kullanılmayacak.** Sezon başında geniş eşleme = kontrolsüz harcama.
- **Fiyat reklam metnine yazılmayacak.** Fiyat arayan trafik dönüşmüyor; konuşma WhatsApp'ta başlasın.
- **Öğrenme fazında müdahale edilmeyecek.** İlk 7-10 gün elleme.
