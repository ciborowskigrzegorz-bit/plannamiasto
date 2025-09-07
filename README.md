# PlannaMiasto

PlannaMiasto to blog o planowaniu przestrzennym, urbanistyce i miejskich inspiracjach. Zbudowany przy użyciu Hugo – najszybszego generatora stron statycznych.

## 🔧 Technologie

- **Generator:** [Hugo](https://gohugo.io)
- **Motyw:** [Ananke](https://themes.gohugo.io/ananke/)
- **Hostowanie:** [Netlify](https://www.netlify.com)

## 🚀 Uruchomienie lokalne

1. **Zainstaluj Hugo:**

   - Na macOS:
     ```bash
     brew install hugo
     ```
   - Na Linux:
     ```bash
     sudo apt install hugo
     ```
   - Na Windows:
     Pobierz instalator z [oficjalnej strony Hugo](https://gohugo.io/getting-started/installing/).

2. **Klonuj repozytorium:**

   ```bash
   git clone https://github.com/ciborowskigrzegorz-bit/plannamiasto.git
   cd plannamiasto

3. Uruchom serwer lokalny:

hugo server

Otwórz stronę w przeglądarce:

Przejdź do http://localhost:1313/.

📦 Struktura katalogów
plannamiasto/
├── archetypes/
├── content/
│   └── posts/
├── data/
├── layouts/
├── static/
├── themes/
│   └── ananke/
├── config.toml
└── README.md
content/posts/: Twoje wpisy w formacie Markdown.
static/: Pliki statyczne (np. obrazy, CSS, JS).
themes/ananke/: Motyw Ananke.
config.toml: Główna konfiguracja strony.
🌐 Wdrożenie na Netlify
Połącz repozytorium z Netlify:
Zaloguj się na Netlify.
Kliknij "New site from Git".
Wybierz GitHub i autoryzuj dostęp.
Wybierz repozytorium plannamiasto.
Skonfiguruj ustawienia builda:
Build command: hugo
Publish directory: public
Dodaj własną domenę:
W panelu Netlify przejdź do Domain settings.
Dodaj domenę plannamiasto.pl i skonfiguruj rekordy DNS zgodnie z instrukcjami Netlify.
Włącz HTTPS:
W Domain settings włącz opcję "Verify DNS configuration" i aktywuj darmowy certyfikat SSL.
✍️ Dodawanie nowych wpisów
Stwórz nowy wpis:
hugo new posts/nowy-wpis.md
Edytuj plik:
Otwórz content/posts/nowy-wpis.md i dodaj treść.
Ustaw draft: false, aby wpis był widoczny na stronie.
Zatwierdź zmiany:
git add .
git commit -m "Dodano nowy wpis"
git push
Netlify automatycznie zbuduje i opublikuje stronę.

📄 Licencja
MIT License – patrz plik LICENSE.

---

## ✅ Dodatkowe uwagi

- **Brak folderu `public/` w repozytorium:** Pamiętaj, że folder `public/` jest generowany lokalnie podczas budowania strony i nie powinien być dodawany do repozytorium. Upewnij się, że masz go w `.gitignore`.
  
- **Dodawanie nowych wpisów:** Aby dodać nowy wpis, użyj polecenia `hugo new posts/nazwa-wpisu.md`, a następnie edytuj plik w folderze `content/posts/`.

- **Aktualizacja motywu:** Jeśli chcesz zaktualizować motyw Ananke, wejdź do folderu `themes/ananke` i wykonaj:

  ```bash
  git pull origin main
Jeśli potrzebujesz dodatkowej pomocy przy konfiguracji CI/CD, GitHub Actions czy integracji z innymi usługami, daj znać!
