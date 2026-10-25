# Session Log — 21 Eylül 2026
Konu: `Sedam - Arama - Eylul 2026` ilk 2 günlük performans kontrolü

Önceki oturum: [session-log-2026-09-20.md](session-log-2026-09-20.md)

---

## 0. Veri kaynağı

Tarayıcı otomasyonu kullanılmadı — Chrome'da `sedaninmuzigi@gmail.com` oturumu kapalıydı
(açık olanlar: `amsterdam.520@gmail.com` / Ads 308-826-9254 iptal edilmiş giyim hesabı,
`ibrahim4car@gmail.com` hiç Ads hesabı yok, `s3148615@gmail.com`).
`__e=8805496844` ve `authuser=1` denendi, Google 308'e geri yönlendirdi.

Kullanıcı raporları CSV olarak indirdi → `Masaüstü/Yeni klasör/`:
- `Reklam grubu raporu.csv` (20-21 Eylül, UTF-16)
- `Reklam raporu (1).csv` (20-21 Eylül, UTF-16)
- `Genel_bakış_kartları_excel_csv(2026-09-21_21_13_45).zip` (yalnız 20 Eylül kartları)

**Bu yol tarayıcı gezmekten çok daha hızlı — bundan sonra varsayılan bu olsun.**

---

## 1. Performans

