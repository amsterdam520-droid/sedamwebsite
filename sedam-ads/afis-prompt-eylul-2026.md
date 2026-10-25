# Sedam Müzik — Eylül Kayıt Sezonu Afiş Promptu
Tarih: 19 Eylül 2026
Kullanım: Aşağıdaki prompt bloğunu olduğu gibi kopyala, Claude'a yapıştır.

---

## ÖNCE DOLDUR (afişte uydurma rakam çıkmasın)

Prompt içinde `[...]` ile işaretli yerler var. Yapıştırmadan önce bunları değiştir:

| Alan | Promptaki yeri | Senin değerin |
|---|---|---|
| Kardeş / 2. enstrüman indirimi | `[KARDES_INDIRIMI]` | ör. %20 |
| Kontenjan ifadesi | `[KONTENJAN]` | ör. "Son 12 kontenjan" veya "Kontenjan sınırlı" |
| Son kayıt tarihi | `[SON_TARIH]` | ör. 15 Ekim |

Emin değilsen genel ifade kullan ("kontenjan sınırlı"), sayı uydurma — afişte yazan sayıyı telefonda savunmak zorunda kalırsın.

---

## PROMPT (buradan aşağısı kopyalanacak)

```
ROL: Sen dönüşüm odaklı bir kampanya tasarımcısısın. Bilgi afişi değil,
HAREKETE GEÇİREN afiş tasarlıyorsun. Çıktı: tek bir HTML artifact içinde,
4 farklı en-boy oranında, aynı tasarım dilini paylaşan afiş seti.

İŞ: Sedam Müzik Merkezi — Avcılar / İstanbul müzik kursu
KAMPANYA: Eylül kayıt sezonu. Kayıt penceresi: 15 Eylül - [SON_TARIH] 2026.

HEDEF KİTLE (öncelik sırasıyla):
1. 35-44 yaş anneler — okul çağında (6-14) çocuğu var. Motivasyon:
   "çocuğum ekrandan uzaklaşsın, bir şey üretsin, kendine güveni gelsin".
   Karar verici bu segment. (Google Ads verimizde gösterimlerin %18,1'i,
   en yüksek pay.)
2. 25-34 yaş yetişkinler — "hep istedim ama başlayamadım" hobiciler.
3. Lise / üniversite gençleri — kendi kararını kendi veriyor.

TEK İŞ: Afişi gören kişi 10 saniye içinde WhatsApp'tan yazsın.
Afişin başarı ölçüsü estetik değil, gelen mesaj sayısı. Güzel ama sessiz
bir afiş başarısızdır.

MESAJ HİYERARŞİSİ — buna harfiyen uy. Dört teklifi EŞİTLEME.
Dört eşit teklif = sıfır teklif. Sıra ve boyut şöyle:

  1. KAHRAMAN (en büyük, ilk okunan, afiş yüksekliğinin en az %15'i):
     Ücretsiz Deneme Dersi
  2. ACİLİYET (ikinci okunan, kahramanın hemen altında veya üstünde):
     Eylül kontenjanı: [KONTENJAN] — son kayıt [SON_TARIH]
  3. DESTEK (küçük, tek satırlık alt şerit, ayırıcı nokta ile):
     Kardeşe [KARDES_INDIRIMI] indirim · Eylül'de kaydol, yıl boyu fiyatın sabit
  4. CTA (kahraman kadar göze çarpan, tıklanabilir hissi veren DOLU blok):
     WhatsApp'tan yaz -> 0534 016 48 65   + yanında QR kod alanı
  5. GÜVEN (en küçük punto, en altta, tek satır):
     Avcılar merkezde · Uzman eğitmenler · 5 yaştan itibaren ·
     Gitar Piyano Keman Bağlama Klarnet Flüt

KOPYA KURALLARI:
- Kurumsal dil yasak. "Merkezimiz bünyesinde eğitim verilmektedir" gibi
  cümle kurma. Anneyle konuşur gibi, sade ve sıcak yaz.
- Enstrüman listesini BAŞLIĞA koyma. Başlık duyguyu taşır, liste dipte durur.
- Somut ol: "5 yaştan itibaren", "haftada 1 ders", "ilk ders ücretsiz".
- Ya soruyla aç ya iddiayla aç — ikisini aynı afişte karıştırma.
- Fiyat YAZMA. Reklam verimiz fiyat arayan trafiğin dönüşmediğini gösteriyor;
  fiyat konuşması WhatsApp'ta başlasın.
- Ünlem işaretini tek yerde kullan, o da CTA olmasın.

MARKA SİSTEMİ (sedammuzik.com ile birebir uyumlu olmak zorunda):
- Zemin: #070510 (çok koyu mor-siyah)
- Kart / blok zemini: #0E0C14
- Aksan (lila): #C4B5E8 — CTA bloğu ve kahraman vurgu bu renkte
- Metin: #E8E4F0
- Başlık fontu: Cormorant Garamond (600 / 700) — @import ile çek
- Metin fontu: DM Sans (400 / 500 / 700) — @import ile çek
- Koyu zemin + lila aksan kimliği KORUNACAK. Basılı sürümde bile zemini
  beyaza çevirme; marka tanınırlığı gider.

TASARIM YÖNÜ:
- Telefonda küçük önizlemede bile kahraman mesaj okunabilmeli.
- Boşluk cömert olsun. Dört mesajı sıkıştırma; hiyerarşi sadece puntoyla
  değil, boşlukla kurulur.
- Fotoğraf kullanacaksan TEK fotoğraf, koyu gradient overlay altında,
  metnin arkasında. Kolaj yapma, çerçeveli küçük kareler dizme.
- Müzik ikonografisi klişeye kaçmasın: nota yağmuru yok, sol anahtarı
  süsü yok, piyano tuşu şeridi yok. Enstrüman siluet/fotoğrafı ya da
  soyut dalga / ritim formu tercih et.
- CTA bloğu buton gibi görünsün: dolu lila zemin (#C4B5E8), üstünde koyu
  metin (#070510), yumuşak köşe yarıçapı, etrafında nefes alanı.
- Hizalama tek eksende kalsın (ya hep sola dayalı ya hep ortalı).

TESLİM EDİLECEK 4 KESİM — hepsi aynı HTML artifact içinde, alt alta,
her birinin üstünde ölçü etiketi:

1. Instagram post — 1080 x 1350 px (4:5)
2. Instagram story / WhatsApp durum — 1080 x 1920 px (9:16)
   Üst %15 ve alt %15 güvenli alan: kritik metin buraya girmesin
   (arayüz elemanları ve parmak bu alanı kapatıyor).
3. Basılı el ilanı A5 — 1748 x 2480 px (@300 dpi)
   Kritik metin kenardan en az 8 mm (yaklaşık 95 px) içeride olsun.
   QR kod + adres + telefon ZORUNLU.
   Adres: Şht. Erdoğan Çabuk Sk. No:8/A, Üniversite Mah., Avcılar/İstanbul
4. Google Ads görseli — 1200 x 628 px (yatay)
   Metin minimumda: sadece KAHRAMAN + CTA + marka adı.
   Aciliyet satırını ve destek şeridini bu kesimden ÇIKAR.

TEKNİK:
- Tek HTML artifact. Her kesim kendi container'ında, gerçek px ölçülerinde,
  ekran görüntüsü alınabilecek şekilde net sınırlı.
- Fontları Google Fonts @import ile çek, sistem fallback'e bırakma.
- QR kod için yer tutucu kare bırak, içine "QR: wa.me/905340164865" yaz.
- Kesimlerin altına kullanım talimatı yazma, sadece tasarımı ver.

ÖNCE ŞUNU YAP: Tasarıma başlamadan önce 3 farklı KAHRAMAN BAŞLIK
alternatifi öner (her biri en fazla 6 kelime), her birinin altında tek
cümle gerekçe. Ben birini seçtikten sonra 4 kesimi üret.
```

