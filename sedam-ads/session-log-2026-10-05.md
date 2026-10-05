# Session Log — 5 Ekim 2026

4 Ekim takvim görevinin (14 gün mini audit) bir gün gecikmeli oturumu.
Kampanya: `Sedam - Arama - Eylul 2026` (ID 24268863002) · Hesap 880-549-6844

## 0. Veri kaynağı

8 dosya, `C:\Users\ASUS\Downloads\Yeni klasör`, 20 Eyl – 5 Eki 2026:
reklam grubu · anahtar kelime · arama terimleri (iki aralık) · reklam raporu ·
genel bakış kartları ZIP · negatif liste · Dönüşümler ekran görüntüsü.

**Eksik:** değişiklik geçmişi. "Araçlar → Toplu işlemler" altında bulunamadı — menü taşınmış.
Üstteki arama kutusuna `Değişiklik geçmişi` yazmak gerekiyor. Bu yüzden 25 Eylül sonrası
panelde ne yapıldığı dolaylı çıkarımla tespit edildi.

---

## 1. 🔴 Kampanya 2–5 Ekim arası yayında değildi — ÖDEME SORUNU

Zaman serisi:

| Tarih | Tıklama | Gösterim | Maliyet |
|---|---|---|---|
| 29 Eyl Sal | 13 | 81 | ₺127,30 |
| 30 Eyl Çar | 10 | 100 | ₺107,27 |
| **1 Eki Per** | 9 | **59** | ₺106,32 |
| 2 Eki Cum | 0 | 0 | ₺0,00 |
| 3–5 Eki | 0 | 0 | ₺0,00 |

Kampanya durumu "Etkin" görünürken dört gün tek gösterim yok.

**Teşhis kalıbı:** 1 Ekim normal günün yaklaşık yarısında (59 gösterim) kesildi. Bitiş tarihi
olsaydı o gün tam çalışır, sonra sıfırlanırdı — **gün ortasında kesilme ödeme işaretidir.**
Aylık tavan değildi: Eylül toplamı ₺1.770, tavan ₺150 × 30,4 = ₺4.560.

**5 Ekim'de kullanıcı doğruladı: ödeme sorunuymuş, çözüldü.**

Maliyet: sezonun 17 gününün 4'ü kaybedildi (≈₺600 planlanmış harcama yayınlanmadı).

**Ders:** günlük gösterim sıfıra düşerse önce faturalandırmaya bak. Kampanya durumu "Etkin"
kalıyor, panelde hiçbir kırmızı işaret kampanya sayfasında görünmüyor.

---

## 2. Performans (20 Eyl – 1 Eki, 12 aktif gün)

| Metrik | Değer |
|---|---|
| Gösterim | 1.234 |
| Tıklama | 146 |
| TO | %11,83 |
| Ort. TBM | ₺12,85 |
| Maliyet | ₺1.876,35 |
| Günlük ort. | ₺156,36 |
| Dönüşüm (Ads) | 11 |
| Maliyet / dönüşüm | ₺170,58 |
| **Gerçek kayıt** | **0** |

25 Eylül'e göre TO %9,44 → %11,83, TBM ₺17 bandından ₺12,85'e indi. Negatif temizliği işe
yaradı. Trafik kalitesi metrik olarak iyileşti, **iş sonucu değişmedi.**

---

## 3. 🔴 Dönüşüm ölçümü — 11 rakamının içi boş

`Hedefler → Dönüşümler` ekranı:

| İşlem | Kaynak | İzleme durumu | Sayım | Dönüşüm |
|---|---|---|---|---|
| WhatsApp Tıklama | Web sitesi | Etkin | **Hepsini** | **10** |
| Potansiyel müşteri formu gönderimi | Web sitesi | Müdahale gerekiyor | Bir | 1 |
| Form Gönderimi | Web sitesi | Müdahale gerekiyor | Bir | 0 |
| Reklamlardan sesli arama yapma | Reklamlardan Gelen Arama | Kayıt yok | Hepsini | **0** |
| **Tıkla ve ara** | Reklamlardan Gelen Arama | **Kaldırıldı** | Bir | 0 |
| **Kişi** | Web sitesi | **Kaldırıldı** | Bir | 0 |
| | | | **Toplam** | **11** |

