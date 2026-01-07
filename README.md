# 🚀 Reinwarth Media - Website Launch Package

## 📦 Komplettes Website-Paket

Alle benötigten Dateien für den Launch deiner Website.

---

## 📄 BENÖTIGTE DATEIEN FÜR UPLOAD:

### ✅ HTML Seiten (Pflicht):
```
✅ index.html                    (Hauptseite mit Quiz)
✅ datenschutz.html              (Datenschutzerklärung - DSGVO)
✅ impressum.html                (Impressum)
✅ agb.html                      (AGB)
✅ success.html                  (Erfolgsseite nach Quiz)
```

### ✅ Icons & Bilder (Pflicht):
```
✅ favicon.ico                   (Dein RM Logo)
✅ apple-touch-icon.png          (180x180px für iOS)
✅ favicon-16x16.png
✅ favicon-32x32.png
✅ favicon-48x48.png
✅ icon-192.png                  (für Android)
✅ icon-512.png                  (für Android)
```

### ✅ Videos (Optional aber empfohlen):
```
✅ drohne.mp4                    (5MB - Hintergrund-Video)
```

---

## 🌐 UPLOAD STRUKTUR:

```
deine-domain.de/
│
├── index.html              ← Hauptseite
├── datenschutz.html        ← Datenschutz
├── impressum.html          ← Impressum
├── agb.html                ← AGB
├── success.html            ← Erfolgsseite
│
├── favicon.ico             ← Favicons
├── apple-touch-icon.png
├── favicon-16x16.png
├── favicon-32x32.png
├── favicon-48x48.png
├── icon-192.png
├── icon-512.png
│
└── drohne.mp4              ← Video (optional)
```

**WICHTIG:** Alle Dateien im **ROOT-Verzeichnis** hochladen (nicht in Unterordner)!

---

## ⚙️ NACH DEM UPLOAD:

### 1. Google Sheet URL prüfen:
Öffne `index.html` und suche nach (Zeile ~1194):
```javascript
const GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/...";
```
✅ Prüfe ob die URL korrekt ist

### 2. Website testen:
- ✅ index.html öffnen → Quiz starten
- ✅ Cookie-Banner erscheint
- ✅ Quiz durchspielen
- ✅ success.html wird angezeigt
- ✅ Daten im Google Sheet prüfen

### 3. DSGVO-Test:
- ✅ Cookie-Banner → "Nur Essenzielle" klicken
- ✅ F12 → Network Tab → KEIN Google Analytics Aufruf
- ✅ Cookie-Banner → "Alle Cookies gönnen" klicken
- ✅ Google Analytics lädt ✅

### 4. Mobile-Test:
- ✅ Auf Smartphone öffnen
- ✅ Alle Seiten durchklicken
- ✅ Quiz ausfüllen
- ✅ Alles lesbar?

---

## 🔧 GITHUB UPLOAD ANLEITUNG:

### Option A: GitHub Desktop (Einfach):
1. GitHub Desktop öffnen
2. "New Repository" → Name: `reinwarth-media-website`
3. Alle Dateien in den Ordner kopieren
4. "Commit to main" → "Publish repository"
5. GitHub Pages aktivieren (Settings → Pages)

### Option B: Kommandozeile:
```bash
# Repository erstellen
git init
git add .
git commit -m "Initial launch"
git branch -M main
git remote add origin https://github.com/DEIN-USERNAME/reinwarth-media-website.git
git push -u origin main

# GitHub Pages aktivieren
# → Gehe zu Settings → Pages → Source: main → Save
```

### Option C: Direkter Upload:
1. GitHub → New Repository
2. Drag & Drop alle Dateien
3. Settings → Pages aktivieren

---

## 🌐 DOMAIN VERBINDEN:

### Bei GitHub Pages:
1. Settings → Pages
2. Custom domain: `reinwarth-media.de` eingeben
3. Bei deinem Domain-Provider (z.B. Namecheap):
   ```
   A Record: 185.199.108.153
   A Record: 185.199.109.153
   A Record: 185.199.110.153
   A Record: 185.199.111.153
   CNAME: www → DEIN-USERNAME.github.io
   ```

---

## ✅ CHECKLISTE VOR LAUNCH:

### Technisch:
- [ ] Alle 5 HTML-Dateien hochgeladen
- [ ] Alle 7 Icon-Dateien hochgeladen
- [ ] drohne.mp4 hochgeladen (optional)
- [ ] Google Sheet URL korrekt in index.html
- [ ] Cookie-Banner funktioniert
- [ ] Quiz funktioniert
- [ ] success.html erreichbar

### Rechtlich:
- [ ] Datenschutzerklärung vorhanden (✅)
- [ ] Google Analytics erwähnt (✅)
- [ ] Facebook Pixel erwähnt (✅)
- [ ] Impressum vollständig (✅)
- [ ] AGB vorhanden (✅)

### DSGVO:
- [ ] Tracking nur mit Consent (✅)
- [ ] IP-Anonymisierung (✅)
- [ ] Opt-Out Möglichkeiten (✅)

### Mobile:
- [ ] Auf Smartphone getestet
- [ ] Auf Tablet getestet
- [ ] Alles lesbar

---

## 🎯 DATEIGRÖSSEN:

```
index.html          116 KB    ← Hauptseite
datenschutz.html     17 KB    ← Datenschutz
impressum.html       10 KB    ← Impressum
agb.html             25 KB    ← AGB
success.html         11 KB    ← Erfolg
drohne.mp4          5.1 MB    ← Video (optional)
Icons gesamt         21 KB    ← Alle Favicons

TOTAL: ~5.3 MB
```

---

## 🚨 WICHTIG:

### Google Sheet muss LIVE sein:
Die Website sendet Daten an:
```
https://script.google.com/macros/s/AKfycb.../exec
```
→ Prüfe ob das Script deployed ist!

### Browser-Cache:
Nach Upload immer **STRG + SHIFT + R** drücken für Hard Reload!

---

## 💡 SUPPORT:

### Problem: Cookie-Banner erscheint nicht?
→ Browser-Cache leeren (STRG + SHIFT + R)

### Problem: Quiz-Daten kommen nicht an?
→ Google Apps Script URL prüfen
→ F12 → Console → Fehlermeldungen?

### Problem: Seite lädt langsam?
→ drohne.mp4 ist 5MB → Optional weglassen

### Problem: Mobile sieht komisch aus?
→ Browser-Cache leeren
→ Inkognito-Modus testen

---

## 🎉 FERTIG!

**Alle Dateien sind bereit für den Launch!**

Einfach auf GitHub hochladen und loslegen! 🚀

---

**Version:** 2.0 - DSGVO-konform
**Letztes Update:** 07.01.2026
**Status:** ✅ Production Ready
