# Geçmişten Günümüze Bursa'da STEM

**Bursa İl Millî Eğitim Müdürlüğü — Yenilik ve Eğitim Teknolojileri Hizmetleri Şubesi**

Bursa'nın tarihten günümüze bilim, teknoloji, mühendislik ve matematik mirasını altı izlek ve 24 STEM varlığı üzerinden sunan, GitHub Pages'te çalışan statik bir web sitesi.

## İçerik

| Bölüm | Açıklama |
|---|---|
| 6 izlek | İpek · Su · Toprak ve Yapı · Ateş ve Malzeme · Gökyüzü ve Işık · Hareket |
| 24 STEM varlığı | Her biri için genel bakış, gelişim süreci, bilim köşesi, STEM ve mühendislik alanı bağlantıları |
| 3B inceleme | Parçalarına ayrılıp yeniden birleşen şematik model, bilgi notları, 360° döndürme, etiketler, "İnşa et" modu |
| 4 etkileşimli uygulama | Kemer Kur, Su Terazisi Simülasyonu, Çini Simetri Atölyesi, Karagöz Gölge Laboratuvarı |
| 48 PDF | Her varlık için Türkçe öğretmen kılavuzu ile öğrenci çalışma kâğıdı ve kes-birleştir sayfası |
| İki dil | Site arayüzü ve içerikler Türkçe / İngilizce (sağ üstteki dil düğmesi); PDF'ler yalnızca Türkçe |
| Erişilebilirlik | Klavye ile gezinme, ekran okuyucu etiketleri, yazı boyutu, yüksek kontrast, okuma kolaylığı ve animasyon azaltma |

## GitHub Pages'te yayımlama

Site **tek bir `index.html` dosyasıdır**; tüm sayfalar, 3B modeller ve uygulamalar bu dosyanın içindedir. PDF'ler `pdf/tr` klasöründedir.

Toplam 51 dosya olduğu için hepsi **tek seferde** yüklenebilir (GitHub web arayüzü sınırı 100 dosyadır):

1. Deponuzda **Add file → Upload files** sayfasını açın.
2. Bu klasördeki `index.html`, `README.md` dosyalarını ve **`pdf` klasörünü** birlikte sürükleyip bırakın, ardından "Commit changes" düğmesine basın.
3. **Settings → Pages** bölümünde Source: "Deploy from a branch", Branch: `main`, klasör: `/ (root)` seçeneklerini seçip kaydedin.

Dikkat: Dosyanın adı tam olarak `index.html` olmalıdır. Türkçe klavyede yeniden adlandırırken "i" harfi noktasız "ı" olursa (`ındex.html`) site açılmaz.

## Kurum logosu

Resmî logo bu pakete eklenmemiştir. Logoyu eklemek için depoda `img/logo.png` yoluyla (kare, saydam arka planlı, en az 128 × 128 piksel) kaydetmeniz yeterlidir; başlıkta otomatik olarak görünür. Dosya yoksa site, kendi sade amblemini kullanır.

## Klasör yapısı

```
index.html              Sitenin tamamı (tema, içerik, 3B modeller, uygulamalar, three.js ve Leaflet de içinde)
pdf/tr                  Öğretmen ve öğrenci PDF'leri (Türkçe)
```

## İçerik güncelleme

Varlık metinleri `index.html` içinde, her alan `{ tr: '…', en: '…' }` biçimindedir. Metin değişikliğinde güncellenmiş `index.html` dosyasını yeniden yüklemeniz yeterlidir. (PDF'ler ayrı üretildiği için metin değişikliği PDF'lere otomatik yansımaz.)

## Kaynak ilkesi

Bilgiler yalnızca resmî kurumların (bakanlıklar, valilik, belediyeler, UNESCO, Ramsar Sekretaryası), ilgili kurum ve kuruluşların kendi sitelerinden derlenmiştir. Vikipedi, ansiklopediler, akademik makaleler, haber siteleri ve görsel arşivleri kaynak olarak kullanılmamıştır.

## Fotoğraflar

Site fotoğrafları deponun `img` klasöründen okur (ör. `img/irgandi.jpg`). Fotoğrafı olmayan varlıklarda şematik çizim gösterilir. Dosya adlarının listesi ve kurallar için **FOTOGRAF-REHBERI.md** dosyasına bakın.

- Harita OpenStreetMap altlığı kullanır (© OpenStreetMap katkıcıları, ODbL).

## Bilinen sınırlar

- 3B modeller öğretim amacıyla hazırlanmış şematik gösterimlerdir; oranlar yaklaşık olarak korunmuştur, ölçüler birebir değildir.
- "Yaklaşık" olarak işaretlenen harita konumları bir bölgeyi ya da süreci temsil eder.
- Etkinliklerin dijital tarafı (PDF sayfa düzeni, kes-birleştir geometrisi, uygulamalar) test edilmiştir; sınıf ortamında pilot uygulama yapılması önerilir.
