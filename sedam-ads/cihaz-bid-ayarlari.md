# Sedam Müzik — Cihaz ve Demografi Teklif Düzeltmeleri

Güncelleme: **5 Ekim 2026**
Veri kaynağı: Genel bakış kartları ZIP — Cihazlar + Demografi (20 Eyl – 5 Eki 2026, 12 aktif gün)
Kampanya: `Sedam - Arama - Eylul 2026` (ID 24268863002)

Uygulama: Kampanyalar → `Sedam - Arama - Eylul 2026` → Ayarlar → Cihazlar / Demografi

---

## Cihaz

| Cihaz | Göstr. | Tık | TO | Ort. TBM | Maliyet | Mevcut | **Yeni** |
|---|---|---|---|---|---|---|---|
| Cep telefonları | 1.072 | 128 | %11,94 | **₺11,95** | ₺1.529,41 | -%20 | **0** |
| Bilgisayarlar | 162 | 18 | %11,11 | **₺19,27** | ₺346,94 | +%15 | **-%35** |
| Tabletler | 0 | 0 | — | — | ₺0,00 | -%80 | -%80 |
| TV ekranları | 0 | 0 | — | — | ₺0,00 | — | — |

### Neden

Mayıs 2026'da "mobil aşırı baskın, dengelensin" diye mobile `-%20`, masaüstüne `+%15`
verilmişti. Eylül-Ekim verisi bunun **ters çalıştığını** gösteriyor:

- Masaüstü tıklaması mobilden **%61 pahalı** (₺19,27 vs ₺11,95)
- Masaüstünün TO'su da daha düşük (%11,11 vs %11,94)
- Yani pahalı ve daha az ilgi çeken cihaz desteklenirken, ucuz ve ilgili cihaz kısılıyor

Şüphe 21 Eylül'de doğdu (tek günlük veri), 25 Eylül'de 6 günle güçlendi, 5 Ekim'de 16 günle
kesinleşti.

### `-%35` nasıl bulundu

Çarpan `1,15 → 0,65` olur, yani ×0,565. `₺19,27 × 0,565 ≈ ₺10,9` — mobil seviyesine iner.

Sıfırlamak yerine kısmak tercih edildi: **cihaz bazlı dönüşüm verisi yok**, 18 masaüstü
tıklamasının değeri bilinmiyor. Tamamen kapatmak geri dönüşü olmayan bir bahis olurdu.

### Sonraki kontrol
Yeni ayardan 1 hafta sonra masaüstü TBM'i ₺11-13 bandına indi mi. İnmediyse `-%50`.

---

## Demografi — düşük öncelik

| Yaş | Göstr. | Pay | Mevcut | Arındırılmış talep | **Yeni** |
|---|---|---|---|---|---|
| 25-34 | 351 | %30,08 | +%10 | 319 | +%10 |
| 35-44 | 345 | %29,56 | **+%20** | 288 | **+%10** |
| 45-54 | 221 | %18,94 | **—** | 221 | **+%10** |
| 18-24 | 158 | %13,54 | — | 158 | — |
| 55-64 | 55 | %4,71 | -%20 | 69 | -%20 |
| 65+ | 40 | %3,43 | -%30 | 57 | -%30 |

Cinsiyet: **Kadın %57,58 / Erkek %42,59** — dengeli, düzeltme yok.
(21 Eylül'deki %70/%30 tek günlük gürültüydü.)

### Neden sadece iki satır değişiyor

"Arındırılmış talep" = gözlenen gösterim ÷ (1 + mevcut düzeltme). Ham gösterim yanıltıcıdır
çünkü her segment kendi düzeltmesinin baskısı altında ölçülür.

Arındırıldığında `35-44` ikinci sırada çıkıyor ama en büyük desteği (`+%20`) alıyor;
`45-54` üçüncü sırada ama hiç düzeltme almıyor. İkisi `+%10`'da eşitlenir.

### ⚠️ Bu tablo hacim bazlı, değer bazlı değil

Yaş kırılımlı **dönüşüm** verisi yok. Üstelik kampanyanın hiç kaydı yok — hangi yaşın
kaydolduğu bilinmediği sürece demografi düzeltmesi tahmindir.

**Cihaz ve reklam takvimi düzeltmelerinden sonra yapılır.** Bu ikisi kanıtlı, demografi değil.

---

İlgili: `reklam-takvimi.md` · `session-log-2026-10-05.md`
