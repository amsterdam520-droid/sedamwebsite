# Sedam Müzik - Cihaz ve Demografik Bid Ayarları
Güncelleme: 19 Mayıs 2026
Veri kaynağı: Cihazlar + Demografi CSV (19 Nis - 18 May 2026)

## Google Ads'e Uygulama
Kampanyalar → YENİ → Ayarlar → [Cihazlar] ve [Demografi]

---

## Cihaz Bid Adjustment

| Cihaz | Mevcut Harcama | Mevcut Pay | Yeni Teklif | Gerekçe |
|-------|---------------|-----------|------------|---------|
| Cep telefonları | ₺2,246.09 | %94.8 | **-20%** | Aşırı baskın — dengelenmeli |
| Bilgisayarlar | ₺101.07 | %4.3 | **+15%** | Düşük pay — kayıt formu doldurma masaüstünde daha kolay |
| Tabletler | ₺22.68 | %0.9 | **-80%** | Neredeyse sıfır — minimize et |

**Uygulama Adımları:**
1. Kampanyalar → YENİ → Cihazlar sekmesi
2. "Mobil" satırında teklif düzeltme: **-20%**
3. "Masaüstü" satırında: **+15%**
4. "Tablet" satırında: **-80%**
5. Kaydet

**Önemli Not:** Mobil -%20 ile başla. 2 hafta sonra şunu kontrol et:
- Mobil CVR > Desktop CVR ise → mobil'i -%10'a çek
- Desktop CVR > Mobil CVR ise → desktop'u +%20'ye çıkar

---

## Demografik Bid Adjustment

| Segment | Gösterim Payı | Yeni Teklif | Gerekçe |
|---------|--------------|------------|---------|
| Kadın 35-44 | %18.10 | **+20%** | Zirve trafik — okul çağı çocuk anneleri |
| Kadın 25-34 | %12.51 | **+10%** | İkinci yüksek kadın segmenti |
| Erkek 25-34 | %11.39 | **+5%** | Anlamlı trafik, küçük destek |
| Erkek 35-44 | %11.18 | **+5%** | Potansiyel baba segmenti |
| Kadın 18-24 | %14.74 | +0% | Yüksek gösterim ama düşük satın alma niyeti |
| 55-64 tüm cinsiyet | %5-6 | **-20%** | Düşük potansiyel |
| 65+ tüm cinsiyet | %2-3 | **-30%** | Çok düşük potansiyel |

**Uygulama Adımları:**
1. Kampanyalar → YENİ → Demografi sekmesi
2. "Yaş" ve "Cinsiyet" kolonlarını göster (sağ üstten sütun ekle)
3. Her segment için bid adjustment gir
4. Kaydet

**Not:** Google Ads demografi bid'i yaş ve cinsiyet kombinasyonu olarak girmeni gerektirmeyebilir.
Önce yaş bazlı, sonra cinsiyet bazlı ayrı ayrı girilebilir.

---

## Beklenen Etki (2 Hafta İçinde)

- Mobil harcama payı: %94.8 → %70-75'e düşer
- Desktop görünürlüğü artar — kayıt formu CVR'i yükselebilir
- Kadın 35-44 segmentine daha fazla reklam gösterilir
- Toplam maliyet aynı kalır, kalite artar
