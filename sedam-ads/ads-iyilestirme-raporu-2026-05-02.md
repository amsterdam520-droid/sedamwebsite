# Sedam Muzik Merkezi - Google Ads Iyilestirme Raporu
**Tarih:** 2 Mayis 2026
**Analiz Donemi:** 25 Nisan - 1 Mayis 2026

---

## Haftalik Performans Ozeti

| Metrik | Deger | Durum |
|--------|-------|-------|
| Toplam Harcama | 614.41 TL | - |
| Gosterim | 1.197 | Dusuk |
| Tiklama | 66 | Dusuk |
| CTR | %5.5 | Kabul edilebilir |
| Ort. TBM (CPC) | 9.31 TL | Yuksek |
| Donusum | **0** | KRITIK |

---

## YAPILACAKLAR (Oncelik Sirasina Gore)

### 1. ACIL: Donusum Izlemeyi Duzelt

**Sorun:** 614 TL harcandi, 0 donusum. Izleme ya bozuk ya da eksik.

**Google Ads'te adimlar:**
1. Google Ads'e gir → ust menude "Araclar ve Ayarlar" (anahtar ikonu)
2. "Olcum" altinda "Donusumler"e tikla
3. Mevcut donusum aksiyonlarini kontrol et:
   - "Durum" sutununda "Aktif" mi yoksa "Kayit yok" mu yaziyor?
   - "Son donusum" tarihini kontrol et
4. Eger "Kayit yok" veya "Etkin degil" gosteriyorsa → izleme kodu bozuk

**Eksikse su donusumleri ekle:**
- **Telefon aramasi:** "Yeni donusum aksiyonu" → "Telefon aramalari" → "Web sitenizdeki bir numaraya yapilan tiklamalar"
- **WhatsApp tiklama:** "Yeni donusum aksiyonu" → "Web sitesi" → WhatsApp linkine tiklama eventi
- **Form gonderimi:** "Yeni donusum aksiyonu" → "Web sitesi" → form submit eventi

**Test:** Kendin telefondan reklamina tikla, formu doldur veya numarayi ara. 24 saat icinde Google Ads'te donusum gozukmeli.

---

### 2. ACIL: Negatif Anahtar Kelimeleri Ekle

**Sorun:** Butcenin onemli bir kismi alakasiz aramalara gidiyor.

**Google Ads'te adimlar:**
1. Google Ads → "Araclar ve Ayarlar" → "Paylasilan kitaplik" → "Negatif anahtar kelime listeleri"
2. Mavi "+" butonuna tikla → "Negatif anahtar kelime listesi"
3. Isim: "Sedam - Genel Negatif Liste"
4. Asagidaki kelimeleri yapistir (her satir bir kelime):

```
ucretsiz
bedava
free
indir
youtube
pdf
nasil calinir
nasil ogrenilir
fotograflar
ismek
ibb
belediye
belediyesi
halk egitim
malatya
kadikoy
kagithane
levent
sisli
besiktas
uskudar
sultanbeyli
cekmekoyu
arnavutkoy
basaksehir
bahcesehir
ankara
izmir
bursa
antalya
sonat
ugur akyol
arif sag
erhan birol
imran kaya
caner basbuga
gokay ozgur
dombra
tulum
erbane
bendir
kaval
kemence
akordeon
```

5. "Kaydet" → sonra "Kampanyalara uygula" → tum kampanyalari sec

> Detayli liste: `sedam-ads/negatif-anahtar-kelimeler.md` dosyasinda

---

### 3. YUKSEK: Reklam Takvimini Duzelt

**Sorun 1:** Cumartesi gunu 0 gosterim — kampanya kapali!
**Sorun 2:** Gece 00-06 arasi gosterimlerin %24'u — para israfi

**Google Ads'te adimlar:**
1. Kampanyani sec → sol menude "Reklam takvimi"
2. Mevcut takvimi incele

**Yapilacak degisiklikler:**
- Cumartesi'yi **aktif** et (09:00-21:00)
- Pazar'i **tam gun** aktif et (09:00-21:00) — su an sadece 14:00-17:00
- Hafta ici: 07:00-22:00 (gece 22-07 arasi kapat)
- **Teklif artisi:** 10:00-12:00 ve 15:00-17:00 saatlerinde %20 teklif artisi ekle (en yogun arama saatleri)

---

### 4. YUKSEK: "muzik kursu" Kelimesini Optimize Et

