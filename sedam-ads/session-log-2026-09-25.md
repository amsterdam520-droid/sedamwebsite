# Session Log — 25 Eylül 2026
Konu: Kaçan 22-23 Eylül hatırlatıcılarının toparlanması + "0 dönüşüm" teşhisi

Önceki oturum: [session-log-2026-09-21.md](session-log-2026-09-21.md)

---

## 0. Veri kaynağı

21 Eylül'de kararlaştırılan yöntem kullanıldı: kullanıcı panelden indirdi, tarayıcı gezilmedi.
`Masaüstü/Yeni klasör/`:
- `Reklam grubu raporu.csv` (20-25 Eylül)
- `Arama terimleri raporu.csv` (20-25 Eylül, 129 benzersiz terim)
- `Genel_bakış_kartları_excel_csv(2026-09-25_14_06_10).zip`
- `tüm dönüşümler.png` — Hedefler → Dönüşümler ekranı

**Kodlama tuzağı genişledi:** Ads **aynı ZIP içinde** UTF-16 LE ve UTF-8 BOM karıştırıyor.
Sadece UTF-16 denemek kartların yarısını CJK hurdasına çeviriyor — sessiz bozulma, hata vermiyor.
**BOM baytlarına bakarak karar ver:** `\xff\xfe` → utf-16, `\xef\xbb\xbf` → utf-8-sig.

4 gün ölçüm yapılmadı: 22, 23, 24 Eylül'de oturum açılmadı.

---

## 1. Performans (20-25 Eylül, 6 gün)

| | Değer |
|---|---|
| Gösterim | **625** |
| Tıklama | **59** |
| TO | **%9,44** |
| Maliyet | **₺954,65** |
| Ort. TBM | **₺16,18** |
| Dönüşüm | **4,00** |
| Maliyet / dönüşüm | **₺238,66** |

Optimizasyon puanı **%94,1 → %73,7** düştü — birikmiş öneri var, 4 Ekim'de bakılacak.

### Gün bazlı

