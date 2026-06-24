# Kalkulačka projektu — Alpha Reality

Webová kalkulačka pre rýchly výpočet nákladov, predajnej ceny a hrubého zisku z developerského projektu (holodom + pozemok).

**Funkcie:**
- Holodom — vstupná cena za m² s DPH, výsledok bez DPH aj s DPH
- Pozemok — bez DPH
- Hrubý zisk zvlášť za holodom a zvlášť za pozemok
- Súhrnná tabuľka projektu
- Plne offline, jeden HTML súbor, žiadne závislosti

---

## Nasadenie na GitHub Pages

### 1. Vytvor nový repozitár
1. Choď na [github.com/new](https://github.com/new)
2. Názov: napríklad `kalkulacka` alebo `kalkulacka-alpha-reality`
3. Visibility: **Public** (povinné pre bezplatné GitHub Pages)
4. Klikni **Create repository**

### 2. Nahraj súbory
1. V repozitári klikni **uploading an existing file**
2. Pretiahni súbor `index.html` (a tento `README.md`)
3. Klikni **Commit changes**

### 3. Zapni GitHub Pages
1. V repozitári choď do **Settings** → **Pages** (ľavé menu)
2. Pod **Source** vyber **Deploy from a branch**
3. Branch: **main**, Folder: **/ (root)**
4. Klikni **Save**

Po 1–2 minútach bude kalkulačka dostupná na:
```
https://TVOJEMENO.github.io/kalkulacka/
```

### 4. (Voliteľné) Vlastná doména
Ak chceš URL typu `kalkulacka.alphareality.sk`:

1. V **Settings → Pages** zadaj **Custom domain**: `kalkulacka.alphareality.sk`
2. U poskytovateľa domény (kde máš alphareality.sk) pridaj DNS záznam:
   - Type: **CNAME**
   - Name: `kalkulacka`
   - Value: `TVOJEMENO.github.io`
3. Počkaj 5–30 minút na propagáciu DNS
4. V GitHub Pages zaškrtni **Enforce HTTPS**

---

## Úpravy

Celá kalkulačka je v jednom súbore `index.html`. Ak chceš zmeniť:

- **Sadzbu DPH** — v `<script>` zmeň `const VAT = 0.23;`
- **Farby** — v `:root` na začiatku `<style>`:
  - `--gold: #DAB967;` — Alpha Gold
  - `--onyx: #141414;` — Onyx
  - `--cream: #F2EFE9;` — Warm Cream
- **Predvolené hodnoty** — atribút `value=""` pri jednotlivých `<input>`

---

Alpha Reality s.r.o. · [alphareality.sk](https://www.alphareality.sk)
