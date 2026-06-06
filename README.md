# AI Insights

## 1. Úvod

**AI Insights** je jednoduchý více-stránkový prezentační web o umělé inteligenci. Cílem je představit základní principy AI, její využití a dokumentaci technických rozhodnutí v přehledné a responzivní podobě.

Živý web: https://www.mojeaiprezentace.cz/

## 2. Použité technologie

- HTML5
- CSS3
- Vanilla JavaScript (ES6)
- Žádné externí frameworky
- Systémové fonty místo Google Fonts

## 3. Adresářová struktura

- `index.html` – úvodní stránka projektu
- `proc-ai.html` – stránka „Proč AI“
- `vyuziti.html` – stránka s příklady využití AI
- `zkusenost.html` – stránka s osobní zkušeností
- `dokumentace.html` – technická dokumentace projektu
- `style.css` – hlavní styly
- `script.js` – navigace, aktivní odkaz a animace scrollu
- `robots.txt` / `sitemap.xml` – SEO soubory

## 4. Technický rozbor

### Výkon
Web používá co nejméně externích zdrojů.

- JavaScript je načítán s atributem `defer`, aby se neblokovalo vykreslování.
- Použity jsou systémové fonty místo stahování webových fontů.

```html
<script src="script.js" defer></script>
```

### SEO
Stránky obsahují základní SEO meta tagy a strukturu.

- `lang="cs"` v `<html>`
- `meta description`
- `link rel="canonical"`
- `robots.txt` a `sitemap.xml`

```html
<meta name="description" content="Simplistický úvod do světa umělé inteligence.">
<link rel="canonical" href="https://www.mojeaiprezentace.cz/">
```

### Přístupnost
Projekt používá sémantické HTML a základní ARIA prvky.

- `aside`, `main`, `section`
- `aria-label` na navigaci
- Skip link pro rychlý přeskok na obsah
- Viditelné fokusové styly pro klávesnici

```html
<a href="#main-content" class="skip-link">Přejít na obsah</a>
```

### Sociální metadata
Do hlaviček byly přidány Open Graph a Twitter tagy pro lepší sdílení.

```html
<meta property="og:title" content="Potenciál a Síla Umělé Inteligence - Úvod">
<meta name="twitter:card" content="summary_large_image">
```

### UI/UX a responzivita
Web je navržen responsivně.

- `meta viewport`
- adaptivní postranní panel pro menší obrazovky
- `clamp()` pro plynulé titulky

```css
#hero-title {
    font-size: clamp(3rem, 5vw, 5rem);
}
```

### Validita a čistota kódu
Web je postaven bez zbytečných knihoven a obsahuje minimální množství CSS/JS. Kód je dobře strukturovaný a snadno čitelný.

## 5. AI Deník

Při práci na projektu jsem použil AI jako asistenta pro:

- tvorbu technické dokumentace
- návrh SEO a sociálních meta tagů
- kontrolu přístupnosti a UX
- sepsání tohoto `README.md`

Pár použitých promptů:

- „Napiš README pro web o umělé inteligenci v češtině podle struktury: úvod, technologie, struktura, technický rozbor, AI deník, instalace, galerie."
- „Jaké jsou nejlepší praktiky pro přístupnost v jednoduchém HTML/CSS projektu?"

## 6. Instalace a spuštění

### Lokálně otevřít soubor
Otevřete `index.html` přímo v prohlížeči.

### Spuštění z lokálního serveru
Pokud používáte Python, můžete spustit lokální server:

```powershell
cd "c:\Users\Kuchtík\Desktop\the big program"
python -m http.server 8000
```

Pak otevřete v prohlížeči: `http://localhost:8000`

## 7. Galerie

- Desktop verze: úvodní stránka se sidebar navigací.
- Mobilní verze: postranní panel se mění na horní navigaci a obsah je čitelný na malých obrazovkách.
- Klíčové funkce: aktivní odkaz v navigaci, skip link, responsivní rozvržení, animace načítání obsahu.

> Poznámka: Doporučuji do galerie přidat screenshoty za běhu v desktopu a mobilu z Chrome DevTools nebo z mobilního zařízení.
