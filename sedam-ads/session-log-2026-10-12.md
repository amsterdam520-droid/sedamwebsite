# Session Log — 12 Ekim 2026

9 Ekim takvim görevinin ("5 Ekim ayarları tuttu mu + kayıt geldi mi") üç gün gecikmeli oturumu.
Kampanya: `Sedam - Arama - Eylul 2026` (ID 24268863002) · Hesap 880-549-6844
**Sezon 22 Ekim'de kapanıyor — 10 gün kaldı.**

## 0. Veri kaynağı

4 dosya, `ADS RAPORLARI/2026-10-12/`, aralık **5–12 Eki 2026**:
reklam grubu raporu · arama terimleri · genel bakış kartları ZIP (15 kart) ·
`Tüm dönüşümler` ekran görüntüsü.

**Uyarı:** dönüşüm ekran görüntüsünün tarih aralığı `20 Eyl – 5 Eki` — yeni dönem değil.
Yine de işe yarıyor, çünkü kritik sütunlar (`İzleme durumu`, `Sayım`, `Birincil/İkincil`)
**tarihten bağımsız, canlı ayarı** gösteriyor.

12 Ekim verisi kısmi gün (rapor 19:59'da çekildi), oran hesaplarında 6–11 Eki tam günleri
kullanıldı.

---

## 1. Özet: 5 Ekim ayarlarının net etkisi negatif

| Metrik | 20 Eyl – 1 Eki (12 gün) | **5 – 12 Eki (8 gün)** | Yön |
|---|---|---|---|
| Gösterim | 1.234 | 1.137 | — |
| Tıklama | 146 | 117 | — |
| TO | %11,83 | **%10,29** | ⬇ kötü |
| Ort. TBM | ₺12,85 | **₺14,68** | ⬆ kötü |
| Maliyet | ₺1.876,35 | ₺1.718,09 | — |
| **Günlük ort.** | ₺156,36 | **₺214,76** | ⬆⬆ |
| Günlük (6-11 Eki tam gün) | — | **₺247,96** | 🔴 bütçenin %165'i |
| **Dönüşüm** | 11 | **4** | ⬇ (beklenen) |

> ⚠️ Bu tabloda ilk olarak "dönüşüm 0" yazılmıştı; arama terimleri kartının `0,00` sütunundan
> yanlış okunmuştu. Panelden doğrulanan rakam **4** — `Sayım: Hepsini → Bir` değişikliğinin
> beklenen etkisi. Ayrıntı §12.

TO ve TBM beklentinin tersine gitti: masaüstü kısılacak, TBM düşecek, dağılım düzelecekti.
**Cihaz ayarı mekanik olarak ters çalıştı** (§2), takvim ve demografi tuttu (§6).

---

## 2. 🔴 Harcama hızı patladı — en acil kalem

| Tarih | Tıklama | Gösterim | Ort. TBM | Maliyet |
|---|---|---|---|---|
| 5 Eki Pzt | 9 | 110 | ₺14,73 | ₺132,58 |
| 6 Eki Sal | 10 | 88 | ₺10,04 | ₺100,36 |
| 7 Eki Çar | 17 | 196 | ₺17,22 | **₺292,68** |
| 8 Eki Per | 21 | 205 | ₺14,28 | **₺299,84** |
| 9 Eki Cum | 14 | 187 | ₺19,01 | ₺266,12 |
| 10 Eki Cmt | 19 | 164 | ₺15,79 | **₺299,97** |
| 11 Eki Paz | 18 | 107 | ₺12,71 | ₺228,79 |
| 12 Eki Pzt (kısmi) | 9 | 80 | ₺10,86 | ₺97,75 |

**Dört gün ₺300 tavanında oturdu.** Google günlük bütçenin 2 katına kadar aşırı teslimata
izin veriyor; ₺150 bütçe için sert tavan ₺300 ve kampanya oraya yapıştı.

### Aylık tavan riski

```
Ekim harcaması (1 Eki ₺106,32 + 5-12 Eki ₺1.718,09) = ₺1.824,41
Aylık tavan ₺150 × 30,4                             = ₺4.560,00
Kalan                                               = ₺2.735,59
13-22 Eki (10 gün) × ₺248/gün                       = ₺2.480,00
```
**Pay ₺255.** Hız biraz artarsa tavana 21 Ekim civarı çarpar ve **sezonun son günleri
karanlık geçer** — son kayıt gününde reklam yayınlanmaz.

### Sebep: mobil `-%20`'nin kaldırılması bir maliyet freniydi

| Cihaz | Teklif ayarı | Gösterim | Tıklama | Maliyet | Ort. TBM |
|---|---|---|---|---|---|
| Cep telefonları | **%0** (eski -%20) | 1.071 | 116 | ₺1.712,81 | **₺14,77** |
| Bilgisayarlar | **-%35** (eski +%15) | 66 | **1** | ₺5,28 | ₺5,28 |
| Tabletler | -%80 | 0 | 0 | ₺0,00 | — |

Mobil TBM **₺11,95 → ₺14,77 (+%24)**. Bu tam olarak `-%20`'nin kalkmasının mekanik etkisi
(`×1,25`). Tıklama/gün 10,7 → 14,5 (+%36) oldu ama **ölçülen dönüşüm 11 → 4** ve
**gerçek kayıt yalnız 1.** Daha pahalı tıklama, daha çok tıklama, aynı sonuç.

Masaüstü ise **aşırı kısıldı**: 18 tıklama → **1**, TO %11,11 → %1,52. ₺5,28'e indi,
pratikte kapandı. Para kazandırmadı — mobil boşluğu fazlasıyla doldurdu.

---

## 3. Ölçüm tablosu — 12 Ekim sabahı görülen hâli

> Bu bölüm oturumun **ilk** teşhisidir. Her iki "arıza" da gün içinde çözüldü:
> `Tıkla ve ara` Etkin yapıldı (ama yanlış tür, §11a-4), site etiketi şüphesi ise
> **çürütüldü** — 5-12 Eki'de 4 dönüşüm kaydedilmiş (§12). Tarihsel kayıt için bırakıldı.

`Tüm dönüşümler` ekranının canlı hâli:

| İşlem | Kaynak | İzleme durumu | Sayım | Birincil | Hedeflere dahil | Dönş. |
|---|---|---|---|---|---|---|
| Potansiyel müşteri formu | Web sitesi | ⚠️ Müdahale gerekiyor | Bir | ✓ | Evet | 1,00 |
| Form Gönderimi | Web sitesi | ⚠️ Müdahale gerekiyor | Bir | ✓ | Evet | 0,00 |
| WhatsApp Tıklama | Web sitesi | ⚠️ Müdahale gerekiyor | **Bir** ✅ | ✓ | Evet | 11,00 |
| Reklamlardan sesli arama yapma | Reklamlardan Gelen Arama | Daha önce kaydedilmiş dönüşüm yok | Hepsini | ✓ | Evet | 0,00 |
| **Tıkla ve ara** | Reklamlardan Gelen Arama | 🔴 **Kaldırıldı** | Bir | ✓ | Evet | 0,00 |
| Kişi | Web sitesi | 🔴 Kaldırıldı | Bir | ✓ | Evet | 0,00 |

### 3a. `Tıkla ve ara` geri kurulmamıştı — gün içinde Etkin yapıldı

5 Ekim logu bu işi `✅ geri kuruldu` diye kapatmıştı. **Panel hâlâ `Kaldırıldı` diyor.**
Değişiklik ya kaydedilmedi ya sonradan geri alındı. Sonuç: **tek kayıt getiren kanal
(telefon) 12 Ekim itibarıyla hâlâ ölçülmüyor.**

`Reklamlardan sesli arama yapma` ise doğru kurulmuş (Birincil ✓, hedeflere dahil ✓) ama
`Daha önce kaydedilmiş dönüşüm yok` diyor — bu, **kampanyada arama öğesinin (call asset)
hiç bulunmadığına** işaret ediyor. Uzantı yoksa o işlem tanım gereği hiç kaydetmez.

### 3b. ~~Site dönüşümleri 8 günde sıfır~~ — ÇÜRÜTÜLDÜ, bkz. §12

İlk okumada "117 tıklama, ₺1.718, 0 dönüşüm" çıkarılmış ve etiket arızası şüphelenilmişti.
**Yanlıştı:** o `0,00` rakamları arama terimleri kartından geliyordu; o kart dönüşümü terim
bazında atfetmiyor. Hesap seviyesi tablo **4,00 dönüşüm** gösteriyor (§12).

`Sayım: Hepsini → Bir` değişikliği 10'u **4'e** indirdi — tam beklenen etki.
Üç web işlemindeki `Müdahale edilmesi gerekiyor` uyarısı yalnız "son X gündür kayıt yok"
demek ve arıza göstergesi değil. **Etiket sağlam, konu kapandı.**

---

## 4. Reklam grubu ekonomisi — bütçe yanlış gruplara kaydı

| Grup | Maliyet | Pay | Tık | TO | Ort. TBM | Önceki pay |
|---|---|---|---|---|---|---|
| 06 - Baglama | **₺613,42** | **%35,7** | 44 | %11,76 | ₺13,94 | %22,6 |
| 03 - Gitar | ₺378,93 | %22,1 | 24 | %8,28 | ₺15,79 | %31,5 |
| 04 - Piyano | **₺326,05** | **%19,0** | 18 | %9,00 | **₺18,11** 🔴 | %7,3 |
| 02 - Cocuk Sezon | ₺158,11 | %9,2 | 12 | %12,50 | ₺13,18 | %8,2 |
| 07 - Nefesli | ₺131,64 | %7,7 | 10 | **%23,26** | ₺13,16 | %7,3 |
| **05 - Keman** | **₺77,09** | **%4,5** | 6 | **%4,96** 🔴 | ₺12,85 | %20,9 |
| 08 - Yetiskin | ₺24,94 | %1,5 | 2 | %40,00 | ₺12,47 | %0 |
| 01 - Marka | ₺7,91 | %0,5 | 1 | %12,50 | ₺7,91 | %2,3 |

Üç kayda değer kayma:

- 🔴 **`04 - Piyano` TBM ₺18,11 — maks. TBM tavanının (₺18) üstünde oturuyor.** Payı
  %7,3 → %19,0'a çıktı, 2,4 kat. TO %9, dönüşüm 0. En hızlı büyüyen gider kalemi.
  (TBM'in tavanı aşması hata değil: teklif düzeltmeleri tavanı çarpıyor.)
- 🔴 **`05 - Keman` çöktü** — kaydı getiren grup. TO %12,99 → **%4,96**, pay %20,9 → %4,5.
  `"keman dersi"` üzerindeki **Sınırlı: düşük kalite** uyarısı 25 Eylül'den beri sürüyor ve
  artık grubu susturmuş görünüyor.
- `07 - Nefesli` TO **%23,26** ile açık ara en iyi, hâlâ bütçenin %7,7'sini alıyor.
- `08 - Yetiskin` ölüydü, 2 tıklama aldı (TO %40) — kelime hacmi sorunu, 10 gün kaldı.

Piyano'nun ₺18,11'i, raporun kapsadığı 5-12 Ekim boyunca tavanın hâlâ **₺18** olduğunu
doğruluyor. Tavan **12 Ekim 19:57'de ₺14'e çekildi** ve panelde doğrulandı (§12) —
etkisi bir sonraki raporda görülecek.

---

## 5. 🟡 Negatif sızıntı geri döndü — Türkçe çekim eki açığı

5 Ekim'de "negatifler çalışıyor, konu kapandı" denmişti. 8 günlük raporda yeni sızıntılar:

| Kelime teması | Maliyet | Tık | Geçen sorgular |
|---|---|---|---|
| `nasıl` | **₺53,21** | 3 | `gitar çalmayı nasıl öğrenirim` · `gitar nasıl calinir` · `6 yaş piyano eğitimi nasıl olmalı` |
| `gitar çalmayı` | **₺36,02** | 2 | `gitar çalmayı nasıl öğrenirim` · `gitar çalmayı öğrenmek` |
| `öğrenme` / `öğreniyorum` / `sıfırdan` | ₺0 | 0 | `kendi kendine saz öğrenme` · `sıfırdan gitar öğrenme` · `gitar öğreniyorum` (20 gösterim) |
| `ne kadar` / `kaç` / `ucretleri` | ₺0 | 0 | `gitar kursları ne kadar` · `keman dersi kaç yaşında başlar` · `klarnet kaç ayda öğrenilir` |
| Rakip adları | ₺0 | 0 | `batuhan saz evi esenyurt bağlama kursu` · `cennet kültür merkezi gitar kursu` · `fon müzik avcılar` (19 gösterim) |
| `halkalı` / `küçükçekmece` | ₺0 | 0 | `halkalı saz kursu` · `küçükçekmece gitar kursu` |

**₺89,23 "kendi kendine öğrenme" niyetine gitti.** Listede `nasıl çalınır` var ama
`çalmayı nasıl öğrenirim` ve `nasıl calinir` (Türkçe karaktersiz) eşleşmiyor —
21 ve 25 Eylül'de tespit edilen çekim eki / ASCII açığının aynısı, yeni varyantlarla.

**Eklenecek (her biri hem Türkçe hem ASCII):**
```
çalmayı nasıl öğrenirim / calmayi nasil ogrenirim
nasıl calinir / nasil calinir / nasıl çalınır
çalmayı öğrenmek / calmayi ogrenmek
kendi kendine / sıfırdan / sifirdan
öğrenme / ogrenme / öğreniyorum / ogreniyorum
nasıl olmalı / nasil olmali
kaç ayda / kac ayda / kaç yaşında / kac yasinda
batuhan saz evi / cennet kültür merkezi / cennet kultur merkezi / fon müzik / fon muzik
```
`ne kadar` ve `ucretleri` **eklenmeyecek** — fiyat sorgusu satın alma niyetidir, ₺0 yedi.
`halkalı` / `küçükçekmece` Sedam oraya hizmet veriyorsa dokunulmaz (Küçükçekmece zaten
`+%5` ile hedefli).

---

## 6. Doğrulanan ve doğrulanmayan ayarlar

| Ayar | Uygulandı mı | Sonuç |
|---|---|---|
| Mobil `-%20 → 0` | ✅ uygulanmış | 🔴 TBM +%24, harcama patladı — **geri alınmalı** |
| Masaüstü `+%15 → -%35` | ✅ uygulanmış | 🟡 aşırı kısıldı (1 tıklama), zararsız |
| Reklam takvimi 6 bant | ✅ uygulanmış | 🟡 bkz. aşağıda |
| Yaş `35-44 +%10`, `45-54 +%10` | ✅ uygulanmış | ✅ `45-54` payı %18,94 → %21,73 ile tepki verdi |
| `WhatsApp Tıklama` sayımı `Bir` | ✅ uygulanmış | — (dönüşüm 0 olduğu için ölçülemedi) |
| **`Tıkla ve ara` geri kurma** | 🔴 **UYGULANMAMIŞ** | panel `Kaldırıldı` diyor |
| **Maks. TBM ₺18 → ₺14** | 🔴 uygulanmamış | Piyano ₺18,11'de |

### Reklam takvimi — 5 Ekim'in "21-23 zirvedir" tezi fazla iddialıydı

Saatlik gösterimi `(1 + düzeltme)`'ye bölerek arındırınca:

| Bant | Gösterim | Gözlenen/saat | Düzeltme | Arındırılmış | Sıra |
|---|---|---|---|---|---|
| 19-21 | 209 | 104,5 | +%15 | **90,9** | 1 |
| 14-16 | 170 | 85,0 | **0** | **85,0** | 2 |
| 21-23 | 189 | 94,5 | +%15 | 82,2 | 3 |
| 16-19 | 269 | 89,7 | +%10 | 81,5 | 4 |
| 12-14 | 121 | 60,5 | -%20 | 75,6 | 5 |
| 07-12 | 179 | 35,8 | -%40 | 59,7 | 6 |

`21-23` bandının payı %15,8 → %16,6 ile ancak kıpırdadı — düzeltme `-%20`'den `+%15`'e
(×1,44) çıkmasına rağmen. Yani o bant **talebin zirvesi değil, ortası.** Gerçek zirve
`19-21`; `14-16` ikinci sırada ve hiç düzeltme almıyor.

**Bu tur takvime dokunulmayacak.** Harcama hızı sorunu varken bant yükseltmek yanlış yön;
fark zaten ±%10 bandında. 22 Ekim kapanış raporuna not düşülür. `07-12` `-%40` ile en
düşük bant olarak doğrulandı ✓.

### Demografi ve konum — müdahale yok

| Yaş | Pay | Düzeltme | Arındırılmış |
|---|---|---|---|
| 35-44 | %30,60 | +%10 | 285 |
| 25-34 | %26,71 | +%10 | 249 |
| 45-54 | %21,73 | +%10 | 203 |
| 18-24 | %14,52 | 0 | 149 |
| 55-64 | %5,26 | -%20 | 68 |
| 65+ | %1,75 | -%30 | 26 |

Sıralama düzeltmelerle tutarlı. Dokunulmaz.

| Konum | Teklif ayarı | Tıklama |
|---|---|---|
| Esenyurt | -%10 | 36 |
| **Beylikdüzü** | **Hiç veri yok (ayar yok)** | **33** |
| Avcılar | +%20 | 28 |
| Küçükçekmece | +%5 | 20 |

Beylikdüzü en çok tıklama alan ikinci konum ve **hiç düzeltme taşımıyor.** Arama terimi
tarafında kümülatif ₺293 / 21 tıklama / 0 dönüşüm. Ama 5 Ekim'de kullanıcı oradan öğrenci
geldiğini doğruladı — **negatif yapılmıyor, ayar da değiştirilmiyor**, veri yetersiz.

---

## 7. ✅ Kampanya kârlı — 2 kayıt, ikisi de telefondan

Kullanıcı aynı gün iki kez bilgi verdi. İkinci bilgi tabloyu çeviriyor:

| | |
|---|---|
| Gerçek kayıt | **2** (1'i 20 Eyl–1 Eki, 1'i 5–12 Eki) |
| Branş | Keman / Baglama |
| Kanal | **İkisi de telefon araması** |
| Ücret | **₺5.500 / ay** (aylık olduğu doğrulandı) |

```
Harcama ₺3.594,44 / 2 kayıt     = CAC ₺1.797
İlk ay cirosu 2 × ₺5.500        = ₺11.000  ->  3,06x
Sezon sonu tahmini ₺6.074 / 2   = CAC ₺3.037  ->  1,81x (ilk ay cirosuyla)
```

Öğrenci birkaç ay kalırsa oran hızla büyüyor. **Bütçe kesilmeyecek, kampanya kapanmayacak.**

### Kanal karşılaştırması — tek çalışan kanal telefon

| Kanal | Temas | Kayıt | Ads ölçümü |
|---|---|---|---|
| **Telefon** | ~7-8 arama | **2** | 🔴 hiç ölçülmüyor |
| WhatsApp | ~4-6 kişi (10 tıklama) | **0** | 11 dönüşüm kaydetti |
| Form | 1 | 0 | 1 dönüşüm |

**Ads'in ölçtüğü tek kanal kaybeden kanal; kazanan kanal hiç ölçülmüyor.**

### Seda'dan hâlâ gerekenler

1. **Kontenjan durumu** — 10 gün kaldı, doluysa harcamanın anlamı yok. Açık tek soru.
2. 5-12 Ekim'de WhatsApp'a yazan oldu mu — 93 tıklamalık WhatsApp bağlantısına karşı
   0 WhatsApp dönüşümü kaydedildi, etiket şüphesi buna bağlı.

---

## 8. Panelde yapılacaklar — öncelik sırasıyla

| # | İş | Yer | Etki |
|---|---|---|---|
| 1 | **Mobil teklif düzeltmesi `0` → `-%20`** (geri al) | arama kutusu → `Cihazlar` | ~₺45/gün |
| 2 | **Maks. TBM sınırı `₺18` → `₺14`** | Ayarlar → Teklif verme | ~₺25/gün |
| 3 | **`Tıkla ve ara`'yı gerçekten geri kur + kaydettiğini doğrula** | Hedefler → Dönüşümler | ölçüm |
| 4 | **Arama öğesi (call asset) var mı — yoksa ekle** | `Öğeler` | ölçüm |
| 5 | **Site etiketi kontrolü** — WhatsApp/form 8 gündür 0 | Ölçüm → Google etiketi | ölçüm |
| 6 | Negatif ekle — §5 listesi, Türkçe + ASCII | Paylaşılan kitaplık → Hariç tutma listeleri | ~₺11/gün |
| 7 | `"keman dersi"` düşük kalite uyarısı — açılış sayfası alakası | 05 - Keman | kazanan grup |

**Durum 12 Ekim akşamı:** 1, 2, 4, 7 **uygulandı.** 3, 5, 6 yapılamadı — §12'de devam.

### ⚠️ Düzeltme: teklif kısmak günlük harcamayı düşürmez

Oturum içinde "1+2+6 günlük ₺248 → ₺165 yapar" denmişti. **Mekanik olarak yanlış.**
`Tıklama Maksimizasyonu` bütçe sınırına kadar harcar; teklif düşünce tıklama **ucuzlar**,
aynı lira daha çok tıklama alır. Günlük harcama ₺215-250 bandında kalır, değişen şey
**verim**. Harcamayı gerçekten düşüren tek kol **günlük bütçedir.**

Bu, 1 ve 2'yi yanlış yapmaz — pahalı kuyruğu kesip lira başına tıklamayı artırıyorlar,
istenen etki de bu. Sadece fatura kalemi beklendiği gibi düşmeyecek.

**Günlük bütçeye dokunulmuyor:** CAC 3,06x ile ₺150 savunulabilir.

### Yapılmayacaklar

| Konu | Neden |
|---|---|
| Teklif stratejisi değişikliği | 8 günde 0 ölçülen dönüşüm — akıllı teklif için veri yok |
| Kelime duraklatma | n=1 kayıtla ayrım yapılamaz; `04 - Piyano` TBM tavanıyla kısılacak |
| Reklam takvimi | ±%10 bandında fark, harcama hızı varken yanlış yön (§6) |
| Masaüstü `-%35` | Aşırı kısılmış ama ₺5,28 harcıyor — düzeltmeye değmez |
| Beylikdüzü negatifi / konum ayarı | Oradan öğrenci geldi, 21 tıklama karar için az |
| `08 - Yetiskin`, `Reklam grubu 1`'deki 47 kelime | 10 gün kaldı |
| Bütçe artırma önerileri | Reddedilecek |

---

## 9. Sonraki kontrol

- **15-16 Ekim (2-3 gün sonra):** günlük harcama ₺165 bandına indi mi, ort. TBM ₺14,68'den
  düştü mü, `Tıkla ve ara` kayıt etmeye başladı mı.
- **22 Ekim — sezon kapanışı.** Tek gerçek başarı kriteri: `Tıkla ve ara` veya
  `Reklamlardan sesli arama yapma` >0 kaydetti mi. Kaydettiyse sezon ölçülebilir bitti.

## 10. Kalıcı dersler

1. **Ads dönüşüm tablosundaki `0` kanalın çalışmadığını değil ölçülmediğini gösterir.**
   Tek gerçek kayıt, panelde 0 yazan telefon kanalından geldi; 10 WhatsApp dönüşümü
   0 kayıt üretti.
2. **Panelde yapıldığı varsayılan ayar bir sonraki oturumda yeniden doğrulanmalı.**
   `Tıkla ve ara` 5 Ekim'de `✅ geri kuruldu` diye kapatıldı, 7 gün sonra hâlâ `Kaldırıldı`.
3. **Negatif teklif düzeltmesi kaldırılırken maliyet etkisi ayrıca hesaplanmalı.**
   Mobil `-%20 → 0` "ters ayarın düzeltilmesi" diye yapıldı; mekanik sonucu `×1,25` teklif
   artışı oldu ve günlük harcamayı %59 yukarı taşıdı. Düzeltme kaldırmak = teklif artırmak.
4. **Tek bantta gösterim payının kıpırdamaması "talep yok" demektir.** `21-23` düzeltmesi
   ×1,44 arttı, pay %15,8 → %16,6'da kaldı. Arındırma tek yönlü kullanılmamalı:
   düzeltme değiştikten sonra payın ne kadar tepki verdiği de ölçülmeli.
5. **`Tıklama Maks.`ta teklif kısmak günlük harcamayı düşürmez, verimi artırır.**
   Bütçe sınırına kadar harcanır; ucuzlayan tıklama daha çok tıklamaya dönüşür.
   Harcama kalemini düşürmek isteniyorsa tek kol günlük bütçedir.

---

## 11. Öğe (varlık) raporu — iki soruyu kapattı, bir yenisini açtı

`Öğe ilişkilendirme raporu`, 5–12 Eki, 46 satır. Dosya: `ADS RAPORLARI/2026-10-12/`.

### 11a. ✅ Arama öğesi VAR ve yayınlanıyor — eksik olan o değil

```
0534 016 48 65 | Telefon | Hesap seviyesi   | Uygun | 334 göstr. | ₺412,11
0534 016 48 65 | Telefon | Kampanya seviyesi | Uygun |   0 göstr. | ₺0,00
```

Telefon numarası 1.137 gösterimin **334'ünde (%29)** yayınlanmış. Hesap seviyesindeki öğe
çalışıyor, kampanya seviyesindeki kopya hiç yayınlanmıyor (normal — biri yeter).

Yani `Reklamlardan sesli arama yapma`'nın 0 olması **uzantı eksikliğinden değil.**

### 11a-2. Çağrı raporlama da etkin — sorun ölçüm ayarı değil, arama biçimi

İlk hipotez "arama raporlaması kapalı" idi. **Yanlış.** `Ayarlar → Hesap ayarları`
ekranı şunu gösteriyor (etiket Türkçe'de farklı adlanmış):

```
Telefon araması üreten reklamlar  ->  Çağrı raporlama etkin
Otomatik etiketleme              ->  Evet
```

Ölçüm altyapısı ayakta. Geriye tek açıklama kalıyor ve kullanıcının ifadesinde duruyor:
kayıtlar **"normal arayarak"** geldi.

| Arama biçimi | Ölçülür mü |
|---|---|
| Reklamın arama butonuna basma | ✅ ölçülebilir — çağrı raporlama etkin, **0 basan olmuş** |
| Sitedeki `tel:` linkine tıklama | ⏳ `Tıkla ve ara` ile ölçülür — hâlâ `Kaldırıldı` |
| **Numarayı görüp elle çevirme** | 🔴 **hiçbir yöntemle ölçülemez** |

Numara 334 gösterimde yayınlandı ama arama butonuna basan olmadı; 117 tıklamanın tümü
başlık ve site bağlantılarına gitti. Sonra site görülüp numara elle çevrildi.

**İki kaydın en az biri yapısal olarak ölçülemez bir yoldan geldi.** `Tıkla ve ara`yı
kurmak hâlâ doğru — site numarasına *tıklayanları* yakalar — ama elle çevirenleri asla.

### 11a-4. 🔴 Asıl bulgu: `Tıkla ve ara` yanlış TÜRDE, site ondan tetiklenemez

Kullanıcı 12 Ekim akşamı `Tıkla ve ara`yı geri yükledi — satır **Etkin** (yeşil) oldu.
Ama uyarı balonu şunu gösterdi:

```
Müdahale edilmesi gerekiyor
⚠ Etiket etkin değil
  Son etkinlik: 15 May 2026 (150 gün önce)
```

Site tarafı incelendi ve **sağlam çıktı.** `index.html` (canlı site ile birebir aynı,
`curl` ile doğrulandı):

```
<script src=".../gtag/js?id=AW-11553345216">   ✓ yüklü
gtag('config', 'AW-11553345216')                ✓
function gtag_report_conversion(url)            ✓ tanımlı (satır 2273)
<a href="tel:+905340164865" onclick="return gtag_report_conversion(...)">  ✓ bağlı
```

WhatsApp etiketi (`dsz5CPm6_qQcEMCdiIUr`) 20 Eyl – 5 Eki'de 11 dönüşüm kaydetti —
**site etiketi canlıda çalışıyor.** Sorun `Tıkla ve ara`ya özel.

Git geçmişi sebebi verdi. `97128ef` · 2 Haziran 2026:

```
fix: tikla-ara conversion ID guncellendi (Potansiyel musteri formu donusumu)
  Eski (Reklamlardan Gelen Arama - calismiyordu): AW-11553345216/hHLBCL2usa0cEMCdiIUr
  Yeni (Web sitesi - Potansiyel musteri formu):   AW-11553345216/X-LoCJfS0bccEMCdiIUr
```

**İki sonuç:**

1. **Sitedeki telefon tıklamaları 2 Haziran'dan beri `Potansiyel müşteri formu gönderimi`
   olarak kaydediliyor.** O işlemin 20 Eyl – 5 Eki'deki **1,00 dönüşümü form değil,
   bir telefon tıklamasıydı.** Form kanalı da hiçbir şey üretmemiş.
2. **`Tıkla ve ara`nın kaynağı `Reklamlardan Gelen Arama`** — o tür yalnız reklamın arama
   butonundan gelen aramaları ölçer ve **Google kendisi tetikler.** Site `gtag` olayıyla
   vurulamaz. Haziran'da "çalışmıyordu" denmesinin sebebi etiketin ölü olması değil,
   **yanlış tür** olması. Geri yüklemek site tıklamalarını ölçmez; **0 kalması normaldir.**

### Doğru kurulum — yeni işlem GEREKMİYOR, yeniden adlandırma yeter

Site iki ayrı etiket kullanıyor (`index.html` doğrulandı):

| Tetikleyen | Etiket | Ads'teki işlem adı | Dönüşüm |
|---|---|---|---|
| `tel:` tıklaması (satır 2035) | `X-LoCJfS0bccEMCdiIUr` | "Potansiyel müşteri formu gönderimi" | 1 |
| Gerçek form (satır 2233) | `yy64CKW__aQcEMCdiIUr` | "Form Gönderimi" | 0 |

Gerçek form **başka** etikete gidiyor. Yani `Potansiyel müşteri formu gönderimi` etiketini
**yalnız telefon tıklamaları** tetikliyor — o 1 dönüşüm gerçekten bir telefon tıklamasıydı,
ve 0 form = kimse form göndermedi. Form kanalı da hiçbir şey üretmemiş.

**Çözüm: `Potansiyel müşteri formu gönderimi` → `Telefon Tıklama` olarak yeniden adlandır**,
kategoriyi **Telefon aramasıyla elde edilen potansiyel müşteriler** yap. `Sayım: Bir` ve
`Birincil` zaten doğru.

Site kodu değişmez, deploy gerekmez, yeni işlem oluşturulmaz, geçmiş veri korunur —
adlandırma düzelince **daha doğru** olur.

### 🚫 Hiçbir dönüşüm işlemi SİLİNMEYECEK

| İşlem | Karar |
|---|---|
| Potansiyel müşteri formu gönderimi | **Yeniden adlandır → `Telefon Tıklama`** + kategori telefon |
| Form Gönderimi | Dokunma — gerçek formu ölçüyor, 0 doğru rakam |
| WhatsApp Tıklama | Dokunma |
| `Tıkla ve ara` | Etkin kalsın. Reklamın arama butonunu ölçer, **0 normal** |
| Reklamlardan sesli arama yapma | Dokunma, aynı tür |
| `Kişi` (Kaldırıldı) | Bırak — site hiç kullanmıyor |

Dönüşüm işlemi kaldırmak etiketi ve ilişkilendirmeyi kopardığı için **bu sorunun
kaynağıydı.** 10 gün kala tekrarlanmaz.

### 🟡 `tel:` linkinde ayrıca gerçek bir açık vardı — düzeltildi

```js
gtag('event', 'conversion', { ..., 'event_callback': callback });
return false;
```

`return false` navigasyonu iptal ediyor, aramayı **yalnız `event_callback` başlatıyordu.**
gtag engellenirse (reklam engelleyici, izleme koruması) callback hiç çalışmaz — kullanıcı
numaraya basar, **hiçbir şey olmaz.** Telefon tek kayıt getiren kanal olduğu için bu sessiz
kayıp pahalı.

12 Ekim'de `index.html`'e `try/catch` + 1 saniyelik `setTimeout` emniyeti eklendi
(çift tetiklemeyi `navigated` bayrağı engelliyor). **Canlıya gitmedi** — dal
`docs/sedam-ads-session-2026-09-25`, deploy `main`'e push ile tetikleniyor
(`.github/workflows/deploy.yml`, gh-pages).

⚠️ `deploy.yml` çalışma kopyasında **silinmiş** (commit edilmemiş). O silme `main`'e
giderse deploy tamamen durur.

### ⚠️ Güvenlik — repo dışı konu

`git remote -v` çıktısında GitHub kişisel erişim token'ı düz metin gömülü
(`github_pat_11CAU3AMA0...`, `.git/config` içinde). İptal edilip yenilenmeli, remote
token'sız hâle çevrilmeli:
```
git remote set-url origin https://github.com/amsterdam520-droid/sedamwebsite.git
```
Kimlik doğrulama Git Credential Manager / `gh auth login` üstlensin.

### 11a-3. Gerçek çözüm: reklama özel telefon numarası

Yalnız reklamlarda kullanılan ayrı bir numara: o numaraya gelen her arama reklam
kaynaklıdır, Google'a bağımlılık yok. Bu sezon için geç — **gelecek sezon öncesi
kurulacak iş.**

Bedava ara çözüm, bugünden işler: **Seda arayanlara "bizi nereden buldunuz" sorsun**,
kayıt defterine tek kolon. 10 günde bile kapanış raporunu kör olmaktan çıkarır.

### 11b. 🔴 Öğe metinleri kaybeden kanala yönlendiriyor

| Öğe | Tür | Göstr. | Tık | TO | Maliyet |
|---|---|---|---|---|---|
| "Kurslarımız — Gitar, piyano, keman, bağlama" | Site bağlantısı | 704 | 104 | %14,77 | ₺1.541,03 |
| **"Ücretsiz Deneme Dersi — WhatsApp'tan hemen randevu al"** | Site bağlantısı | **647** | **93** | %14,37 | ₺1.373,58 |
| "Eğitmenlerimiz — Konservatuvar mezunu" | Site bağlantısı | 511 | 61 | %11,94 | ₺919,00 |
| "Kurslar: Gitar,Piyano,Keman,Bağlama,Klarnet,Yan Flüt" | Snippet | 473 | 32 | %6,77 | ₺441,79 |
| "İlk Ders Ücretsiz. Uzman Eğitmenler..." | Açıklama | 445 | 40 | %8,99 | ₺557,75 |
| "Neden Sedam? — Kişiye özel ders programı" | Site bağlantısı | 360 | 27 | %7,50 | ₺351,56 |
| **`0534 016 48 65`** | **Telefon** | 334 | 29 | %8,68 | ₺412,11 |
| "Müzik Dersi" | Promosyon | 305 | 15 | **%4,92** | ₺216,90 |
| İşletme logosu | Logo | 203 | 16 | %7,88 | ₺205,50 |

(Öğe metrikleri çakışır — aynı tıklama birkaç öğe altında sayılır, toplamları ₺1.718'e
eşit olmaz.)

**İkinci en çok yayınlanan öğe insanları WhatsApp'a gönderiyor.** WhatsApp ~4-6 kişi
ve **0 kayıt** üretti; telefon **2 kayıt / 2**. Metin kazanan kanalı değil kaybedeni
öne çıkarıyor.

**Öneri:** o site bağlantısının ikinci açıklama satırını değiştir —
`WhatsApp'tan hemen randevu al` → `Hemen arayın: 0534 016 48 65`. Tek satır, 10 gün kaldı.

`Promosyon | Müzik Dersi` TO %4,92 ile en zayıf öğe ve süresi 22 Ekim'de doluyor.

### 11c. İki artık — temizlik

- `Sedam Müzik Merkezi | İşletme adı` → **Uygun değil / Onaylanmadı**, iki ayrı satırda
  (5 Eyl 2025 ve 26 Nis 2026). 0 gösterim.
- `Hemen iletişime geç! | https://sedammuzikevi.com.tr/iletisim/` → **eski domain**
  (güncel site `sedammuzik.com`). 0 gösterim, zararsız ama kaldırılmalı.

---

## 12. Panelde yapılan ve doğrulanan işler (tarayıcı oturumu, 12 Eki ~21:00)

Google Ads paneline tarayıcıdan girilip her madde tek tek doğrulandı.

### ✅ Doğrulananlar

| Kontrol | Bulgu |
|---|---|
| Maks. TBM sınırı | `₺14,00`, onay kutusu işaretli — **kaydedilmiş** |
| Mobil teklif düzeltmesi | **`-%20`** — geri alınmış. Masaüstü `-%35`, tablet `-%80` |
| Günlük bütçe | `₺150,00/gün`, kampanya `Etkin / Uygun` |
| Teklif stratejisi | `Tıklama sayısını en üst düzeye çıkarma` |
| `Telefon Tıklama` adlandırması | **Yapılmış.** Kaynak `Web sitesi`, Sayım `Bir`, `Birincil`, hedeflere dahil `Evet` |
| Paylaşılan negatif liste | `Sedam - Genel Negatifler` · **223 kelime · Kampanyalar: 1** → **bağlı** |
| Arama öğesi | `0534 016 48 65`, hesap seviyesi, `Uygun`, 337 gösterim, ₺412,11 |
| Çağrı raporlama | `Hesap ayarları → Telefon araması üreten reklamlar` = **Çağrı raporlama etkin** |
| Otomatik etiketleme | `Evet` |
| Değişiklik geçmişi | **Sol menüde, kampanya kapsamında** — arama kutusuna yazmak gerekmiyor |

### 🔴 5–12 Ekim dönüşüm rakamı düzeltmesi

Oturumun ilk bölümünde "8 günde 0 dönüşüm, etiket bozuldu" denmişti. **Yanlıştı.**
Hesap seviyesi tablo **4,00 dönüşüm** gösteriyor (hepsi `WhatsApp Tıklama`).
Arama terimleri kartı her satırda `0,00` gösterdiği için yanlış okundu — o kart dönüşümü
terim bazında atfetmiyor.

`Sayım: Hepsini → Bir` değişikliği 10'u **4'e** indirdi; tam beklenen etki. **Etiket sağlam,
site ölçümü çalışıyor.** "Tracking kırık" şüphesi kapandı.

### 🔴 Kategori değişikliği YAPILAMIYOR — kalıcı kısıt

`⋮ → Başka bir dönüşüm hedefine geçin` alt menüsünün tam içeriği:

```
Satış:                 Satın alma · Sepete ekleme · Ödeme başlatma · Abone olma
Potansiyel müşteriler: Kaydolma · Randevu rezervasyonu · Kişi · Yol tarifi ·
                       Giden tıklama · Fiyat teklifi isteyin
Diğerleri:             Sayfa görüntüleme · Diğer
```

**`Telefon aramasıyla elde edilen potansiyel müşteri` listede yok.** O kategori yalnız
`Reklamlardan Gelen Arama` kaynaklı işlemlere açık; `Telefon Tıklama`nın kaynağı `Web sitesi`.

**Karar: kategoriye dokunulmadı.** İşlevsel kazanç yok (`Birincil` + hedeflere dahil zaten
doğru, ölçüm çalışıyor); kategori sadece raporlama etiketi. `Kişi`ye taşımak hesapta
bulunmayan yeni bir hedef yaratır ve kampanya bağlantısını (`3/3`) riske atar — sezonun son
10 gününde ölçümü bozma riski kozmetik düzeltmeye değmez.

### 🆕 WhatsApp site bağlantısı — orijinal öneri GEÇERSİZ, yerine ekleme yapıldı

Panelde iki engel çıktı:

1. **Site bağlantısı metni düzenlenemez.** Öğe araç çubuğunda yalnız
   `Kaldır / Duraklat / Etkinleştir / Ekle` var. Metin değiştirmek = öğeyi silip yenisini kurmak.
2. **Reklam metninde telefon numarası Google politikasına aykırı.** Önerilen
   `"Hemen arayın: 0534 016 48 65"` **reddedilirdi.** Numara yalnız arama öğesiyle yayınlanabilir
   — o da zaten çalışıyor.

Bunun yerine **mevcut WhatsApp bağlantısına dokunulmadan** telefon odaklı yeni site bağlantısı
eklendi (politika uyumlu, numara yok):

```
Başlık:      Hemen Arayın                     (12/25)
Açıklama 1:  Telefonla hızlı bilgi alın       (26/35)
Açıklama 2:  Ücretsiz deneme dersi ayarlayın  (31/35)
Nihai URL:   https://sedammuzik.com/#iletisim
Durum:       Beklemede: İnceleniyor (12 Eki 21:17)
```

Gerekçe: WhatsApp bağlantısı 655 gösterim / 95 tıklama / **%14,50 TO** ile en çok trafik üreten
ikinci öğe. Onu yerinden oynatmak yerine 5. site bağlantısı olarak telefon mesajı eklendi;
Google ikisini döndürür. Kampanyanın site bağlantıları: Kurslarımız (717 göstr.) ·
Ücretsiz Deneme Dersi (655) · Eğitmenlerimiz (517) · Neden Sedam? (369) · **Hemen Arayın (yeni)**.

### ⚠️ Oturumda yapılan hata — kayda geçsin

`Ücretsiz Deneme Dersi` site bağlantısı yanlışlıkla **duraklatıldı** (21:13:02) ve
**21 saniye sonra geri etkinleştirildi** (21:13:23). Sebep: öğe araç çubuğundaki buton
`Düzenle` diye eşleşti, gerçekte `Duraklat`tı. Gösterim kaybı yok, durum `Uygun`.
Değişiklik geçmişinde iki `Kampanya öğesi değiştirildi` satırı olarak görünür.

### Negatifler geniş eşlemeli eklendi — düzeltme gerekmiyor

Değişiklik geçmişi: `12 Eki 20:30:47 — "Sedam - Genel Negatifler": 27 negatif geniş eşlemeli
anahtar kelime listeye eklendi`. Talimat `Sözcük Öbeği` idi.

**Sorun değil, hatta daha koruyucu:** geniş negatif, sorgu tüm terimleri içeriyorsa
(sıra önemsiz) bloklar — sözcük öbeğinden daha fazla sorgu kapsar. Tek kelimelik negatiflerde
(`öğrenme`, `sıfırdan`) iki tür pratikte aynı. Bu listede istenmeyen blok üretmiyor.
29 satırın 27'si eklendi; 2'si (`nasıl çalınır` gibi) listede zaten vardı.

### ✅ Madde 7 kapandı — `"keman dersi"` uyarısı kendiliğinden geçmiş

`Kitleler, anahtar kelimeler ve içerikler → Anahtar kelimeler`, 54 kelimenin tamamı yüklendi.
**Düşük kalite uyarısı taşıyan tek kelime `"bağlama dersi"`:**

```
"bağlama dersi" · 06 - Baglama · Sıralı eşleme
Durum: Uygun (Sınırlı) — Nadiren gösteriliyor (düşük Kalite Puanı)
57 gösterim · %7,02 TO · ₺60,09 · 4 tıklama · 0 dönüşüm
```

`"keman dersi"` artık **hiçbir uyarı taşımıyor** — 25 Eylül'den beri açık olan madde
kendiliğinden kapandı. Keman grubunun TO çöküşü (%12,99 → %4,96) kalite puanından değil.

**Sebep tabloda görünüyor: 54 kelimenin hepsinin `Nihai URL`'si `https://sedammuzik.com`** —
yani ana sayfa. Branşa özel açılış sayfası yok, site tek sayfa (`#dersler`, `#egitmenler`,
`#neden`, `#iletisim` yalnız çapa).

**Müdahale yapılmadı.** Kelime düzeyinde `#dersler` çapası vermek kalite puanını değiştirmez
(Google çapayı ayrı sayfa saymaz, yalnız kaydırma pozisyonu). Gerçek çözüm branş bazlı açılış
sayfaları — 10 günde yapılacak iş değil, gelecek sezon notu. Kelime zaten "nadiren
gösteriliyor" ile kısılmış durumda ve ₺60 harcamış.

### ✅ Madde 11c kapandı — temizlik gereksiz, öğeler duraklatılmış kampanyalarda

| Öğe | Kampanya | Durum |
|---|---|---|
| `Hemen iletişime geç!` → `sedammuzikevi.com.tr` (eski domain) | **Campaign #1** | duraklatılmış, 0 gösterim |
| `Müzik Kurslarımız` · `Neden Sedam?` · `Eğitmenlerimiz` · `Deneme Dersi Al` (8 May 2026) | **YENİ** | duraklatılmış, 0 gösterim |
| `Sedam Müzik Merkezi` İşletme adı — *Uygun değil / Onaylanmadı* | Campaign #1 ve YENİ | duraklatılmış, 0 gösterim |

Hiçbiri `Sedam - Arama - Eylul 2026` kampanyasında değil; **halka hiç gösterilmiyor.**
Kaldırmak kozmetik ve kullanıcının sormadığı duraklatılmış kampanyalara dokunmak gerekir —
**yapılmadı.**

### 🔴 Faturalandırma okundu — 2–5 Ekim kesintisi kesin olarak açıklandı

`Faturalandırma → Fatura özeti`:

```
Bakiye                   ₺1.907,48
Sonraki otomatik ödeme   1 Kas  VEYA  bakiye ₺5.000,00'a ulaşınca
Ödeme yöntemi            Visa •••• 0017
Son ödeme                5 Eki · ₺1.849,68 · MANUEL ödeme
Eylül                    net maliyet ₺1.849,68 · ödemeler ₺0,00
```

`Faturalandırma → Faturalandırma ayarları`:

```
Ödeme yöntemleri   ⚠️ Yedek ödeme yöntemi yok
Ödeme yöntemin     Sonradan ödeme (eşik bazlı)
Ödeyen             Sedam Müzik Evi
Google Payments    5529-3404-0858-4515
```

**Teşhis tamamlandı:** Eylül'de ₺1.849,68 maliyet birikti, **Eylül ödemesi ₺0,00** — otomatik
çekim `Visa •••• 0017`'den geçmedi. Yedek ödeme yöntemi olmadığı için ikinci deneme yapılamadı,
1 Ekim gün ortasında yayın kesildi, 5 Ekim'de **manuel ödemeyle** açıldı. 5 Ekim'de kurulan
"gün ortasında kesilme = ödeme" kalıbı doğrulandı ve sebebi netleşti: **yedek yöntem yokluğu.**

#### ⚠️ Aciliyet düzeltmesi

Oturum içinde "son kayıt gününde kesinti sezonu kapatır" denmişti — **aciliyet fazla
gösterilmiş.** Sonraki otomatik ödeme **1 Kasım**, sezondan sonra. Eşik tarafı:
bakiye ₺1.907 + 10 gün × ₺215 ≈ **₺4.057**, ₺5.000 eşiğine çarpmaz.
**Normal hızda sezon içinde ödeme tetiklenmez.**

Risk yalnız şu kuyrukta: harcama ₺300/gün bandına dönerse 10 günde ₺3.000 → bakiye **₺4.907**
→ 21-22 Ekim'de eşiğe değer, otomatik çekim denenir, kart yine geçmezse **tam son kayıt
gününde yayın durur.** Yedek yöntem bu kuyruk riskini kapatır.

**Yapılmadı — yapılamaz.** Yedek ödeme yöntemi eklemek kart bilgisi girmeyi gerektiriyor;
bu Claude'un yapmayacağı işlemler arasında. Kullanıcının yapması gereken, tam yol:
`https://ads.google.com/aw/billing/settings → Ödeme yöntemleri → Yedek ödeme yöntemi ekle`

Ayrıca optimizasyon puanı **%60,3** (5 Ekim'de %73,7) — düşüş büyük ölçüde "bütçe artır" ve
"resim ekle" tipi reddedilmesi gereken önerilerden geliyor, aksiyon alınmadı.

---

## 13. Devreden işler

| # | İş | Durum |
|---|---|---|
| `Tıkla ve ara` geri kurma | ✅ Etkin — ama yanlış tür, §11a-4. 0 kalması normal |
| `Telefon Tıklama` yeniden adlandırma | ✅ yapıldı ve panelde doğrulandı |
| Kategoriyi telefona çevirme | 🚫 **yapılamıyor** — §12, kalıcı kısıt |
| Maks. TBM `₺14` | ✅ doğrulandı |
| Mobil `-%20` | ✅ doğrulandı |
| Negatif ekleme | ✅ 27 kelime eklendi, liste kampanyaya **bağlı** (223 kelime) |
| Çağrı raporlama | ✅ **etkin** — hipotez çürüdü, §11a-2 |
| Site etiketi şüphesi | ✅ **kapandı** — 5-12 Eki'de 4 dönüşüm var, §12 |
| Telefon odaklı site bağlantısı | ✅ `Hemen Arayın` eklendi, incelemede |
| `index.html` `tel:` emniyet zamanlayıcısı | ✅ yazıldı · ⏳ deploy edilmedi (acil değil) |
| **Yedek ödeme yöntemi** | 🔴 **kullanıcı yapacak** — kart bilgisi gerektirir. `/aw/billing/settings`. Kesintinin kesin sebebi bu (§12) |
| `Hemen Arayın` site bağlantısı onayı | ⏳ `Beklemede: İnceleniyor`, ~1 iş günü |
| `"keman dersi"` düşük kalite | ✅ **kapandı** — uyarı geçmiş; tek uyarı `"bağlama dersi"` (§12) |
| Öğe temizliği (eski domain, onaylanmayan ad) | ✅ **kapandı** — duraklatılmış kampanyalarda, 0 gösterim |
| Gelecek sezon: branş bazlı açılış sayfaları | ⏳ 54 kelimenin hepsi ana sayfaya gidiyor |
| **Seda arayanlara "nereden buldunuz" sorsun** | ⏳ ölçümün tek pratik yolu |
| **Kontenjan durumu (Seda)** | ⏳ tek açık soru |
| Onaylanmayan işletme adı + eski domain bağlantısı | ⏳ düşük öncelik, 0 gösterim |
| Gelecek sezon: reklama özel telefon numarası | ⏳ kalıcı çözüm |

### 3 için adımlar

`Hedefler → Dönüşümler → Tüm dönüşümler`. `Tıkla ve ara` satırı `Kaldırıldı`.
Kaldırılmış işlem düzenlenemez; satıra tıklayıp **"Geri yükle" / "Yeniden etkinleştir"**
aranır. Çıkmazsa yeniden kurulur:
`+ Yeni dönüşüm → Web sitesi → Manuel`, ad `Tıkla ve ara`,
kategori **Telefon aramasıyla elde edilen potansiyel müşteriler**, Sayım **Bir**, Birincil.
Sonra **sayfa yenilenip** satırın `Etkin` olduğu görülür — 5 Ekim'de kaydettiği varsayıldı,
bir hafta kaybedildi.

Yeniden kurulursa sitedeki `tel:` linkine etiketin bağlanması gerekir.

### 6 için not

Negatifler **Sözcük Öbeği** eşleşmesiyle, paylaşılan `Sedam - Genel Negatifler` listesine
eklenir. Liste bağlı değilse (`Kampanyalar` sütunu 0) satır seçilip
**"Kampanyalara uygula"** denir. `ne kadar` / `ucretleri` **bilinçli olarak listede yok** —
fiyat sorgusu satın alma niyetidir ve ₺0 harcadı.