| | 20 Eyl | 21 Eyl (21:13'e dek) | Toplam |
|---|---|---|---|
| Gösterim | 104 | 140 | **244** |
| Tıklama | 9 | 11 | **20** |
| Maliyet | ₺130,18 | ₺220,65 | **₺350,83** |
| Ort. TBM | ₺14,46 | ₺20,06 | **₺17,54** |
| TO | %8,65 | — | **%8,20** |
| Dönüşüm | 0 | 0 | **0** |

20 Eylül'de ilk gösterim **17:00**'de — kampanya o saatte yayına girdi, gün yarım.
İnceleme beklemesi yaşanmadı. Optimizasyon puanı **%94,1**.

### Reklam grubu kırılımı (2 gün)

| Grup | Gösterim | Tıklama | Ort. TBM | Maliyet |
|---|---|---|---|---|
| 03 - Gitar | 76 | 8 | ₺19,07 | **₺152,52** (%43) |
| 05 - Keman | 60 | 4 | **₺20,27** | ₺81,09 |
| 06 - Baglama | 50 | 4 | ₺12,16 | ₺48,62 |
| 02 - Cocuk Sezon | 16 | 2 | ₺19,06 | ₺38,11 |
| 07 - Nefesli | 10 | 2 | ₺15,25 | ₺30,49 |
| 04 - Piyano | 32 | **0** | — | ₺0 |
| 01 - Marka | 0 | 0 | — | ₺0 |
| 08 - Yetiskin | 0 | 0 | — | ₺0 |

---

## 2. TBM tavanı — müdahale edilmedi, bilinçli

Ort. TBM ₺17,54; Keman/Gitar/Çocuk grupları ₺18'in **üstünde**. Hata değil:
teklif düzeltmeleri tavanı çarpıyor. 16-19 saat `+%25` × Avcılar `+%20`
= ₺18 × 1,5 = **₺27 efektif tavan**. Piyasa fiyatı ₺18 üstünde, kampanya sürekli tavanda alıyor.

**Tavan yükseltilmedi.** Tıklama Maks. bütçeyi zaten tüketiyor; tavanı artırmak
tıklama başı maliyeti yükseltip günlük tıklama sayısını düşürür.
₺150 ÷ ₺17,54 ≈ günde 8-9 tıklama, kapasite bu.

---

## 3. RSA durumu: 16/16 **Uygun**

Reddedilen yok, incelemede kalan yok.

| Reklam gücü | Adet |
|---|---|
| Ortalama | 14 |
| **Yetersiz** | **2** — ikisi de `08 - Yetiskin` |

Eski `Reklam grubu 1` duraklatılmış, doğru durumda.

---

## 4. Bütçe aşımı — izlemede

21 Eylül 21:13'te **₺220,65** = günlük bütçenin **%147'si**. 23:00'e kadar ~₺250 kapatır.
Google günde 2x aşırı teslimata izin veriyor (₺300 tavanı) — **fatura hatası değil**.
Aylık tavan doğrulandı: ₺150 × 30,4 = **₺4.560**.

Risk: iki gün üst üste ₺220+ giderse ay ortasında aylık tavana çarpıp reklamlar kısılır.
22 Eylül akşamı tek kontrol noktası bu.

Hesap bildirimi ("günlük harcama sınırı kaldırıldı") **hâlâ okunmadı** — oturum kapalıydı.

---

## 5. ✅ YAPILDI — Negatif listesindeki Türkçe karakter açığı

**Negatif anahtar kelimeler yakın varyantlarla eşleşmez.** Pozitif kelimeler yazım hatası/
aksan varyantını yakalar, negatifler yakalamaz. Liste ASCII yazılmıştı (`ucretsiz`,
`halk egitim`), Türkçe karakterli sorguları geçiriyordu. 137 kelimenin 103'ü ASCII'ydi.

Arama terimleri raporundan dört bağımsız kanıt:

| Listedeki negatif | Geçen sorgu | Sonuç |
|---|---|---|
| `ucretsiz` | `ücretsiz gitar kursu istanbul` + 4 varyant | 8 gösterim |
| `halk egitim` | `halk eğitim keman kursu` | **₺19,90 harcandı** |
| `arnavutkoy` | `arnavutköy keman kursu` | 2 gösterim |
| `arif sag` | `arif sağ saz kursu` | 2 gösterim |

**Aksiyon:** `negatif-anahtar-kelimeler.md` → Bölüm 9 (31 Türkçe ikiz) + Bölüm 10
(`onur art`, `silivri`) eklendi. Liste **137 → 170**. ASCII sürümler silinmedi, ikisi de duruyor.

**Kullanıcı 33 kelimeyi `Sedam - Genel Negatifler` paylaşılan listesine yapıştırdı (21 Eyl).**

Bilerek eklenmeyenler: `büyükçekmece` (Beylikdüzü komşusu), `atakent` (Küçükçekmece içi),
`esenyurt` (hedefte, `-%10` düzeltmeli).

---

## 6. Tespit edildi, müdahale edilmedi (veri yetersiz → 4 Ekim audit'i)

- **Mobil `-%20` ters çalışıyor olabilir.** 20 Eylül cihaz kırılımı:
  mobil 89 gösterim / 9 tıklama / ₺130,18 · masaüstü 15 gösterim / **0 tıklama** · tablet 0.
  Tüm tıklama mobilden geliyor, biz mobili kısıyoruz. Tek günlük veri, dokunulmadı.
- **Demografi kayması.** Gösterimlerin %43,6'sı 25-34 (biz `+10` verdik),
  %19,2'si 35-44 (biz `+20` verdik). Cinsiyet: **kadın %70,2** / erkek %30,9.
- **`04 - Piyano`: 32 gösterim, 0 tıklama.** %8 TO'da 0 tıklama olasılığı ~%7 —
  henüz istatistiksel alarm değil, izlenecek.
- **`08 - Yetiskin` hiç gösterim almadı** ve iki RSA'sı da "Yetersiz". Metinler güçlendirilmeli.
- **`01 - Marka` 0 gösterim.** Kimse markayı aramıyor; yerel işletme için beklenen, sorun değil.

---

## 7. Yarın (22 Eylül) yapılacaklar

1. **Günlük harcama** ₺220'de mi kalıyor, ₺150'ye mi oturuyor — tek kritik kontrol
2. **Hesap bildirimi** "günlük harcama sınırı kaldırıldı" metnini oku (aylık tavan teyidi)
3. Negatif eklemesi sonrası arama terimleri raporunu tekrar çek — `ücretsiz`/`halk eğitim`
   sorguları kesildi mi doğrula
4. 20 tıklamada 0 dönüşüm sürüyorsa açılış sayfası şüphesi devreye girer

## 8. Takip takvimi (20 Eylül'den devir)

- [x] ~~Bugün akşam — gösterim/TBM/harcama kontrolü~~ → bu oturumda yapıldı
- [ ] **22 Eylül** — günlük harcama + bildirim metni
- [ ] **23 Eylül** — arama terimleri 2. tarama, dönüşüm uyarılarının geçtiğini doğrula
- [ ] **27 Eylül** — 15+ dönüşüm varsa Dönüşüm Maksimizasyonu'na geç, bütçe ₺175
- [ ] **4 Ekim** — mini audit: cihaz/demografi/saat düzeltmelerini taze veriyle gözden geçir
- [ ] **22 Ekim** — sezon kapanış audit'i