Üç sonuç:

**3a. 11 dönüşümün 10'u tek işlemden, hem de `Sayım: Hepsini`.** Aynı kişinin her WhatsApp
tıklaması ayrı sayılıyor. Gerçek kişi sayısı muhtemelen 4-6. `₺170,58/dönüşüm` kişi başı maliyet
değil; gerçek kişi başı ≈ **₺300-450**.
→ **Karar: `Bir`e çevrilecek** (kullanıcı onayladı 5 Ekim).

**3b. Telefon tarafı tamamen kör.** `Tıkla ve ara` **kaldırılmış** — site içi `tel:` tıklamaları
artık hiç sayılmıyor. `Reklamlardan sesli arama yapma` 25 Eylül'de Birincil yapılıp arama süresi
30 sn'ye çekilmesine rağmen hâlâ **0**.

**3c. Seda 5-6 telefon araması aldığını söylüyor, Ads bunların hiçbirini görmüyor.** İki açıklama:
ya aramalar reklam arama uzantısından değil siteden numarayı görüp elle yapıldı (bu durumda
`Tıkla ve ara` kaldırıldığı için ölçülmüyor), ya da organikten geldi. Ayrımı yapacak veri yok —
`Tıkla ve ara` geri kurulmadan bu kör nokta kapanmaz.

---

## 4. 🟡 Asıl teşhis: sorun trafik hacmi değil, temasın kayda dönmemesi

```
146 tıklama
  → ~10-13 temas   (WhatsApp ~4-6 kişi + 1 form + Sedanın 5-6 telefonu)
  → 0 kayıt
```

Tıklamadan temasa dönüş **%7-8** — bu oran sağlıklı. Kırılan halka **temastan kayda** geçiş.

Yani Ads'in satın aldığı trafik kötü değil; temas sonrasında ne olduğu bilinmiyor.
**Kampanyaya yapılacak hiçbir teklif ayarı bunu düzeltmez.**

### Destekleyen kanıt: dönüşüm getiren terimlerin hepsi doğru kalıpta

| Terim | Dönüşüm | Maliyet | Grup |
|---|---|---|---|
| `yan flüt kursu istanbul` | 2 | ₺8,13 | 07 - Nefesli |
| `esenyurt keman kursu` | 2 | ₺22,63 | 05 - Keman |
| `avcılar gitar kursu` | 1 | ₺21,73 | 03 - Gitar |
| `saz kursu` | 1 | ₺18,54 | 06 - Baglama |

Dördü de **konum + branş** kalıbı, niyet net, fiyatlar makul. Yanlış kitle değil.

### Konum israfı var ama sorunu açıklamıyor

Beylikdüzü sorguları ₺157 yedi, 10 tıklama, 0 dönüşüm (`beylikdüzü gitar kursu` ₺75,47 ile
tek başına en pahalı terim). **Kullanıcı 5 Ekim'de Beylikdüzü'nden öğrenci geldiğini doğruladı —
negatif YAPILMADI.** 10 tıklama karar vermek için az örnek.

`elektro gitar kursları` (₺23,66): Sedam elektro gitar veriyor, normal sorgu. Dokunulmadı.

### ❗ Eksik parça

Sedanın 5-6 aramasında ne konuşulduğu alınamadı. Teşhisin son adımı buna bağlı:
hangi branş, kimin için, fiyat sordu mu, konum neresi, nasıl bitti. Ders ücreti de gerekli.

---

## 5. ✅ Negatifler çalışıyor — konu kapandı

- 25 Eylül'ün 15 kelimelik bloğu **yapıştırılmış**, 15'inin hepsi listede ✓
- Liste **196 kelime**
- **26 Eyl – 5 Eki aralığında tek sızıntı yok** — listedeki hiçbir kelime sorgu geçirmemiş

21 ve 25 Eylül'de iki oturum yiyen "negatifler tutmuyor" şüphesi kesin olarak kapandı.
Doğrulama yöntemi tekrar işe yaradı: **raporu daima son değişiklik tarihinden sonrasıyla çek.**

---

## 6. Reklam grubu ekonomisi (12 aktif gün)

