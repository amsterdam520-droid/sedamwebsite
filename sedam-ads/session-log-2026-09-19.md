# Session Log — 19 Eylül 2026
Konu: Eylül kayıt sezonu · Afiş seti + Google Ads kampanya kurulumu

---

## 1. Hesap ve Kimlikler

| Alan | Değer |
|---|---|
| Google Ads hesabı | **880-549-6844** — Sedam Müzik Merkezi |
| Giriş | sedaninmuzigi@gmail.com |
| Yeni kampanya | `Sedam - Arama - Eylul 2026` — ID **281499251119124** |
| Durum | **Yayınlandı → Duraklatıldı** (19 Eyl 2026, ~22:00) |
| Eski kampanyalar | `YENİ` (Arama, ₺100/gün, duraklatıldı) · `Campaign #1` (PMax, ₺70/gün, duraklatıldı, öğe grubu yok) |
| Ölü taslak | campaignId 281499245339739 / draftId 10214782518 — sihirbazda takıldı, **silinecek** |

**Dikkat:** İlk denemede `amsterdam.520@gmail.com` (hesap 308-826-9254) açıktı — orası giyim reklamları, hesap iptal edilmiş. Sedam hesabı farklı girişte.

---

## 2. Afiş Seti — TAMAMLANDI

4 kesim üretildi, 3 revizyon turu geçti (v1 → v2 → v3).

**Kaynak dosyalar:**
- `sedam-ads/afis-prompt-eylul-2026.md` — Claude design promptu, başlık bankası, revizyon komutları, kanal kullanım notları
- `preview/afis-eylul-2026-v3/` — son sürüm HTML + PNG render
- `preview/afis-eylul-2026-v2/`, `preview/afis-eylul-2026/` — önceki turlar

**Kesimler:** IG post 1080x1350 · Story/WhatsApp 1080x1920 · A5 el ilanı 1748x2480 @300dpi · Google Ads 1200x628

**İçerik:** Kahraman "Ekran kapanır, müzik başlar." · "Ücretsiz deneme dersi" · "Kontenjan sınırlı — Son kayıt 22 Ekim" · "Kardeşe %25 indirim · Eylül'de kaydol, yıl boyu fiyatın sabit" · CTA WhatsApp 0534 016 48 65

**QR kodları hazır:** `google-ads-gorseller/qr/`
- `qr-el-ilani.png/svg` → `wa.me/905340164865?text=El%20ilani`
- `qr-instagram.png/svg` → `?text=Instagram`
- `qr-genel.png/svg` → düz link
- Hata düzeltme seviyesi H (%30), 820x820px, marka renkleri

**Afişte kalan tek iş:** A5'teki sahte QR yer tutucusunu `qr-el-ilani.png` ile değiştirmek. Ayrıca A5 fotoğraf kadrajında piyano görünmüyor (isteğe bağlı düzeltme).

---

## 3. Google Ads — Kampanya Kuruldu

### Canlıya alınan yapı

| Ayar | Değer |
|---|---|
| Teklif | Tıklama Sayısını En Üst Düzeye Çıkar, maks. TBM **₺18** |
| Bütçe | **₺150/gün** |
| Ağlar | Yalnızca Google Arama (**ortaklar + Görüntülü Reklam Ağı kapalı**) |
| Konumlar | Avcılar, Küçükçekmece, Beylikdüzü, Esenyurt |
| Konum tipi | **Varlık** (sadece o konumlarda bulunanlar) |
| Dil | Türkçe |
| AI Max / metin özelleştirme / nihai URL genişletmesi | **Kapalı** |
| Reklam grubu | "Reklam grubu 1" (tek) |
| Anahtar kelime | 12, hepsi sıralı eşleme |
| Reklam | 1 RSA — 7 başlık, 2 açıklama, yol `/Avcilar/Muzik-Kursu` — **Google incelemesinde** |

### Dönüşüm durumu (19 Eyl kontrolü)

| İşlem | Kaynak | Durum | Dönüşüm |
|---|---|---|---|
| WhatsApp Tıklama | Web sitesi | Müdahale gerekiyor (Gelişmiş Dönüşümler ayar sorunu) | 30 |
| Form Gönderimi | Web sitesi | Müdahale gerekiyor | 8 |
| Potansiyel müşteri formu gönderimi | Web sitesi | **Etkin değil** | 0 |
| Reklamlardan sesli arama | Arama | İkincil | 0 |
| Tıkla ve ara | Arama | Kaldırıldı | 0 |
| Kişi | Web sitesi | Kaldırıldı | 0 |

Temel takip çalışıyor (WhatsApp 30 dönüşüm kaydetmiş). Sorun yalnızca Gelişmiş Dönüşümler kurulumunda.

### Site kodu kontrolü (index.html)
gtag yüklü · `AW-11553345216` aktif · 3 dönüşüm ID'si yerinde (`X-LoCJfS0bccEMCdiIUr`, `dsz5CPm6_qQcEMCdiIUr`, `yy64CKW__aQcEMCdiIUr`) · `gtag_report_conversion` tanımlı · gelişmiş dönüşüm `user_data` bloğu var · Web3Forms çalışıyor.

---

## 4. Üretilen Dosyalar

