# Sedam Müzik Merkezi — Google Ads Oturum Notları
**Tarih:** 3 Mayıs 2026  
**Konu:** Google Ads optimizasyon, website iyileştirme, conversion tracking düzeltme

---

## 1. Kampanya Mevcut Durum (19 Nis — 2 May 2026)

| Cihaz | Tıklama | Gösterim | Dönüşüm | Harcama | CPC |
|-------|---------|----------|---------|---------|-----|
| Mobil | 75 | 1.357 | 2 Kayıt | 672 TL | 8.97 TL |
| Masaüstü | 5 | 190 | 0 | 42 TL | 8.39 TL |
| Tablet | 0 | 22 | 0 | 0 TL | — |
| **Toplam** | **80** | **1.569** | **2** | **714 TL** | ~8.9 TL |

**Önemli bulgular:**
- Dönüşüm başı maliyet: 336 TL (yüksek)
- Trafiğin %94'ü mobilden geliyor
- Masaüstü verimsiz: 42 TL harcama, 0 dönüşüm
- Telefon araması dönüşümü: 0 (takip çalışmıyor)
- Kampanya öğrenme aşamasında (5 gün kaldı)
- Durum: "Uygun (Sınırlı)" — bütçe 100 TL/gün

---

## 2. Tespit Edilen Sorunlar ve Çözümler

### 2.1 Gelişmiş Dönüşümler Uyarısı (⚠️ Kritik)
**Sorun:** "Gelişmiş dönüşümlerde, performansı etkileyen ayar sorunları var" uyarısı
- WhatsApp Tıklama ve Form Gönderimi conversion'larını etkiliyor
- Google "Otomatik" mod ile sayfa içi kodu birlikte kullanmak istiyor

**Kod düzeltmesi (yapıldı):**
- Form submit öncesinde kullanıcı email/telefon verisi gtag'e geçirildi
- `gtag('set', 'user_data', {email, phone_number})` eklendi
- Veri artık `form.reset()` çalışmadan önce okunuyor

**Panelde yapılması gereken:**
- Google Ads → Araçlar → Dönüşümler → Ayarlar → Gelişmiş Dönüşümler
- "Otomatik" seçeneğini etkinleştir
- Her iki conversion action için "Talimatları inceleyin" linkine gir

### 2.2 Cihaz Teklif Ayarları (Google Ads paneli)
- Mobil: +%10 teklif artışı (2 dönüşümün tamamı mobilden)
- Masaüstü: -%20 teklif azaltımı (42 TL harcama, 0 dönüşüm)
- Tablet: -%80 teklif azaltımı (hiç dönüşüm yok)

### 2.3 Reklam Metinleri (Güncellendi)
**Önceki durum:** 6-7 başlık, 2 açıklama, CTA yok
**Yeni durum:** 15 başlık, 4 açıklama, güçlü CTA

Yeni başlık örnekleri:
- "İlk Ders Ücretsiz — Gitar"
- "Kontenjan Dolmadan Kayıt Ol"
- "Gitar Dersi Esenyurt"
- "Hemen Kayıt Yaptır"

Yeni açıklama yapısı: bilgi + CTA
- "Avcılar'da bireysel gitar dersleri. Uzman eğitmenler. Hemen ara, ücretsiz bilgi al."

### 2.4 Anahtar Kelime Genişletme
Her enstrüman grubu 3-4 kelimeden 10 kelimeye çıkarıldı.
Yeni lokasyon varyantları eklendi: Esenyurt, Küçükçekmece, Avrupa Yakası

---

## 3. Website Değişiklikleri (index.html)

### 3.1 İletişim Formu Güçlendirildi
**Eklenen alanlar:**
- Email alanı (enhanced conversions için)
- Enstrüman dropdown: Gitar, Piyano, Bağlama, Keman, Flüt, Klarnet, Diğer
- Seviye seçimi: Başlangıç, Orta, İleri

### 3.2 Schema Markup Eklendi
MusicSchool structured data:
- Ad, adres, telefon, çalışma saatleri, URL
- Google arama sonuçlarında zengin snippet için

### 3.3 CSS Güncellendi
Select elementleri için form stilleri eklendi (önceden input/textarea vardı)

---

## 4. Conversion Tracking Detayları

**Google Ads Account ID:** AW-11553345216  
**Form Submit Conversion:** AW-11553345216/yy64CKW__aQcEMCdiIUr  
**WhatsApp Click Conversion:** AW-11553345216/dsz5CPm6_qQcEMCdiIUr  

**Mevcut tracking durumu:**
- Form: index.html satır 2200-2240 (JavaScript)
- WhatsApp: index.html satır 2245 (onclick)
- 2 Mayıs 2026'da son ping alındı → tracking çalışıyor

---

## 5. Panelde Yapılması Gereken Aksiyonlar (Öncelik Sırasıyla)

1. **Gelişmiş Dönüşümler → Otomatik etkinleştir** (bu hafta)
2. **Cihaz teklifleri:** Mobil +%10, Masaüstü -%20, Tablet -%80
3. **Reklam takvimi:** Gece 00-06 kapat
4. **Lokasyon:** "Bu konumdaki veya bu konumu düzenli ziyaret eden" yap
5. **Reklam metinlerini** güncelle (reklam-metinleri.md dosyasından kopyala)

---

## 6. Negatif Anahtar Kelime Listesi
43 kelime, 8 kategori. Güncelleme tarihi: 2 Mayıs 2026.
Dosya: `sedam-ads/negatif-anahtar-kelimeler.md`
**Kampanyalara uygulandı mı kontrol et!**

---

## 7. Öğrenme Aşaması Notu
Kampanya şu an "Yeni teklif stratejisi öğreniyor" durumunda.
**5 gün daha bekle**, performans değişecektir.
Öğrenme bitmeden büyük değişiklik yapma — öğrenme sıfırlanır.

---

*Bu notlar 3 Mayıs 2026 tarihli Claude Code oturumunda oluşturulmuştur.*
*Bir sonraki review: 10 Mayıs 2026*