| Grup | Göstr. | Tık | TO | Ort. TBM | Maliyet | Pay | Dönş. | ₺/dönş. |
|---|---|---|---|---|---|---|---|---|
| 03 - Gitar | 382 | 42 | %10,99 | ₺14,07 | **₺591,06** | **%31,5** | 2 | **₺295,53** |
| 06 - Baglama | 274 | 38 | %13,87 | ₺11,17 | ₺424,47 | %22,6 | 3 | ₺141,49 |
| 05 - Keman | 231 | 30 | %12,99 | ₺13,05 | ₺391,39 | %20,9 | 3 | ₺130,46 |
| 02 - Cocuk Sezon | 88 | 11 | %12,50 | ₺14,00 | ₺154,00 | %8,2 | **0** | — |
| 04 - Piyano | 172 | 13 | %7,56 | ₺10,54 | ₺137,04 | %7,3 | 1 | ₺137,04 |
| 07 - Nefesli | 71 | 10 | **%14,08** | ₺13,62 | ₺136,16 | %7,3 | 2 | **₺68,08** |
| 01 - Marka | 15 | 2 | %13,33 | **₺21,12** | ₺42,23 | %2,3 | 0 | — |
| 08 - Yetiskin | 1 | 0 | — | — | ₺0,00 | 0 | 0 | — |

- **`07 - Nefesli` ile `03 - Gitar` arasında 4,3 kat verimlilik farkı var** (₺68 vs ₺296).
  Nefesli en az bütçeyi alıyor.
- **`04 - Piyano` alarmı kapandı:** TO %2,82 → %7,56. RSA'ları "Ortalama" gücünde. Müdahale yok.
- **`08 - Yetiskin` hâlâ ölü** (1 gösterim). Sebep RSA değil kelime hacmi — 5 kelimenin 3'ü
  "nadiren yayınlanıyor". İki RSA'sı da "Yetersiz" reklam gücünde. 17 gün kaldığı için
  düşük öncelik.
- **`01 - Marka` TBM ₺21,12** — kendi marka adı için absürt, normali ₺2-5.
- **`02 - Cocuk Sezon`** TO iyi (%12,50) ama ₺154'te 0 dönüşüm.

### RSA durumu
17 etkin reklamın tümü **"Ortalama"** reklam gücünde. Tek istisna `08 - Yetiskin`'in iki reklamı:
**"Yetersiz"**. Reddedilen / uygun olmayan reklam yok.