| Gün | Gösterim | Tıklama | Ort. TBM | Maliyet |
|---|---|---|---|---|
| 20 Eyl Paz (17:00'de başladı, yarım) | 104 | 9 | ₺14,46 | ₺130,18 |
| 21 Eyl Pzt | 162 | 13 | ₺19,27 | **₺250,49** |
| 22 Eyl Sal | 173 | 13 | ₺16,99 | ₺220,91 |
| 23 Eyl Çar | 74 | 11 | ₺15,78 | ₺173,55 |
| 24 Eyl Per | 90 | 10 | ₺14,21 | ₺142,10 |
| 25 Eyl Cum (14:00'e dek) | 22 | 3 | ₺12,47 | ₺37,42 |

### Reklam grubu kırılımı

| Grup | Gösterim | Tıklama | TO | Ort. TBM | Maliyet | Dönüşüm |
|---|---|---|---|---|---|---|
| 03 - Gitar | 194 | 18 | %9,28 | ₺17,14 | **₺308,47** (%32) | 0 |
| 05 - Keman | 121 | 11 | %9,09 | ₺17,90 | ₺196,91 | **2** |
| 06 - Baglama | 151 | 14 | %9,27 | ₺13,18 | ₺184,55 | 0 |
| 02 - Cocuk Sezon | 46 | 6 | %13,04 | ₺17,72 | ₺106,33 | 0 |
| 07 - Nefesli | 35 | 6 | **%17,14** | ₺14,42 | ₺86,51 | **2** |
| 01 - Marka | 7 | 2 | %28,57 | ₺21,12 | ₺42,23 | 0 |
| 04 - Piyano | 71 | 2 | **%2,82** | ₺14,83 | ₺29,65 | 0 |
| 08 - Yetiskin | 0 | 0 | — | — | ₺0,00 | 0 |

---

## 2. ✅ ÇÖZÜLDÜ — "0 dönüşüm" aslında 4 dönüşüm

21 Eylül'de 20 tıklamada 0 dönüşüm görünüyordu. **Takip çalışıyor.** `tüm dönüşümler.png`'den:

| Dönüşüm işlemi | Kaynak | İzleme durumu | Birincil? | Hedefe dahil | Tüm dönş. |
|---|---|---|---|---|---|
| Potansiyel müşteri formu gönderimi | Web sitesi | **Etkin** | Birincil | Evet | **1,00** |
| WhatsApp Tıklama | Web sitesi | Müdahale gerekiyor | Birincil | Evet | **3,00** |
| Form Gönderimi | Web sitesi | Müdahale gerekiyor | Birincil | Evet | 0,00 |
| Reklamlardan sesli arama yapma | Reklamlardan Gelen Arama | Kayıt yok | **İkincil** | **Hayır** | 0,00 |
| Tıkla ve ara | Reklamlardan Gelen Arama | **Kaldırıldı** | Birincil | Evet | 0,00 |
| Kişi | Web sitesi | **Kaldırıldı** | Birincil | Evet | 0,00 |

Site kodu (`index.html`) bu oturumdan önce canlıda doğrulandı — `gtag.js`, `config AW-11553345216`
ve üç dönüşüm etiketi canlıda mevcut. **Site tarafına dokunulmadı, gerek yoktu.**

Etiket eşleşmesi (sayılardan çıkarıldı):
`dsz5CPm6_qQcEMCdiIUr` → WhatsApp Tıklama (3) · `X-LoCJfS0bccEMCdiIUr` → Potansiyel müşteri
formu gönderimi (1) · `yy64CKW__aQcEMCdiIUr` → Form Gönderimi (0)

### 2a. ⚠️ Gerçek kayıp: SERP'ten gelen aramalar sayılmıyor

Kullanıcı 20-25 Eylül arasında **gerçekten arama geldiğini** doğruladı. Ads bunların yalnızca
site içi tıklamalarını görüyor. `Reklamlardan sesli arama yapma` işlemi **İkincil** ve
**"Hesap düzeyindeki hedeflere dahil edildi: Hayır"** — reklam arama uzantısından doğrudan
arayanlar site hiç açılmadığı için site içi `tel:` dönüşümünü tetiklemiyor, bu işlem de
sayıma girmiyor. Gerçek dönüşüm sayısı 4'ten yüksek.

**Arama varlığı mevcut ve çalışıyor — ama ölçülmüyor.** `Öğeler → Öğeler → Ara`:

| Numara | Tür | Seviye | Durum | Oluşturma | Tıklama | Gösterim | TO | Ort. TBM | Maliyet |
|---|---|---|---|---|---|---|---|---|---|
| 0534 016 48 65 | Ara | Hesap | Uygun | 10 Oca 2025 | **14** | 137 | %10,22 | ₺12,58 | **₺176,13** |

**14 tıklama** arama varlığından geldi — kampanyanın 59 tıklamasının **%24'ü**. Harcamanın
₺176,13'ü (%18) buraya gitti. `Reklamlardan sesli arama yapma` işlemi ise **"Daha önce
kaydedilmiş dönüşüm yok"** diyor: 14 tıklamaya rağmen **tek bir arama dönüşümü kaydedilmemiş**.

İkincil olması yalnız "Dönüşümler" sütununu etkiler; "Tüm dönş." de 0 olduğuna göre sorun
sayımda değil **kayıtta**.

### Teşhis zinciri — üç hipotez elendi, dördüncüsü doğru çıktı

| # | Hipotez | Sonuç |
|---|---|---|
| 1 | Site kodu bozuk | ✗ Canlı site doğrulandı, üç etiket de yerinde |
| 2 | İşlem `İkincil`, sayıma girmiyor | ✗ `İşlem optimizasyonu: Birincil işlem` |
| 3 | Çağrı raporlama kapalı | ✗ `Hesap ayarları → Çağrı raporlama: Açık` |
| 4 | **Arama süresi eşiği çok yüksek** | ✅ **`Arama süresi: 60 saniye`** |

Dönüşüm işlemi ayarları (ID `6985905580`, oluşturma 10.01.2025):
`Değer 1` · `Sayım: Her dönüşüm` · **`Arama süresi: 60 saniye`** · `Tıklama dönüşümü aralığı: 30 gün` ·
`İlişkilendirme: Veriye dayalı`

**14 arama tıklamasının hiçbiri 60 saniyeyi aşmamış.** Müzik kursu sorgusu ("kurs var mı,
ücret ne, hangi günler") tipik olarak 35-45 saniye sürer — eşik gerçek aramaların üstünde kalmış.

**Aksiyon: `Arama süresi` 60 → 30 saniye.** Geçmişi geri getirmez, o 14 arama kalıcı kayıp;
sezonun kalan 27 günü ölçülebilir hâle gelir.

Yan doğrulamalar (hesap ayarları): `Otomatik etiketleme: Evet` · `Geliştirilmiş dönüşümler
kaydediliyor` (site kodundaki `user_data` gerçekten çalışıyor) · `Müşteri verisi şartları:
Kabul edildi` · `Telefon araması dönüşüm işlemi` doğru işleme bağlı.

Açık bırakılanlar (bilinçli): `Telefon araması kaydetme` — KVKK kapsamında arayanı
bilgilendirmeden çağrı kaydı riskli, ihtiyaç arama **sayısı**, içeriği değil.
`Arama ayrıntılarını yönlendirme` — üçüncü taraf sağlayıcı yok.

**Kullanıcı 20-25 Eylül'de gerçekten arama geldiğini doğruladı. Kayıp büyük ihtimalle bu 14 tıklama.**
Gerçek dönüşüm 4 değil, 4 + bu aramaların bir kısmı. Maliyet/dönüşüm ₺238,66'dan çok daha düşük.

### 2b. Dikkat: isimlendirme yanıltıcı

Telefon tıklaması `Potansiyel müşteri formu gönderimi` adlı işleme yazıyor, gerçek form ise
`Form Gönderimi`ne. Rapor okurken karıştırmaya açık.

### 2c. `Form Gönderimi` 6 günde 0

59 tıklamada hiç form doldurulmamış. WhatsApp (3) ve telefon (1) tercih ediliyor.
Form ya görünmüyor ya da uzun. 4 Ekim'de açılış sayfası incelenecek.

---

## 3. ✅ Bütçe alarmı kapandı — müdahale edilmedi

21 Eylül'de ₺220,65/gün (bütçenin %147'si) endişe yaratmıştı. 4 tam günün ortalaması
**₺196,76** ama **trend net aşağı**: ₺250 → ₺221 → ₺174 → ₺142. Son iki tam gün ortalaması **₺157,83**.

Aylık tavan ₺150 × 30,4 = **₺4.560**.

- **Eylül:** 20-25'te ₺954,65. Kalan 5 güne ~₺160 → ay toplamı ≈ **₺1.755**. Tavanın çok altında.
- **Ekim:** Sezon 22 Ekim'de bitiyor, yani 22 gün. ₺4.560 ÷ 22 = **günlük ₺207'ye kadar yer var.**
  Mevcut trend ₺160 civarı — rahat geçer.

**Karar: günlük bütçeye dokunulmadı.** Planın "₺190 üstü ise düşür" eşiği aylık tavana 22 Ekim'den
önce çarpma riskine dayanıyordu; hesap o riskin olmadığını gösteriyor.

Hesap bildirimi ("günlük harcama sınırı kaldırıldı") **hâlâ okunmadı** — ekran görüntüsü gelmedi.
Bütçe matematiği sorunsuz çıktığı için önceliği düştü.

---

## 4. ⚠️ KISMEN AÇIK — Liste bağlı, kaçak sebebi netleşmedi

**Oturum içinde doğrulandı:** `Sedam - Genel Negatifler` listesinde **184 kelime** var ve
`Sedam - Arama - Eylul 2026` kampanyasına **ekli**. "Liste bağlı değil" hipotezi elendi.

Yan bulgu: bu depodaki `negatif-anahtar-kelimeler.md` **170** kelime izliyor, Ads'te **184** var.
İki kaynak senkron değil — **dokümanda yazan bir kelimenin Ads listesinde olduğu varsayılamaz.**

21 Eylül'de 33 Türkçe karakterli negatif listeye yapıştırıldı.
20-25 Eylül arama terimleri raporunda o kelimeler **hâlâ görünüyor**:

| Negatif | Sorgu sayısı | Gösterim | Maliyet |
|---|---|---|---|
| `ücretsiz` | **10 farklı sorgu** | **22** | ₺14,84 |
| `halk eğitim` | 1 | 2 | ₺19,90 |
| `arnavutköy` | 1 | 2 | ₺0,00 |
| `arif sağ` | 1 | 2 | ₺0,00 |

**Kesin değil.** Rapor 20-25 Eylül'ü toplu veriyor, tarih segmenti yok; bu gösterimlerin
eklemeden önce (20-21 Eyl) mi sonra mı olduğu ayırt edilemiyor. İki yön:

- **Kaçak lehine:** 21 Eylül logunda `ücretsiz` **8 gösterim / 5 varyant** idi. Şimdi
  **22 gösterim / 10 varyant** — aradaki 14 gösterim eklemeden sonraya işaret ediyor.
- **Kaçak aleyhine:** `halk eğitim keman kursu` maliyeti 21 Eylül'deki ile **birebir aynı**
  (₺19,90) — o tıklama eklemeden önce olmuş. `arnavutköy` ve `arif sağ` da 2'de sabit kalmış.

### ✅ Ayırt edici test yapıldı — negatifler ÇALIŞIYOR

22-25 Eylül arama terimleri raporu (93 benzersiz terim, ₺253,93) ayrıca çekildi — yani
eklemeden **sonrası**. Sonuç:

| Negatif | 20-25 aralığında | 22-25 aralığında |
|---|---|---|
| `ücretsiz` (10 sorgu) | 22 gösterim | **0** |
| `halk eğitim` | 2 gösterim | **0** |
| `arnavutköy` | 2 gösterim | **0** |
| `arif sağ` | 2 gösterim | **0** |

**Tamamı 20-21 Eylül'e aitmiş.** 21 Eylül akşamı yapıştırılan 33 kelime tuttu.
Kaçak yoktu; toplu rapordaki tarih karışıklığı yanılttı.

**Ders:** arama terimleri raporunu **her zaman son değişiklik tarihinden sonrasıyla** çek.
Toplu aralık, düzeltmeden önceki ve sonraki gösterimleri tek satırda birleştirip sahte alarm üretir.

### Yine de geçen küçük sızıntılar (22-25, hepsi ₺0 — tıklama almadı)

| Sorgu | Gösterim | Neden geçti |
|---|---|---|
| `gitar nasıl çalınır`, `flüt nasıl çalınır`, `bağlama nasıl çalınır` | 7 | `nasıl çalınır` bu **dokümanda** var ama Ads listesinde yok — senkron açığı |
| `online yan flüt dersi`, `online bağlama` | 3 | `online ders` / `online kurs` sıralı eşleşme; kelime sırası farklı |
| `flüt çalmayı öğreniyorum` | 1 | Bölüm 11.2 henüz Ads'e girilmedi |
| `udemy saz kursu` | 1 | Bölüm 11.1 henüz Ads'e girilmedi |

Hiçbiri tıklama almadı, maliyet sıfır. Aciliyeti düşük ama TO'yu hafifçe seyreltiyorlar.

### 22-25'te para yiyen yeni sorgular

- **`flüt calma` ₺18,06** — öğrenme niyeti, negatif adayı (Bölüm 11.3'te var, Ads'e girilmeli)
- **`kabak kemane kursu` ₺16,94** — Sedam kabak kemane veriyor mu? Vermiyorsa negatif
- **`avcılar bateri kursu` ₺11,14** — Sedam bateri veriyor mu? Vermiyorsa negatif
- `sıfırdan saz öğrenme` ₺12,28 — **negatif DEĞİL**, gerçek başlangıç seviyesi talebi
- `baglama kursu veren yerler` ₺20,80 — gerçek talep, kalsın
- `sedam müzik merkezi` ₺42,23 / 2 tıklama — kendi markası, ₺21 TBM pahalı (madde 5d)

### Yeni negatif adayları (öğrenme/video içeriği arayanlar)

Bu oturumda tespit edilen, listede olmayan boşa harcama: **₺76,18** (harcamanın %8'i).

`udemy` (₺23,38) · `flüt calma` (₺18,06) · `nasıl çalınır` · `öğreniyorum` · `eğitim videoları` ·
`online ... dersi` · `ders 1`

`negatif-anahtar-kelimeler.md` Bölüm 11 olarak eklendi — **her biri ASCII + Türkçe çift sürümle.**

---

## 5. Tespit edildi, 4 Ekim'e bırakıldı (kapsam dışı)

Kapsam bu oturumda "kaçanlar + 27 Eylül hazırlığı" olarak sınırlandı. Bulgular not edildi:

### 5a. Cihaz düzeltmesi ters çalışıyor — artık kanıtlı

| Cihaz | Gösterim | Tıklama | TO | Ort. TBM | Maliyet |
|---|---|---|---|---|---|
| Cep telefonu | 522 | 50 | **%9,58** | **₺14,80** | ₺740,09 |
| Bilgisayar | 103 | 9 | %8,74 | **₺23,84** | ₺214,56 |
| Tablet / TV | 0 | 0 | — | — | ₺0,00 |

Masaüstü tıklaması mobilden **%61 pahalı** ve TO'su düşük. Mobile hâlâ `-%20` veriliyorsa
tam ters yönde çalışıyor. 21 Eylül'deki tek günlük şüphe 6 günlük veriyle doğrulandı.

### 5b. Saat bantları gerçek talebe uymuyor

| Bant | Gösterim | Pay | Mevcut teklif |
|---|---|---|---|
| 07-12 | 57 | %9,1 | -%5 |
| 12-14 | 60 | %9,6 | 0 |
| 14-16 | 118 | %18,9 | +%15 |
| 16-19 | 139 | %22,2 | +%25 |
| 19-21 | 130 | %20,8 | +%10 |
| **21-23** | **121** | **%19,4** | **-%20** ← ters |

Zirve saat **19:00 (78 gösterim)**, ardından **15:00 (66)** ve **22:00 (64)**.
`21-23` bandı `16-19` ile neredeyse aynı hacimde ama `-%20` ile kısılıyor. Üstelik bu dağılım
**zaten -%20 baskısı altında** oluştu — gerçek talep daha yüksek.

### 5c. Demografi

| Yaş | Pay | Mevcut düzeltme |
|---|---|---|
| 25-34 | %30,95 | +10 |
| 35-44 | %30,61 | +20 |
| 45-54 | %19,05 | — |
| 18-24 | %10,71 | — |

Cinsiyet **Kadın %55,61 / Erkek %44,73** — 21 Eylül'deki %70/%30 dengelendi, o gün tek günlük
gürültüymüş. 45-54 (%19) düzeltmesiz duruyor, bakılmalı.

### 5d. Grup bazlı

- **`04 - Piyano`: 71 gösterim, 2 tıklama, TO %2,82.** Kampanya ortalaması %9,44 — piyano onun
  üçte biri. Artık istatistiksel alarm; RSA metni veya kelime alaka sorunu.
- **`08 - Yetiskin` 6 günde de 0 gösterim — sebep RSA değil, KELİME HACMİ.** Anahtar kelime
  raporu grubun 5 kelimesinin de 0 gösterim aldığını, üçünün **"Uygun değil — nadiren
  yayınlanıyor"** (düşük arama hacmi) olduğunu gösteriyor: `yeni başlayanlar gitar kursu`,
  `yetişkinler için gitar dersi`, `yetişkin piyano dersi`. Metin yazmak bu grubu kurtarmaz;
  **daha geniş kelime** gerek (`yetişkin müzik kursu`, `40 yaşında gitar öğrenmek` gibi).
- **`01 - Marka` ₺21,12 TBM ile 2 tıklama = ₺42,23.** Kendi marka adına ₺21 TBM çok pahalı;
  marka kelimesi normalde ₺2-5 olur. Teklif düzeltmeleri marka grubunu da çarpıyor olabilir.
- **`03 - Gitar` harcamanın %32'sini alıyor, 18 tıklamada 0 dönüşüm.** En büyük kalem, getirisi yok.

### 5d-2. Anahtar kelime raporu (22-25 Eylül) — kelime seviyesi

4 günde: 369 gösterim · 38 tıklama · TO %10,30 · ₺584,30 · **4 dönüşüm** · ₺146,08/dönüşüm.
**Dört dönüşümün hepsi 22-25 Eylül'de geldi** — 20-21 Eylül'de sıfırdı.

| Kelime | Gösterim | Tıklama | TO | Maliyet | Dönüşüm |
|---|---|---|---|---|---|
| `gitar kursu` | 80 | 7 | %8,75 | **₺103,46** | 0 |
| `bağlama kursu` | 42 | 5 | %11,90 | ₺69,08 | 0 |
| `keman kursu` | 40 | 6 | **%15,00** | ₺90,10 | **2** |
| `saz kursu` | 36 | 4 | %11,11 | ₺54,57 | 0 |
| `gitar dersi` | 34 | 3 | %8,82 | ₺52,49 | 0 |
| `avcılar müzik kursu` | 24 | 3 | %12,50 | ₺55,95 | 0 |
| `piyano kursu` | 22 | 2 | %9,09 | ₺29,65 | 0 |
| `bağlama dersi` | 21 | 1 | %4,76 | ₺12,28 | 0 |
| `keman dersi` | 13 | 1 | %7,69 | ₺20,70 | 0 |
| `piyano dersi` | 12 | **0** | %0,00 | ₺0,00 | 0 |
| `flüt dersi` | 8 | 1 | %12,50 | ₺18,06 | 0 |
| `sedam müzik merkezi` | 8 | 2 | %25,00 | ₺42,23 | 0 |
| `klarnet kursu` | 7 | 1 | %14,29 | ₺12,26 | 0 |
| **`yan flüt kursu`** | 4 | 1 | **%25,00** | **₺8,13** | **2** |

**`yan flüt kursu`: ₺8,13'e 2 dönüşüm = dönüşüm başı ₺4,07.** Hesabın en verimli kelimesi,
ama yalnız 4 gösterim almış. `gitar kursu` ₺103,46 ile en pahalı kalem, 0 dönüşüm.

### Kelime durumu uyarıları

- **`keman dersi` → "Sınırlı: düşük kalite".** Kalite puanı düşük; açılış sayfası alakası veya
  reklam metni uyumu zayıf. Dönüşüm getiren `keman kursu`nun kardeşi olduğu için önemli.
- **8 kelime "Uygun değil — nadiren yayınlanıyor"** (düşük arama hacmi): `gitar dersi avcılar`,
  `sedam avcılar`, `sedam muzik`, `keman dersi avcılar`, `bağlama dersi avcılar` ve
  `08 - Yetiskin`'in üç kelimesi. Bunlar yer kaplıyor, zarar vermiyor; hacim gelirse açılırlar.
- Duraklatılmış `Reklam grubu 1` içinde hâlâ 11 kelime duruyor — etkisiz, temizlik işi.

### 5e. Dönüşüm getiren terimler

| Terim | Dönüşüm | Maliyet | Grup |
|---|---|---|---|
| `esenyurt keman kursu` | 2 | ₺22,63 | 05 - Keman |
| `yan flüt kursu istanbul` | 2 | **₺8,13** | 07 - Nefesli |

İkisi de **konum + branş** kalıbında ve ucuz. `07 - Nefesli` en yüksek TO'ya (%17,14) ve en ucuz
dönüşüme sahip ama en az bütçeyi alıyor (₺86,51). Gitar/Baglama'dan Nefesli/Keman'a kaydırma adayı.

---

## 6. 27 Eylül kararı — ön cevap: **GEÇME**

Eşik: 30 günde **15+ dönüşüm** varsa `Tıklama Maks.` → `Dönüşüm Maks.`, bütçe ₺175.

6 günde 4 dönüşüm. 27 Eylül'de kampanya 8 günlük olacak → beklenen ~5-6 dönüşüm.
**15 eşiğinin çok altında.** Akıllı teklif bu veriyle açlıktan kötü çalışır.

**Karar: Tıklama Maks.'ta kal, bütçe ₺150'de kalsın. Teklif stratejisi kararı 4 Ekim'e ötelendi.**

27 Eylül oturumu kısa geçebilir — tek yapılacak, 4. maddedeki negatif liste bağlantısının
doğrulanması (o güne kadar yapılmadıysa).

---

## 7. Bu oturumda PANELDE yapılan değişiklikler

| # | Değişiklik | Durum |
|---|---|---|
| 1 | `Reklamlardan sesli arama yapma` → **Birincil işlem** | ✅ yapıldı |
| 2 | Aynı işlemin **`Arama süresi` 60 sn → 30 sn** | ✅ yapıldı |
| 3 | 15 kelimelik negatif bloğu → `Sedam - Genel Negatifler` | ⏳ yapıştırılacak, liste 184 → **199** olmalı |

Bütçe, teklif stratejisi, cihaz/saat/demografi düzeltmeleri ve grup TBM'lerine **dokunulmadı** —
bilinçli, kapsam dışıydı.

### Yapıştırılacak 15 kelime

```
bateri
kabak kemane
udemy
coursera
nasıl çalınır
nasil calinir
nasıl öğrenilir
nasil ogrenilir
videosu
videoları
videolari
videolar
ders 1
ders 2
ders 3
```

`bateri` ve `kabak kemane`: kullanıcı 25 Eylül'de Sedam'ın bu ikisini **vermediğini** doğruladı.
`kabak kemane`, `keman`ı engellemez — negatifler tam kelime eşleşir, `kemane` ≠ `keman`.

### ⚠️ Bölüm 11'den geri alınan öneri

İlk taslakta `çalma`, `öğreniyorum`, `öğrenmek istiyorum` da negatif önerilmişti — **iptal.**
`sıfırdan saz öğrenme` (₺12,28), `gitar çalma kursu`, `keman çalmayı öğrenmek istiyorum`
gerçek müşteri sorgularıdır. ₺18'lik tek tıklama için gerçek talebi kesmek kötü takas.
Ayrımı yapan kelime `çalma` değil, **`nasıl`** ve **`video`** — ikisi de blokta var.

---

## 8. Açık sorular

- **Davul / perküsyon veriliyor mu?** Bateri verilmediği doğrulandı ama davul ayrı enstrüman;
  halk müziği kurslarında bağlamayla birlikte sık görülür. Sorulmadan negatif eklenmesin.
- **`online ders` / `online kurs` listede kalsın mı?** 20 Eylül'den beri açık. Sedam online
  ders veriyorsa çıkarılmalı. `online yan flüt dersi` ve `online bağlama` 22-25'te geçti (₺0).
- Hesap bildirimi ("günlük harcama sınırı kaldırıldı") hâlâ okunmadı — bütçe matematiği
  temiz çıktığı için önceliksiz.

---

## 9. Takip takvimi

- [x] ~~22 Eylül — günlük harcama + bildirim metni~~ → kaçtı, 25 Eylül'de toparlandı (bildirim hariç)
- [x] ~~23 Eylül — arama terimleri 2. tarama~~ → kaçtı, 25 Eylül'de yapıldı, **negatifler temiz çıktı**
- [x] ~~Negatif listenin kampanyaya bağlılığı~~ → 184 kelime, bağlı, doğrulandı
- [x] ~~`Reklamlardan sesli arama yapma` Birincil~~ → yapıldı
- [x] ~~Arama süresi eşiği~~ → 30 sn'ye çekildi
- [ ] **27 Eylül** — kısa teyit oturumu:
      (a) liste 199 kelime mi, (b) arama dönüşümü akmaya başladı mı, (c) teklif stratejisi **GEÇME**
- [ ] **4 Ekim** — mini audit: cihaz (5a), saat bantları (5b), demografi (5c),
      Piyano/Yetiskin/Marka (5d), kelime seviyesi (5d-2), bütçe kaydırma (5e)
- [ ] **22 Ekim** — sezon kapanış audit'i

---

## 10. Oturum özeti

Üç alarmın ikisi yanlış çıktı, biri gerçekti.

| Alarm | Sonuç |
|---|---|
| Bütçe aşımı (21 Eyl'den devir) | ✅ Yanlış — harcama ₺250'den ₺142'ye indi, tavana yer var |
| "0 dönüşüm" | ✅ Yanlış — 4 dönüşüm vardı, rapor okuma hatası |
| Negatifler tutmadı | ✅ Yanlış — rapor tarih aralığı yanılttı |
| **Telefon kanalı ölçülmüyor** | ⚠️ **Gerçek** — 60 sn eşiği, 14 arama tıklaması kayıp |

Teşhiste üç hipotez boşuna kovalandı (site kodu / liste bağlantısı / çağrı raporlaması).
Ortak sebep: **toplu tarih aralığı ve yerel doküman ile panel arasındaki kayma.**
Bu iki tuzak memory'ye kalıcı olarak yazıldı.
