# Reklam Metni Generator

Bu promptu Claude'a ver. Girdi bilgilerini doldur, geri kalanı Claude halleder.

---

## KULLANIM

Aşağıdaki "Girdi" bölümünü doldur ve tüm sayfayı Claude'a yapıştır.

---

## Girdi

**Kampanya Konusu:** [ör: Eylül kayıt sezonu / Yaz kampı / Piyano kursları / Yeni başlayanlar]  
**Hedef Kitle:** [ör: ebeveynler, yetişkinler, gençler]  
**Öne Çıkarılacak Avantaj:** [ör: ücretsiz deneme dersi, taksit imkanı, uzman eğitmenler, küçük gruplar]  
**Açılış Sayfası URL:** [ör: sedammuzik.com/kayit]  
**CTA Tercihi:** [ör: Ara / Form Doldur / Kayıt Ol / Ücretsiz Dene]  
**Kısıtlamalar / Kaçınılacaklar:** [ör: fiyat yazma, rakip ismi geçirme]

---

## Claude'a Komut

Yukarıdaki bilgilere dayanarak Sedam Müzik Merkezi için bir **Responsive Search Ad** oluştur.

**Kural:**
- 15 başlık yaz. Her biri MAX 30 karakter (boşluklar dahil). Karakter sayısını yanına yaz.
- 4 açıklama yaz. Her biri MAX 90 karakter. Karakter sayısını yanına yaz.
- Başlıkları çeşitlendirmeli: bazıları benefit odaklı, bazıları CTA, bazıları anahtar kelime içermeli
- Açıklamalar güçlü bir vaadi ve net bir CTA'yı birlikte içermeli
- Türkçe, doğal ve samimi ton
- Sonuna 5 önerilen anahtar kelime (phrase match) ekle

**Çıktı Formatı:**

```
BAŞLIKLAR:
1. [başlık] — [XX karakter]
2. ...
(15 adet)

AÇIKLAMALAR:
1. [açıklama] — [XX karakter]
2. ...
(4 adet)

ÖNERİLEN ANAHTAR KELİMELER:
- "piyano dersi [şehir]"
- ...
```

---

## Örnek Girdi → Referans Amaçlı

```
Kampanya: Eylül kayıt sezonu
Hedef: Ebeveynler (çocuk 6-12 yaş)
Avantaj: İlk ders ücretsiz, deneyimli eğitmenler
URL: sedammuzik.com/cocuk-kurslari
CTA: Ücretsiz Ders Al
```

### Örnek Çıktı (kısaltılmış)

BAŞLIKLAR:
1. Çocuğun Müzikle Tanışsın — 28 karakter  
2. İlk Ders Tamamen Ücretsiz — 28 karakter  
3. Uzman Eğitmenlerle Öğren — 27 karakter  
4. Kayıt Sezonu Başladı! — 22 karakter  
5. Piyano Gitar ve Daha Fazlası — 30 karakter  

AÇIKLAMALAR:
1. Çocuğunuzu müzikle buluşturun. Uzman eğitmenler, küçük gruplar. İlk ders ücretsiz! — 86 karakter
2. Kayıt olun, ilk dersinizi ücretsiz alın. Eylül kontenjanı dolmadan yerinizi ayırtın. — 87 karakter

---

## Aktif RSA - Demografiye Özel Başlıklar (Kadın 35-44 Segmenti)
Güncelleme: 19 Mayıs 2026
Veri: Kadın 35-44 segmenti en yüksek gösterim payına sahip (%18.10) — okul çağı çocuk anneleri

### Mevcut RSA'ya Eklenecek Çocuk/Ebeveyn Odaklı Başlıklar

```
EKLENECEK BAŞLIKLAR:
1. Çocuğunuz İçin Müzik Kursu — 30 karakter
2. 5 Yaşından İtibaren Müzik — 27 karakter
3. Çocuk Müzik Eğitimi Avcılar — 30 karakter
4. Güvenli Çocuk Müzik Okulu — 28 karakter
5. Uzman Eğitmenler Güvenli Ortam — 32 karakter (kısalt: "Uzman Eğitmen, Güvenli Ortam" — 30)
6. Deneyimli Müzik Eğitmenleri — 30 karakter
7. Ailelerin Tercih Ettiği Okul — 30 karakter
```

### Mevcut RSA'ya Eklenecek Yeni Açıklamalar

```
EKLENECEK AÇIKLAMALAR:
1. Çocuğunuz için profesyonel müzik eğitimi. Piyano, gitar, keman. Avcılar'da ilk ders ücretsiz. — 93 karakter (kısalt: son kelimeyi çıkar → 90 altı yap)
   Düzeltilmiş: "Çocuğunuz için profesyonel müzik eğitimi. Piyano, gitar, keman. İlk ders ücretsiz." — 86 karakter

2. Her yaşa özel müzik kursu. Başlangıçtan ileri seviyeye gitar, bağlama, flüt. Ücretsiz deneyin. — 97 karakter
   Düzeltilmiş: "Her yaşa özel müzik kursu. Gitar, bağlama, flüt. Avcılar'da ücretsiz deneme dersi." — 85 karakter

3. Sınırlı kontenjan! Avcılar müzik kursuna kayıt için hemen arayın. İlk ders tamamen ücretsiz. — 95 karakter
   Düzeltilmiş: "Kontenjan dolmadan kayıt olun! Avcılar'da müzik kursu. İlk deneme dersi ücretsiz." — 84 karakter
```

### Google Ads RSA'ya Uygulama Adımları
1. Kampanyalar → YENİ → Reklam grupları → Reklamlar
2. Mevcut RSA'nın üzerine tıkla → Düzenle
3. Başlıklar bölümüne yukarıdaki başlıklardan 3-4 tanesini ekle (toplam 15 başlık limiti)
4. Açıklamalar bölümüne yeni açıklamayı ekle (toplam 4 açıklama limiti)
5. "Sabitle" özelliğini kullanma — Google'ın en iyi kombinasyonu bulmasına izin ver
6. Kaydet

### Hangi Başlıkları Çıkarmalı (Yer Açmak İçin)
Mevcut başlıklardan düşük performanslı olanları Google Ads → Reklamlar → "Reklam gücü" bölümünden gör.
"Düşük" veya "Orta" etiketli başlıkları yenileriyle değiştir.