---

## Kahraman Başlık Bankası (Claude'un önerileri zayıf gelirse)

Anne odaklı:
1. Çocuğunuz bu yıl bir enstrüman çalsın
2. Ekran yerine tel, tuş, nefes
3. İlk ders bizden. Gerisi ona kalmış.
4. Bu yıl "keşke başlasaydık" demeyin

Yetişkin odaklı:
5. Hep istediğin o enstrüman. Bu sene.
6. Başlamak için geç değil. Hiç olmadı.

Sezon / aciliyet odaklı:
7. Okul açıldı, müzik de başlıyor
8. Eylül kontenjanı açıldı

Not: 1, 3 ve 7 test edilmeye en uygun üçlü — biri duygu, biri risk kaldırma, biri zamanlama. Üçünü ayrı afiş olarak üretip hangisinin daha çok mesaj getirdiğine bak.

---

## Revizyon Promptları (afiş geldikten sonra)

Kısa ve tek istekli tut, her seferinde tek şey değiştir:

- `CTA bloğunu %40 büyüt ve kahramanın hemen altına al.`
- `Aciliyet satırını kahramanın üstüne taşı, lila renkte yap.`
- `Destek şeridi çok baskın. Puntoyu küçült, opaklığı 0.7'ye indir.`
- `A5 baskı sürümünde QR kodu iki katına çıkar, telefon numarasını QR'ın altına yaz.`
- `Story kesiminde üst boşluk yetersiz, kahramanı 200px aşağı al.`
- `Google Ads kesiminde çok metin var; sadece başlık + CTA + marka adı kalsın.`
- `Arka plandaki fotoğrafın overlay'ini koyulaştır, başlık okunmuyor.`

