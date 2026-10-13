# WORKLOG

## Aktif Oturum (2026-10-02)

### Mimari Kararlar
- **[PROTOKOL-001] Sifir Ucuncu Taraf Metin Bagimliligi:** GitHub Camo proxy ve Fastly CDN onbellegindeki kirilganliklari onlemek icin tum kartlar, terminaller ve ikonlar dogrudan reponun `assets/` dizininde statik SVG/PNG olarak barindirilir.
- **[PROTOKOL-002] Ozel Siber Scramble Terminali:** Standart `readme-typing-svg` yerine, hem hex/matris cozulum animasyonuna hem de TypeScript sozcuk dizimine sahip ozel SMIL/CSS animasyonlu `terminal-scramble.svg` gelistirildi.
- **[PROTOKOL-003] Saf Vektorel Yetenek Kartlari:** Standart HTML tablolarinin varsayilan gri cerceveleri yerine 850x260 boyutunda `#020617` arka planli, Lucide ikonlu ve cift dilli kartlar uretildi.
- **[PROTOKOL-004] Renk Disiplini:** Saf beyaz (#ffffff) tamamen elendi; yalnizca Deep Slate `#020617`, Sunset Orange `#FF642B`, Electric Cyan `#00EDFF` ve Slate `#94A3B8` tonlari kullanildi.

### Dersler
- **Semptom:** `api.iconify.design` veya yeni yuklenen `raw.githubusercontent.com` dosyalari ilk dakikalarda Camo tarafindan 404 olarak onbellekleniyor.
- **Sebep:** Fastly CDN 5 dakikalik 404 cache (`max-age=300`) uyguluyor.
- **Cozum:** Commit hash ile dogrudan sorgulamak ve dosya adini benzersiz kilmak; reponun icinde goreceli yol veya kalici hash ile dogrulama yapmak.

## Aktif Oturum (2026-10-13)

### Mimari Kararlar
- **[PROTOKOL-005] Seffaf Telemetri ve Uyum:** GitHub Koyu modunda (`#0d1117`) kartlarin kutu gibi gorunmesini engellemek icin `background=00000000` ve `bg_color=00000000` kullanilarak telemetri araclari (Top Languages & Streak Stats) seffaf kilindi.
- **[PROTOKOL-006] Sistem Dilleri & Birlestirilmis Matris:** Rust ve Python yigina dahil edildi; cift dilli bolumlerdeki kopya pin kartlari kaldirilarak merkezi `FEATURED ARCHITECTURES & CORE ENGINES` tablosunda birlestirildi.