### Kelime durum uyarıları
- `05 - Keman / "keman dersi"` → **Sınırlı: düşük kalite** (25 Eylül'den beri sürüyor)
- 7 kelime "nadiren yayınlanıyor" (düşük hacim) — zarar vermiyor
- **Duraklatılmış `Reklam grubu 1` içinde 47 kelime duruyor** — etkisiz, temizlik işi

---

## 7. Hesaplanan düzeltme değerleri

### 7a. Cihaz — mevcut ayar tam ters

| Cihaz | Göstr. | Tık | TO | Ort. TBM | Maliyet | **Mevcut** | **Yeni** |
|---|---|---|---|---|---|---|---|
| Cep telefonları | 1.072 | 128 | %11,94 | **₺11,95** | ₺1.529,41 | **-%20** | **0** |
| Bilgisayarlar | 162 | 18 | %11,11 | **₺19,27** | ₺346,94 | **+%15** | **-%35** |
| Tablet / TV | 0 | 0 | — | — | ₺0,00 | -%80 | -%80 (dokunma) |

Masaüstü tıklaması mobilden **%61 pahalı**, TO'su da düşük — ve `+%15` ile destekleniyor.
Mobil ise %61 daha ucuz tıklama üretirken `-%20` ile kısılıyor. 21 ve 25 Eylül'de şüphelenilen
ters çalışma **16 günlük veriyle kesinleşti.**

`-%35` gerekçesi: çarpan `1,15 → 0,65` olur (×0,565). ₺19,27 × 0,565 ≈ **₺10,9** — mobil
seviyesine iner. Sıfırlamak yerine kısmak tercih edildi çünkü cihaz bazlı dönüşüm verisi yok;
18 tıklamanın değeri bilinmiyor.

### 7b. Reklam takvimi — `21-23` bandı ters kısılıyor

Saatlik gösterim (12 aktif gün, 23:00-07:00 kapalı):

| Saat | 07 | 08 | 09 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Göstr. | 23 | 18 | 16 | 41 | 31 | 66 | 58 | 86 | 104 | 99 | 105 | 141 | **161** | 90 | 106 | 89 |

Ham gösterim yanıltıcı — her bant **kendi teklif düzeltmesinin baskısı altında** oluştu.
Düzeltmeden arındırmak için gözlem `(1 + düzeltme)`'ye bölünür:

| Bant | Göstr. | Saat/bant | Gözlenen/saat | Mevcut | **Arındırılmış talep** | **Yeni teklif** |
|---|---|---|---|---|---|---|
| 07-12 | 129 | 5 | 25,8 | -%5 | **27,2** | **-%40** |
| 12-14 | 124 | 2 | 62,0 | 0 | **62,0** | **-%20** |
| 14-16 | 190 | 2 | 95,0 | +%15 | **82,6** | **0** |
| 16-19 | 345 | 3 | 115,0 | +%25 | **92,0** | **+%10** |
| 19-21 | 251 | 2 | 125,5 | +%10 | **114,1** | **+%15** |
| **21-23** | 195 | 2 | 97,5 | **-%20** | **121,9** ← zirve | **+%15** |

**`21-23` gerçek talebin zirvesi ve `-%20` ile kısılıyor.** Tam ters. `07-12` ise talebin
dörtte birini üretirken neredeyse düzeltmesiz duruyor.

Yeni değerlerin talep ağırlıklı ortalaması **+%1,6** — genel TBM'i şişirmiyor, sadece
dağılımı düzeltiyor.

**Gün katmanı bu tur EKLENMEDİ.** Gerekçe: Cuma ve Cumartesi'nin birer geçerli günü var
(2-3 Ekim yayın durmuştu), örnek çok ince. Ayrıca Ads'te ayrı gün katmanı olmadığı için
gün × saat çarpımı 42 satıra çıkıyor — ince veri için pahalı bir işlem. 6 bant "Her gün"
olarak kalır.

Not: Perşembe (74,5 göstr./gün) ve Çarşamba (87) iki günlük veriyle istikrarlı biçimde
ortalamanın altında. 22 Ekim kapanış raporunda tekrar bakılacak.

### 7c. Demografi — düşük öncelik

| Yaş | Göstr. | Pay | Mevcut | Arındırılmış | **Yeni** |
|---|---|---|---|---|---|
| 25-34 | 351 | %30,08 | +%10 | 319 | +%10 (aynı) |
| 35-44 | 345 | %29,56 | **+%20** | 288 | **+%10** |
| 45-54 | 221 | %18,94 | **—** | 221 | **+%10** |
| 18-24 | 158 | %13,54 | — | 158 | — (aynı) |
| 55-64 | 55 | %4,71 | -%20 | 69 | -%20 (aynı) |
| 65+ | 40 | %3,43 | -%30 | 57 | -%30 (aynı) |

`35-44` en büyük desteği alıyor ama arındırılmış talepte ikinci sırada; `45-54` üçüncü sırada
olmasına rağmen hiç düzeltme almıyor. İkisi `+%10`'da eşitlenir.

Cinsiyet **Kadın %57,58 / Erkek %42,59** — dengeli, dokunulmaz.

**Uyarı:** bunlar hacim bazlı, değer bazlı değil. Yaş kırılımlı dönüşüm verisi yok ve zaten
0 kayıt var. **Düşük öncelik** — cihaz ve takvim düzeltmesinden sonra yapılır.

### 7d. Grup TBM'leri

| Grup | Mevcut TBM tavanı | **Yeni** | Gerekçe |
|---|---|---|---|
| 03 - Gitar | ₺18 | **₺12** | Bütçenin %31,5'i, ₺295,53/dönüşüm |
| 07 - Nefesli | ₺18 | **₺22** | ₺68,08/dönüşüm, en yüksek TO, en az bütçe |
| 01 - Marka | ₺18 | **₺6** | Marka kelimesine ₺21,12 TBM absürt |
| 02 - Cocuk Sezon | ₺18 | **₺15** | ₺154'te 0 dönüşüm, TO iyi — izlemede |
| Diğerleri | ₺18 | ₺18 | Dokunma |

### 7e. Teklif stratejisi — **GEÇME** (karar tekrarlandı)

Eşik 30 günde 15+ dönüşüm. 12 günde 11 dönüşüm → 30 günlük tempo ~27, **eşiğin üstünde.**
Buna rağmen karar değişmedi.

**Gerekçe veri değil, sinyal kalitesi:** 11 dönüşümün 10'u `Sayım: Hepsini` ayarlı WhatsApp
tıklaması ve **hiçbiri kayda dönmedi**. Dönüşüm Maks.'a geçmek, akıllı teklifi "WhatsApp'a
basıp kaydolmayan" profili daha çok satın almaya yönlendirir. Değersiz sinyalle beslenen
akıllı teklif bütçeyi hızla yanlış yere yığar.

`Tıklama Maks.` + TBM tavanı ₺18'de kalınır. Yeniden değerlendirme: WhatsApp sayımı `Bir`e
çekildikten ve gerçek kayıt gelmeye başladıktan sonra.

### 7f. Optimizasyon puanı
**%73,7** (25 Eylül'de de %73,7). Birikmiş öneriler bu oturumda okunamadı — panel erişimi
gerekiyor, kullanıcıya bırakıldı. "Bütçe artır" tipi öneriler **reddedilmeli** (0 kayıt varken
harcamayı artırmak yanlış yön).

---

## 8. Panelde yapılacaklar — öncelik sırasıyla

| # | İş | Yer | Öncelik |
|---|---|---|---|
| 1 | Yayının döndüğünü doğrula (ödeme sonrası) | Kampanyalar → bugünkü gösterim | 🔴 |
| 2 | `WhatsApp Tıklama` sayımı `Hepsini` → **`Bir`** | Hedefler → Dönüşümler | 🔴 |
| 3 | Cihaz: mobil `-%20` → **0**, masaüstü `+%15` → **-%35** | Ayarlar → Cihazlar | 🔴 |
| 4 | Reklam takvimi: 6 bandın yüzdelerini 7b tablosuna göre yaz | Ayarlar → Reklam takvimi | 🔴 |
| 5 | Grup TBM'leri: Gitar ₺12, Nefesli ₺22, Marka ₺6, Çocuk ₺15 | Reklam grupları | 🟡 |
| 6 | `Tıkla ve ara` dönüşümünü geri kur (telefon kör noktası) | Hedefler → Dönüşümler | 🟡 |
| 7 | Demografi: 35-44 `+%10`, 45-54 `+%10` | Ayarlar → Demografi | 🟢 |
| 8 | Değişiklik geçmişi CSV'si (arama kutusuna yaz) | — | 🟢 |
| 9 | Optimizasyon önerilerini oku, bütçe artırma önerilerini reddet | Öneriler | 🟢 |

**Reklam takvimi uygulama notu:** tablo sanallaştırılmış, satırlar görünür alana gelmeden
DOM'a girmiyor. Toplu düzenleme: satırları seç → mavi çubuk → `Düzenle → Teklif ayarlamalarını
değiştirin` → Artır/Azalt + yüzde → Uygula. Uygula sonrası tablo bozuk render edebilir,
sayfayı yenile.

---

## 9. Ads dışı — asıl iş burada

₺1.876 harcandı, ~10-13 temas geldi, **0 kayıt**. Teklif ayarları bu tabloyu değiştirmez.

Seda tarafında netleşmesi gerekenler:
1. 5-6 aramada ne konuşuldu — branş, kim için, fiyat sorusu, konum, nasıl bitti
2. Ders ücreti / aylık paket
3. WhatsApp'a yazanların akıbeti (10 tıklama ≈ 4-6 kişi)
4. Kontenjan durumu — doluysa reklamın anlamı yok

Bu dördü olmadan 22 Ekim'e kadar kalan ~₺2.400'lük harcamanın savunması yok.

---

## 10. Sonraki kontrol

- **Kısa vadeli:** yayın döndükten 3 gün sonra — gösterim normale döndü mü, yeni ayarlar
  TBM'i düşürdü mü
- **22 Ekim:** sezon kapanış audit'i (takvimde duruyor) — son kayıt günü, kampanya
  duraklatma kararı, sezon raporu
