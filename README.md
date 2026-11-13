# Koło Kwintowe (PWA) — Polska Notacja Muzyczna

Interaktywna aplikacja webowa (Progressive Web App) zaprojektowana dla urządzeń z systemem Android oraz przeglądarek desktopowych.

## Funkcje
- **Polska notacja muzyczna:** akordy durowe na zewnętrznym pierścieniu (`C, G, D, A, E, H, Fis/Ges, Des, As, Es, B, F`), molowe na wewnętrznym (`a, e, h, fis, cis, gis, dis/es, b, f, c, g, d`).
- **Podświetlanie pokrewnych funkcji:** 6 akordów danej tonacji podświetlonych na żółto (`#ffd60a`) na ciemnoniebieskim tle (`#0a1428`).
- **Dominanta harmoniczna w tonacjach molowych:** podświetlenie opcjonalnej dominanty durowej `(D)` na kole oraz interaktywny zapis `e (E)` w panelu dolnym.
- **Syntezator Web Audio API:** odsłuch pojedynczych trójdźwięków oraz całej kadencji bez zewnętrznych plików dźwiękowych.
- **Pełna obsługa offline (PWA):** `manifest.json` oraz `sw.js` umożliwiają instalację na ekranie głównym Androida.

## Struktura repozytorium
```text
├── index.html          # Główna aplikacja (HTML + CSS + JS)
├── manifest.json       # Konfiguracja PWA (ikony, tryb standalone, kolory)
├── sw.js               # Service Worker (cache offline)
├── icons/
│   ├── icon-192.svg    # Ikona aplikacji 192x192
│   └── icon-512.svg    # Ikona aplikacji 512x512
└── README.md           # Dokumentacja projektu
```

## Publikacja na GitHub Pages
1. Utwórz nowe repozytorium na GitHubie i wgraj wszystkie pliki z zachowaniem struktury katalogów (wraz z folderem `icons/`).
2. Wejdź w **Settings → Pages**.
3. W sekcji **Build and deployment** wybierz **Deploy from a branch**, wskaż gałąź `main` oraz katalog `/ (root)` i kliknij **Save**.
4. Po chwili aplikacja będzie dostępna pod adresem `https://<twoj-login>.github.io/<nazwa-repozytorium>/`.
5. Otwórz link w przeglądarce Chrome na telefonie z Androidem i wybierz **Dodaj do ekranu głównego / Zainstaluj aplikację**.
