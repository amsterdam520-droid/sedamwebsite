# Sedam Ads — Oturum Logu
**Tarih:** 2026-05-03  
**Konu:** Google Ads optimizasyonu, website iyileştirme, Gelişmiş Dönüşümler sorunu

---

## Tartışılan Konular

1. Google Ads kampanya performans analizi (19 Nis — 2 May 2026)
2. Ekran görüntüsündeki "Gelişmiş Dönüşümlerde ayar sorunları" uyarısı
3. NotebookLM kurulumu ve session log sistemi

---

## Güncel Metrikler

| Cihaz | Tıklama | Gösterim | Dönüşüm | Harcama |
|-------|---------|----------|---------|---------|
| Mobil | 75 | 1.357 | 2 Kayıt | 672 TL |
| Masaüstü | 5 | 190 | 0 | 42 TL |
| **Toplam** | **80** | **1.569** | **2** | **714 TL** |

- Dönüşüm başı maliyet: 336 TL
- Kampanya öğrenme süreci: ~5 gün kaldı

---

## Alınan Kararlar ve Yapılan Değişiklikler

### Kod Değişiklikleri (index.html)
- ✅ Form'a email alanı eklendi
- ✅ Form'a enstrüman dropdown eklendi (Gitar/Piyano/Bağlama/Keman/Flüt/Klarnet/Diğer)
- ✅ Form'a seviye seçimi eklendi (Başlangıç/Orta/İleri)
- ✅ **Gelişmiş Dönüşümler için** `gtag('set', 'user_data', {...})` kodu eklendi — email/telefon `form.reset()`'ten önce okunup Google'a geçiriliyor
- ✅ MusicSchool schema markup eklendi (SEO + kalite skoru)
- ✅ Select CSS stilleri eklendi

### Reklam Metinleri (reklam-metinleri.md)
- ✅ 6-7 başlıktan 15 başlığa çıkarıldı (her enstrüman grubu)
- ✅ 2 açıklamadan 4 açıklamaya çıkarıldı
- ✅ Güçlü CTA'lar eklendi: "İlk Ders Ücretsiz", "Kontenjan Dolmadan Kayıt Ol"
- ✅ Lokasyon varyantları eklendi: Esenyurt, Küçükçekmece, Avrupa Yakası
- ✅ Her grup için 10 anahtar kelimeye çıkarıldı
- ✅ Cihaz teklif önerisi eklendi (Mobil +%10, Masaüstü -%20, Tablet -%80)

### NotebookLM Kurulumu
- ✅ Google hesabı NotebookLM skill'e bağlandı
- ✅ "Sedam Google Ads" notebook kütüphaneye eklendi (ID: sedam-google-ads)
- ✅ Session log sistemi kuruldu (Stop hook + memory)

---

## Panelde Yapılması Gerekenler (Bekleyen)

1. **Gelişmiş Dönüşümler → Otomatik etkinleştir**
   - Araçlar → Dönüşümler → WhatsApp Tıklama → Talimatları İnceleyin
   - Araçlar → Dönüşümler → Form Gönderimi → Talimatları İnceleyin
   - Her ikisinde "Otomatik" seç

2. **Cihaz teklifleri:**
   - Mobil: +%10
   - Masaüstü: -%20
   - Tablet: -%80

3. **Reklam metinlerini Google Ads'e gir** (reklam-metinleri.md'den kopyala)

4. **Reklam takvimi:** Gece 00-06 kapat

5. **Lokasyon ayarı:** "Bu konumdaki veya düzenli ziyaret eden" yap

---

## Enhanced Conversions Test Sonucu (Tag Assistant)

Tag Assistant ile doğrulandı — **KOD ÇALIŞIYOR** ✅
- user_data.email → form'dan alınıp gönderiliyor
- user_data.phone_number → form'dan alınıp gönderiliyor
- conversion event doğru ID ile ateşleniyor
- Google Ads uyarısı 24-48 saat içinde kalkacak

## Sonraki Oturumda Kontrol Edilecekler

- Gelişmiş Dönüşümler uyarısı kalktı mı? (24-48 saat sonra)
- Kampanya öğrenme bitti mi (5 gün)?
- Yeni reklam metinleri girildi mi?
- Dönüşüm başı maliyet düştü mü?
- Cihaz teklif ayarları yapıldı mı?

---

*Sonraki review önerisi: 10 Mayıs 2026*
