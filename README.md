# 3noodles — Website

Single-file One-Pager für das 3noodles Game Dev Studio.

## Dateien

```
index.html   ← Komplette Website (HTML + CSS + JS in einer Datei)
README.md    ← Diese Datei
```

## Showreel-Video einbinden

Sobald du ein Showreel hast, ersetze in `index.html` diesen Kommentar:

```html
<!-- Drop your showreel here: <source src="showreel.mp4" type="video/mp4"> -->
```

...mit:

```html
<source src="showreel.mp4" type="video/mp4">
```

Und lege `showreel.mp4` im selben Ordner ab. Das Video startet automatisch stumm im Hintergrund; der Play-Button (unten rechts) öffnet es im Fullscreen mit Ton.

## GitHub Pages deployen

1. Neues GitHub Repository erstellen (z. B. `3noodles-website`)
2. Diese Dateien pushen:
   ```bash
   git init
   git add .
   git commit -m "initial"
   git branch -M main
   git remote add origin https://github.com/DEIN-USERNAME/3noodles-website.git
   git push -u origin main
   ```
3. Im Repo → **Settings → Pages → Source: main / root**
4. Fertig — läuft auf `https://DEIN-USERNAME.github.io/3noodles-website/`

## Inhalte anpassen

Alle Texte sind direkt in `index.html` — such nach dem Projektnamen (z. B. `FLORA FORGE`) und ersetze die `data-en` / `data-de` Attribute.

## Custom Domain (optional)

Datei `CNAME` im Root-Ordner anlegen mit deiner Domain:
```
3noodles.de
```
Dann im DNS einen CNAME-Record auf `DEIN-USERNAME.github.io` zeigen lassen.
