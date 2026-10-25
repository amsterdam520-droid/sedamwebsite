# Session Log — 20 Eylül 2026
Konu: `Sedam - Arama - Eylul 2026` kampanyasının yayına alınması

---

## 1. Kimlikler

| Alan | Değer |
|---|---|
| Hesap | **880-549-6844** — Sedam Müzik Merkezi |
| Giriş | sedaninmuzigi@gmail.com |
| Kampanya | `Sedam - Arama - Eylul 2026` |
| **Gerçek kampanya ID** | **24268863002** |
| Durum | **Etkin** (20 Eyl 2026) |
| Bütçe | ₺150/gün · Tıklama Maks. · maks. TBM ₺18 |
| Sezon bitişi | 22 Ekim 2026 |

Dünkü nottaki `281499251119124` sihirbaz oturum kimliğiymiş — kampanya URL'lerinde 404 veriyor. Doğrusu yukarıdaki.

---

## 2. Yapı — Google Ads Editor'den yüklendi

`sedam-ads/google-ads-yukleme/editor/` klasöründen `02` → `03` → `04` sırayla içe aktarıldı, yayınlandı.

| Öğe | Sayı |
|---|---|
| Reklam grubu | 8 (`01 - Marka` … `08 - Yetiskin`), TBM ₺4–16 |
| Anahtar kelime | 42, sıralı eşleme |
| RSA | 16 |

`01-kampanya.csv` atlandı (kampanya zaten vardı, başlangıç tarihi geçmişte). `05-negatif-kelimeler.csv` atlandı (paylaşılan liste kullanıldı).

Eski `Reklam grubu 1` **duraklatıldı**, silinmedi — onaylı RSA'sı yedek.

---

## 3. Kampanya ayarları

| Ayar | Değer |
|---|---|
| Reklam takvimi | Her gün 07:00-23:00, 6 bant · **23:00-07:00 kapalı** |
| Saat düzeltmeleri | 07-12 `-%5` · 12-14 `0` · 14-16 `+%15` · 16-19 `+%25` · 19-21 `+%10` · 21-23 `-%20` |
| Cihaz | Mobil `-%20` · Masaüstü `+%15` · Tablet `-%80` (kurulumda girilmişti) |
| Konum | Avcılar `+%20` · Küçükçekmece `+%5` · Beylikdüzü `0` · Esenyurt `-%10` |
| Konum tipi | Hedef konumlarımdaki kişiler (Varlık) |
| Demografi | Yaş katmanı: 18-24 `+5` · 25-34 `+10` · 35-44 `+20` · 45-54 `+10` · 55-64 `0` · 65+ `+10` · Bilinmeyen `-50`. Cinsiyet 0. |
| Negatifler | `Sedam - Genel Negatifler` paylaşılan listesi, **152 kelime**, kampanyaya bağlı |
| Ağlar | Yalnızca Google Arama |
| Dil | Türkçe |

**Gün bazlı teklif düzeltmesi uygulanmadı.** Google Ads'te ayrı gün katmanı yok; gün×saat çarpımı 42 satır el girişi demekti ve gün verisi Nisan-Mayıs'tan, 4 ay eskiydi. 14 günlük audit'te taze veriyle yeniden değerlendirilecek.

---

## 4. Varlıklar

- Site bağlantısı ×4: Kurslarımız `#dersler` · Eğitmenlerimiz `#egitmenler` · Ücretsiz Deneme Dersi `#iletisim` · Neden Sedam? `#neden`
- Açıklama metni (kısmi)
- Snippet — Kurslar: Gitar, Piyano, Keman, Bağlama, Klarnet, Yan Flüt
- Promosyon — Müzik Dersi, bitiş 22 Ekim 2026
- İşletme logosu · Telefon `0534 016 48 65` (hesap seviyesi)

**Temizlenenler:** `Hemen iletişime geç!` → `sedammuzikevi.com.tr` (yanlış alan adı, canlıydı) ve 3 çift site bağlantısı kaldırıldı.

**Eksik:** konum uzantısı — Google Business Profile bağlı değil.

---

## 5. Dönüşüm takibi — sorun yok

Ads panelindeki "Etiket etkin değil / Müdahale edilmesi gerekiyor" uyarıları **yanlış alarm**. Uyarı balonu: *Son etkinlik 1 Haz 2026*. Reklamlar 1 Haziran'da durduğu için Ads hiçbir dönüşümü ilişkilendiremedi; sayaç o yüzden durdu.

Canlı sitede doğrulandı: `gtag` fonksiyon olarak yüklü, `gtag_report_conversion` tanımlı, üç etiket de DOM'da, Web3Forms çalışıyor.

| Satır | Etiket | Tetikleyen |
|---|---|---|
| `index.html:2233` | `yy64CKW__aQcEMCdiIUr` | Form gönderimi (Gelişmiş Dönüşüm, `user_data`) |
| `index.html:2278` | `X-LoCJfS0bccEMCdiIUr` | `tel:` bağlantısı |
| `index.html:2292` | `dsz5CPm6_qQcEMCdiIUr` | WhatsApp tıklama |

Üç dönüşüm işlemi de **Birincil**. Kod değişikliği gerekmedi. Kampanya yayında olduğu için uyarıların birkaç gün içinde geçmesi bekleniyor — 23 Eylül'de teyit et.

---

## 6. Takip takvimi

- [ ] **Bugün akşam** — gösterim geliyor mu, ort. TBM, harcama ₺150 civarı mı. TBM ₺18 tavanına dayanıyorsa müdahale.
- [ ] **23 Eylül** — arama terimleri raporu, alakasız sorguları negatif listeye ekle. Dönüşüm uyarılarının geçtiğini doğrula.
- [ ] **27 Eylül** — 15+ dönüşüm varsa Dönüşüm Maksimizasyonu'na geç, bütçe ₺175.
- [ ] **4 Ekim** — mini audit: saat/gün/cihaz/demografi performansını taze veriyle gözden geçir, gün düzeltmelerini şimdi ekle.
- [ ] **22 Ekim** — sezon kapanış audit'i.

Bekleyen: hesap bildirimi "günlük harcama sınırı kaldırıldı" okunacak. ₺150/gün için aylık tavan ₺4.560.

---

## 7. Açık konular

- Negatif listede `org eğitimi`, `online ders`, `online kurs` var. Sedam org/klavye dersi veriyorsa veya online ders satıyorsa bu aramalar kaçıyor — kontrol edilmeli.
- `kanun` ve `darbuka` negatif kalıyor (bu dersler verilmiyor, 20 Eyl'de teyit edildi).
- Afiş: A5'teki QR yer tutucusu `qr-el-ilani.png` ile değiştirilecek, baskı öncesi telefonla taranıp doğrulanacak.
