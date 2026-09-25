# Sedam Müzik - Reklam Takvimi Ayarları
Güncelleme: 19 Mayıs 2026
Veri kaynağı: Gün_ve_saat CSV (19 Nis - 18 May 2026)

## Google Ads'e Uygulama
Kampanyalar → YENİ → Ayarlar → Reklam takvimi → Düzenle

---

## Saat Bazlı Bid Adjustment

| Saat | Gösterim | Teklif Düzeltme | Gerekçe |
|------|----------|-----------------|---------|
| 07:00-09:00 | Orta | +0% (normal) | Sabah arama |
| 09:00-12:00 | Düşük-Orta | -10% | İş saati, düşük niyet |
| 12:00-14:00 | Orta | +0% | Öğle vakti |
| 14:00-16:00 | Yüksek | +15% | Öğleden sonra, artıyor |
| 16:00-19:00 | EN YÜKSEK | +25% | Pikk saat (17:00 = 1,017 gösterim) |
| 19:00-21:00 | Yüksek | +10% | Akşam, hala aktif |
| 21:00-23:00 | Düşük | -20% | Geç akşam, azalıyor |
| 23:00-07:00 | Çok düşük | KAPAT (-100%) | Boşa harcama — kapalı tut |

**Uygulama Adımları (Saat):**
1. Kampanyalar → YENİ → Ayarlar → Reklam takvimi
2. "Düzenle" butonuna tıkla
3. Her saat dilimine yukarıdaki bid % gir
4. 23:00-07:00 için "-100%" yaz (bu kapatma anlamına gelir)
5. Kaydet

---

## Gün Bazlı Bid Adjustment

| Gün | Gösterim | Teklif Düzeltme | Gerekçe |
|-----|----------|-----------------|---------|
| Salı | 2,230 | +15% | Haftalık zirve |
| Pazartesi | 1,441 | +5% | Güçlü başlangıç |
| Perşembe | 1,383 | +5% | Orta-Yüksek |
| Cumartesi | 1,404 | +5% | Hafta sonu aktif |
| Çarşamba | 1,048 | +0% | Normal |
| Cuma | 983 | +0% | Normal |
| Pazar | 873 | -10% | En düşük gün |

**Not:** Gün bazlı bid adjustment bazı hesaplarda ayrı "Gün ve saat" panelinde olabilir.
Bulamazsan reklam takviminde günlere özel saatler ekleyerek simüle edebilirsin.

---

## Uygulama Notu

- Tüm değişiklikler kampanya seviyesinde yapılmalı (ad group değil)
- Değişiklikler 24 saat içinde aktif olur
- İlk 2 hafta sonra saat/gün performansını tekrar kontrol et
- Yüksek dönüşüm saatleri farklılaşırsa bid'leri güncelle

## Beklenen Etki

- Gece bütçe tasarrufu: Günlük bütçenin tahminen %10-15'i gündüze kayar
- Peak saatlerde görünürlük artar
- CPC artabilir (rekabet yüksek saatlerde) ama CVR de yükselir
