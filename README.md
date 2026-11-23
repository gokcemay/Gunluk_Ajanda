# Günlük Ajanda Oluşturucu

Boox ve Kobo gibi e-mürekkep cihazları için kişiselleştirilebilir, sayfaları birbirine bağlantılı bir PDF ajanda oluşturur. Kurulum veya hesap gerekmez. PDF tarayıcınızda hazırlanır ve dosyalarınız cihazınızdan çıkmaz.

## Kullanım

1. `index.html` dosyasını indirin ve güncel bir tarayıcıda açın.
2. Ayarları seçin. Sağdaki önizleme, ayarları değiştirdikçe güncellenir.
3. **PDF Oluştur** düğmesine tıklayın. Bir yıllık ajandanın hazırlanması birkaç saniye sürer. PDF hazır olduğunda indirilir.
4. PDF’yi cihazınıza kopyalayın ve belge içi bağlantıları destekleyen bir okuyucuda açın.

## Ayarlar

| Ayar | Seçenekler |
|---|---|
| Belge adı | Kapakta ve dosya adında kullanılır |
| Takvim yılı | 2026–2035 |
| Haftanın ilk günü | Pazartesi veya pazar |
| Baskın el | Sağ veya sol. Sol el seçildiğinde gezinme düğmeleri karşı tarafa geçer. |
| Yazı tipi | Ajanda Sans (varsayılan), Inter, Atkinson Hyperlegible, Bitter, Ajanda Serif |
| Sayfa ölçüsü | 3:4 (varsayılan), A4 oranı, 16:10 veya Kobo Libra Colour |
| Başlangıç ve bitiş saati | 06:00–20:00 arasında 30 dakikalık adımlarla seçilebilir. Varsayılan saatler 08:30 ve 17:00. |
| Zaman aralığı | Programdaki her satır için 30 veya 60 dakika |
| Günlük not sayfaları | Günde 1, 2 veya 3 sayfa |
| Kapak sayfası | İsteğe bağlı |

## PDF içeriği

- **Kapak** (isteğe bağlı) ajandanın adını, yılını ve 12 aya giden bağlantıları içerir.
- **Aylık takvim** her ayın ilk gününden hemen önce gelir. Tarihler, ilgili günlük planı açar. Takvimin altında bir not alanı bulunur.
- **Günlük plan** yapılacaklar, hatırlatmalar ve saatli program için ayrı alanlar içerir.
- **Günlük notlar** her gün için bir ila üç çizgili sayfadan oluşur.

### Sayfa ölçüleri

Cihazınızın ekranına uygun oranı seçin. Tüm seçenekler 540 pt (7,5 inç) genişliğindedir. Yükseklik, yazı alanını belirler.

| Seçenek | PDF ölçüsü | Uygun cihazlar |
|---|---|---|
| 3:4 | 540 × 720 pt | Boox, reMarkable, Kindle Scribe, Supernote ve 13 inç iPad |
| A4 oranı | Yaklaşık 540 × 764 pt | 11 inç iPad, iPad mini, Surface Pro ve A4 kâğıda baskı |
| 16:10 | 540 × 864 pt | Samsung Galaxy Tab ve diğer Android tabletler |
| Kobo Libra Colour | Yaklaşık 540 × 717,72 pt | 1264 × 1680 piksel Kobo Libra Colour ekranı |

3:4 oranı, ABD Letter kâğıdına baskıya da uygundur.

### Gezinme

- Sayfanın üstündeki **ay sekmeleri** ilgili ayın takvimini açar.
- Gün başlığının altındaki **gün düğmeleri** aynı haftanın diğer günlerine götürür.
- **◀ ▶ okları** günlük sayfalarda haftayı, takvim sayfalarında ayı değiştirir.
- **Günlük Plan** ve **Günlük Notlar** düğmeleri aynı günün sayfaları arasında geçiş yapar. Numaralı sekmeler not sayfasını seçer.

Varsayılan ayarlarla 2026 ajandası 1.108 sayfadır.

## Çevrimdışı kullanım

`index.html` dosyası internet bağlantısı olmadan çalışır. Türkçe karakterleri destekleyen yazı tipleri dosyaya gömülüdür. Sayfa, jsPDF 4.2.1’i jsDelivr üzerinden yükleyemezse gömülü kopyayı kullanır.

## Kaynaklar

- [Daily Planner Generator](https://github.com/Cosmo-NZ/Daily_Planner) (özgün proje)
- [jsPDF](https://github.com/parallax/jsPDF) (MIT lisansı)
- SIL Open Font License 1.1 kapsamındaki yazı tipleri
  - Ajanda Sans ve Ajanda Serif, ParaType’ın PT Sans ve PT Serif yazı tiplerinden uyarlanmıştır.
  - Inter, Rasmus Andersson
  - Atkinson Hyperlegible, Braille Institute
  - Bitter, Huerta Tipográfica