**Sorun:** "muzik kursu" tek basina 269.84 TL harcamis (%44 butce) ama cok genis, alakasiz aramalari tetikliyor.

**Google Ads'te adimlar:**
1. Kampanya → Anahtar kelimeler → "muzik kursu" satirini bul
2. **Secenekler:**
   - **(A) Duraklat** ve yerine lokasyonlu versiyonlarini ekle:
     - "muzik kursu avcilar"
     - "muzik kursu esenyurt"
     - "muzik kursu kucukcekmece"
     - "muzik kursu beylikduzu"
   - **(B) Butcesini kisitla:** Ayri bir reklam grubuna al, gunluk max 20 TL

3. **Iyi CTR'li kelimelerin teklifini artir** (%15-20):
   - "gitar kursu istanbul" (CTR: %11.54)
   - "baglama dersi" (CTR: %10.71)
   - "piyano kursu" (CTR: %9.38)
   - "gitar dersi" (CTR: %9.09)

---

### 5. ORTA: Konum Hedefleme Ayarini Degistir

**Sorun:** Malatya, Kadikoy, Kagithane gibi uzak bolgerden tiklama geliyor.

**Google Ads'te adimlar:**
1. Kampanya → Ayarlar → "Konumlar"
2. "Konum secenekleri" bolumunu bul
3. "Bu konumdaki **veya bu konumla ilgilenen** kisiler" seciliyse → degistir:
   - **"Bu konumdaki veya bu konumu duzenli olarak ziyaret eden kisiler"** sec
4. Bu, sadece fiziksel olarak o bolgede olan kisilere reklam gosterir

---

### 6. DUSUK: Sifir Gosterimli Kelimeleri Canlandir

**Sorun:** "piyano dersi", "flut dersi", "vokal dersi", "cocuk muzik kursu" gibi degerli kelimeler 0 gosterim almis.

**Google Ads'te adimlar:**
1. Bu kelimelerin "Maks. TBM Teklifi"ni kontrol et — cok dusukse artir
2. Lokasyon ekli olanlari degistir:
   - "piyano dersi avcilar" → **"piyano dersi"** (geo-targeting zaten bolgede)
   - "muzik kursu avcilar" → **"muzik kursu avcilar"** (bunu koru, ama genel versiyonunu da ekle)
   - "keman dersi istanbul" → **"keman dersi"**

---

### 7. GELECEK: Ozel Landing Page Olustur

**Sorun:** Reklamlar ana sayfaya yonlendiriyor. Kullanici ne yapacagini bilmiyor.

**Ideal landing page icermeli:**
- Baslik: "Avcilar'da Profesyonel Muzik Egitimi"
- Kurs listesi (piyano, gitar, keman, baglama, vs.) + fiyat araliklari
- Kayit formu (ad, telefon, ilgilenilen kurs)
- WhatsApp ile hizli iletisim butonu (buyuk, gorunur)
- 2-3 ogrenci yorumu / referans
- Harita ve adres
- Mobil oncelikli tasarim (%93 trafik mobilden)

---

## Olumlu Bulgular (Bunlari Koruyun!)

- CTR ortalamasi %5.5 — sektorde iyi
- En iyi kelimeler %9-11 CTR aliyor — bunlara daha fazla butce verin
- Demografi dogru: %58.65 kadin, 25-34 yas (%18.35) — cocuklari icin arayan anneler
- Cihaz dagilimi dogal: %93 mobil

---

## Haftalik Kontrol Listesi

Her hafta Pazartesi bu raporu guncelle:
- [ ] Arama terimleri raporunu kontrol et → yeni negatif kelime ekle
- [ ] Donusum sayisini kontrol et → 0 ise izlemeyi tekrar test et
- [ ] Butce harcama hizini kontrol et
- [ ] CTR dusen kelimeleri incele
- [ ] Bu raporu bir sonraki haftanin verileriyle karsilastir

---

## Beklenen Sonuclar (1 Hafta Sonra)

Bu degisiklikleri uyguladiktan sonra beklenen iyilesmeler:
- Alakasiz aramalarda %50+ azalma (negatif kelimeler)
- Cumartesi-Pazar gosterimleri gorunecek
- Gece 00-06 arasi 0 gosterim (butce tasarrufu)
- Donusum izleme duzeldiyse → ilk donusumler gorunecek
- Ayni butceyle daha fazla nitelikli tiklama
