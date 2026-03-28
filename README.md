# GardenerX

Fen bilimlerini strateji oyunuyla birlestiren egitici bir iOS mobil oyunu. Quiz'lerde bilgini test et, token kazan, bahceni bocek istilasindan koru!

## Oyun Modlari

### Quiz
- Biyoloji, Fizik, Kimya, Yer Bilimi ve Astronomi kategorilerinde 2050 soru
- 3 zorluk seviyesi (Kolay, Orta, Zor)
- 30 saniye sure limiti, 4 sikli coktan secmeli
- Seri dogru cevaplarla carpan bonusu (3x'e kadar)

### Tower Defense
- 20 seviye, 4 mevsim (Ilkbahar, Yaz, Sonbahar, Kis)
- 8 bocek turu (Karinca, Tirtil, Sivrisinek, Bocek, Orumcek, Salyangoz, Circir, Ari Kralice)
- 12 savunucu rolu (Atici, Keskin Nisanci, Bombaci, Tank, Iyilestirici ve daha fazlasi)
- Her mevsimin kendine ozgu temasi: kar yagisi, dusen yapraklar, cicek yapraklari
- Sezon bazli kart acilma sistemi — guclu kartlar ilerledikce acilir

### Dukkan
- 25 farkli savunma ve taarruz itemi
- Token ile satin alma
- Sezona gore kademeli erisim

## Teknik Detaylar

- **Platform:** iOS
- **Dil:** Swift
- **Motor:** SpriteKit
- **Minimum iOS:** 16.0
- **Yonelim:** Landscape
- **Ses:** AVAudioEngine ile PCM buffer sentezi
- **Veri:** JSON tabanli yerel depolama
- **Grafik:** Emoji tabanli render

## Proje Yapisi

```
GardenerX/
├── Managers/     # Is mantigi (GameState, Battle, Shop, Question, Audio, Persistence)
├── Models/       # Veri yapilari (PlayerData, BattleLevel, BugType, GardenItem, Question)
├── Scenes/       # Oyun ekranlari (MainMenu, Quiz, Battle, Shop, Settings, Guide)
├── Nodes/        # SpriteKit bilesenleri (BugNode, ButtonNode, HealthBar, SeasonTheme)
├── Resources/    # JSON config dosyalari (BattleLevels, BugTypes, ShopCatalog, CombatStats, questions)
└── Extensions/   # Swift extension'lari
```

## Build

```bash
xcodebuild -project GardenerX.xcodeproj -scheme GardenerX build
```

## Gizlilik

GardenerX hicbir kisisel veri toplamaz. Tum veriler cihazda yerel olarak saklanir. Detaylar icin [Gizlilik Politikasi](docs/privacy-policy.md).

## Lisans

© 2026 CKR Games. Tum haklar saklidir.
