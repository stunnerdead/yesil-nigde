# Yeşil Niğde

COP31 Niğde Simülasyonu (27 Ekim 2026) için NÖHÜ Dijital Oyun Geliştirme Kulübü standında hazırlanan iklim temalı mini oyun.

Oyuncu, kuraklık, hava kirliliği ve susuzlukla boğuşan Niğde'yi doğru kararlarla iyileştirir.

1. **Niğde tehlikede!** Şehir kurak ve dumanlı başlar.
2. **Doğru kararları ver!** 9 soruda her soruna en uygun çözümü seç: *Güneş enerjisi kullan*, *Su tasarrufu yap* ya da *Atıkları geri dönüştür*.
3. **Güçlü Türkiye, Güçlü Niğde!** 100 puanı geçersen şehir yeşillenir, havası temizlenir.

## Nasıl oynanır

**İnternetten:** https://stunnerdead.github.io/yesil-nigde/

**İnternetsiz:** Depoyu indir (yeşil **Code** düğmesi → **Download ZIP**), zip'i aç ve `Yesil-Nigde-OYNA.html` dosyasına çift tıkla. Kurulum gerekmez, Chrome veya Edge önerilir.

**Kontroller:** Fareyle tıkla ya da klavyede **1 / 2 / 3** ile seç, **H** ile Elma'dan ipucu al. Sağ üstten müzik, efekt ve tam ekran açılıp kapatılır.

## Özellikler

- 24 soruluk havuz, her oyunda her kategoriden 3 soru (bir önceki oyunun soruları tekrar etmemeye çalışır)
- Hız bonusu ve seri bonusu (3'lü seri +5, 6'lı seri +10)
- Oyun başına bir ipucu jokeri
- Sorular ilerledikçe kısalan süre (12 sn → 8 sn)
- Her doğru kararla değişen manzara: güneş panelleri, dolan göl, elma ağaçları, geri dönüşüm kutuları
- "Günün En İyileri" skor tablosu (skorlar oynanan bilgisayarda saklanır)
- Sonuç ekranında 90 sn işlem yapılmazsa açılış ekranına otomatik dönüş

## Dosyalar

| Dosya | Ne işe yarar |
| --- | --- |
| `Yesil-Nigde-OYNA.html` | Oyunun kendisi, çift tıklayınca açılır |
| `index.html` | GitHub Pages adresini oyuna yönlendirir |
| `kaynak/yesil-nigde.html` | Oyunun kaynağı; `Yesil-Nigde-OYNA.html` bundan üretilir |

`kaynak/yesil-nigde.html` değiştirildikten sonra oynanabilir dosyayı yeniden üretmek için (Git Bash):

```bash
{ printf '<!doctype html>\n<html lang="tr">\n<head>\n<meta charset="utf-8">\n<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">\n'; cat kaynak/yesil-nigde.html; printf '\n</html>\n'; } > Yesil-Nigde-OYNA.html
```

Tek dosyalık HTML5 Canvas oyunudur; harici kütüphane kullanmaz, yalnızca yazı tipleri Google Fonts'tan gelir (internet yoksa sistem yazı tiplerine düşer).