```
sedam-ads/
  afis-prompt-eylul-2026.md          Afiş promptu (tamamlandı)
  eylul-2026-kampanya-plani.md       Kutucuklu uygulama planı
  rsa-metinleri-eylul-2026.md        8 grup × (15 başlık + 4 açıklama), limitler doğrulandı
  negatif-anahtar-kelimeler.md       Bölüm 8 eklendi (Eylül sezon negatifleri)
  session-log-2026-09-19.md          Bu dosya

  google-ads-yukleme/
    01-kampanya.csv  02-reklam-gruplari.csv  03-anahtar-kelimeler.csv
    04-rsa-reklamlar.csv  05-negatif-kelimeler.csv
    04b/04c/04d, 05b/05c/05d/05e     web yükleme denemelerinin varyantları
    05e-negatif-BIRLESIK-genis.txt   152 kelime (hesaptaki 104 + yeni 48), tırnaksız
    06-teklif-duzeltmeleri-referans.csv
    NASIL-YUKLENIR.md
    editor/                          Ads Editor için temiz paket + EDITOR-ADIMLARI.md

google-ads-gorseller/qr/             3 QR (png + svg) + data URI
preview/afis-eylul-2026-v3/          Son afiş sürümü
```

---

## 5. Öğrenilenler — Tekrar Denemeye Değmez

**Google Ads web toplu yükleme (Araçlar → Toplu işlemler → Yüklemeler) yeni kampanya OLUŞTURMUYOR.**
`01-kampanya.csv` "Başarılı bir şekilde tamamlandı" dedi ama yükleme ayrıntısında **Değişiklik: 0, Başarılı: 0, Hata: 0**. Sessiz no-op. Mevcut kayıtları düzenlemek için tasarlanmış.

**Web yüklemenin reddettiği kolonlar** (Editor kabul ediyor):
- `Headline N position` (sabitleme) → jenerik "An error occurred"
- `Criterion Type: Campaign Negative Phrase` → "değer geçersiz"
- `Match Type` + `Criterion Type` birlikte → "Incompatible values"

**Kampanya sihirbazı:** İnceleme adımında "Kampanyayı yayınla" butonu sıralı ilerlemede DOM'da görünmüyor; sayfayı URL'den yeniden yüklersen buton geliyor ama bu sefer "Hata kontrolü yapılıyor" sonsuz döngüye giriyor. **Çözüm:** sihirbazı hiç yenilemeden sonuna kadar götür, inceleme sayfasının en altına kaydır — buton orada, sayfa sonunda.

**Google kimlik doğrulaması** ("İşlemi yapanın siz olduğunuzu onaylayın") sihirbaz sırasında 2 kez çıktı (bütçe adımında). Kullanıcı onaylamadan devam edilemiyor.

**Kampanya listesinde kampanya görünmüyorsa:** (a) tarih aralığı kampanyanın oluşturulma gününden önceyi gösteriyordur, (b) "Durum nedeni" gibi takılı kalmış bir filtre vardır. İkisi de bizi yanılttı.

**Tarayıcı otomasyonu notu:** Sayfa %76 yakınlaştırmadayken ekran görüntüsü koordinatları ile gerçek viewport uyuşmuyordu (1526px görünen / 2035px gerçek). `find` ile ref alıp ref üzerinden tıklamak güvenli; koordinat tıklaması kayıyor.

---

## 6. Sonraki Session — Yapılacaklar

### A. Kampanyayı açmadan önce (zorunlu)
- [ ] Reklam takvimi: **23:00-07:00 kapalı**, 16:00-19:00 +%25, 14:00-16:00 +%15, 09:00-12:00 -%10, 21:00-23:00 -%20
- [ ] Gün düzeltmeleri: Cumartesi +%20, Pazar +%15, Salı +%5, Çarşamba -%15
- [ ] Konum düzeltmeleri: Avcılar +%20, Küçükçekmece +%5, Beylikdüzü %0, Esenyurt -%10
- [ ] Cihaz: Mobil -%20, Masaüstü +%15, Tablet -%80
- [ ] Demografi: Kadın 35-44 +%20, Kadın 25-34 +%10, 65+ +%10, 45-54 +%10, 18-24 +%5, Bilinmiyor -%50
- [ ] Negatif paylaşılan liste kur → `05e-negatif-BIRLESIK-genis.txt` (152 kelime) → bu kampanyaya bağla
- [ ] Dönüşümler: WhatsApp + Form Birincil ve Etkin doğrula, Gelişmiş Dönüşümler ayar sorununu çöz
- [ ] Hesap bildirimi: "günlük harcama sınırı kaldırıldı" — ne anlama geldiğini kontrol et

### B. Yapıyı tamamla
- [ ] Ads Editor girişi (onay kodu Seda'ya gidiyor — erişim çözülmeli)
- [ ] `editor/` klasöründen 8 reklam grubu + 42 kelime + 16 RSA yükle
- [ ] Mevcut "Reklam grubu 1"i "02 - Cocuk Sezon" olarak yeniden adlandır veya sil
- [ ] Varlıklar: site bağlantısı (4), callout (6), snippet, promosyon (bitiş 22 Ekim), konum uzantısı

### C. Afiş
- [ ] A5'teki QR yer tutucusunu `qr-el-ilani.png` ile değiştir
- [ ] Baskıya vermeden QR'ı telefonla tara, doğrula

### D. Temizlik
- [ ] Ölü taslağı sil (Kampanyalar → "Devam eden taslaklar: 1")

### E. Açılış
- [ ] Hepsi tamamsa kampanyayı **Etkin** yap
- [ ] 3 gün sonra arama terimleri taraması
- [ ] 7 gün sonra Dönüşüm Maksimizasyonu'na geç, bütçe ₺175
- [ ] 14 gün sonra mini audit
- [ ] 22 Ekim: sezon kapanış audit'i

---

## 7. Açık Sorular
- `kanun` ve `darbuka` negatif listede — Sedam bu dersleri veriyor mu? Veriyorsa listeden çıkarılmalı.
- Kardeş indirimi %25 olarak afişe girdi, doğru mu?
- Son kayıt 22 Ekim — Ads promosyon varlığı da bu tarihe ayarlandı.