---

## Kanal Bazlı Kullanım

### Instagram post (1080x1350)
Caption'a afişteki metni tekrarlama. Caption'da hikâye anlat, CTA'yı sona koy:

> Okullar açıldı. Bu yıl çocuğunuzun haftada bir günü tamamen kendisine ait olsun.
> Avcılar'daki merkezimizde ilk ders ücretsiz — denesin, sevmezse hiçbir yükümlülük yok.
> Eylül kontenjanı sınırlı. Yazın: 0534 016 48 65

### Instagram story (1080x1920)
Afişin üstüne mutlaka tıklanabilir sticker koy: WhatsApp link sticker veya "Bağlantı" sticker → wa.me/905340164865. Statik story tıklanmaz, sticker tıklanır. Haftada 2-3 kez, 17:00-19:00 arası paylaş (Ads verisinde günün gösterim zirvesi bu saatler).

### WhatsApp durum
Aynı 9:16 görsel. Durum metnine kısa tek satır: "Eylül kontenjanı açıldı — ilk ders ücretsiz". Mevcut veli gruplarına doğrudan atma, spam algısı yapar; durumdan gelsin.

### Basılı el ilanı (A5)
Dağıtım noktaları, etki sırasına göre:

1. Okul çıkışları — 15:00-16:30, velilerin beklediği saat (en yüksek verim)
2. Avcılar / Üniversite Mah. site girişleri ve apartman panoları
3. Kırtasiyeler, kitapçılar, çocuk kuaförleri, dershaneler — vitrine asılmak üzere
4. Muhtarlık ve semt pazarı panoları

QR koddan gelenleri ayırt etmek için QR'ı `https://wa.me/905340164865?text=El%20ilani` şeklinde kur — WhatsApp'a düşen mesaj hangi kanaldan geldiğini kendi söyler. Instagram story için de `?text=Instagram` varyantı kullan.

### Google Ads görseli (1200x628)
Şimdilik sadece arama kampanyasının görsel varlığı olarak yüklenecek. Display açılmayacak (Haziran'da 846 TL harcayıp 0 dönüşüm verdi).
