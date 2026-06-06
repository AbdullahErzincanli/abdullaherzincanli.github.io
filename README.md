# abdullaherzincanli.github.io

AbnaSoftware oyunları için **GitHub Pages kullanıcı sitesi**.
Statik HTML/CSS — derleme (build) adımı yok. `main` branch'e push edildiğinde
`https://abdullaherzincanli.github.io/` adresinde yayınlanır.

## Canlı adresler

| Amaç | URL |
|------|-----|
| Ana sayfa (oyun listesi) | `https://abdullaherzincanli.github.io/` |
| **app-ads.txt** (AdMob) | `https://abdullaherzincanli.github.io/app-ads.txt` |
| Gizlilik politikası | `https://abdullaherzincanli.github.io/privacy.html` |
| Fruit Haul detay | `https://abdullaherzincanli.github.io/games/fruit-haul/` |

## Dosya yapısı

```
.
├── app-ads.txt          # AdMob doğrulaması — KÖKTE kalmalı, taşıma!
├── index.html           # Ana sayfa (oyun ızgarası)
├── privacy.html         # Tüm oyunları kapsayan gizlilik politikası
├── styles.css           # Paylaşılan tasarım sistemi
├── assets/              # Görseller (ikon, truck)
└── games/
    └── fruit-haul/
        └── index.html   # Oyun detay sayfası
```

## Yeni oyun ekleme

1. `games/<oyun-adi>/` klasörü aç, `games/fruit-haul/index.html`'i kopyalayıp düzenle.
2. `index.html` içindeki `games-grid` listesine yeni bir `<li class="game-card">` kartı ekle.
3. Görselleri `assets/` içine koy (web için boyutu küçült).
4. Aynı `privacy.html` yeni oyunu da kapsar — gerekiyorsa "Games" listesine adını ekle.

## Play Console & AdMob kurulumu (her oyun için bir kez)

- **Play Console → Mağaza girişi → Web sitesi:** `https://abdullaherzincanli.github.io`
  (Alan adı app-ads.txt ile birebir aynı olmalı.)
- **Gizlilik Politikası URL'si:** `https://abdullaherzincanli.github.io/privacy.html`
- **AdMob → Uygulamalar → app-ads.txt:** "Tara / kontrol et" ile doğrula.
  (Tarama birkaç saatten birkaç güne kadar sürebilir.)

> Not: `app-ads.txt` mutlaka sitenin **kökünde** olmalı. AdMob alt klasöre
> (`/games/...`) bakmaz; her zaman kök alan adına bakar.
