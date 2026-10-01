# ⚽ FUNiño – Druckzonen-Challenge als iPhone-Web-App

Eine statische Progressive Web App (PWA) für das U7-Training:
- Punktestand Rot/Blau, Punkte erhöhen/verringern, Rollen tauschen
- Countdown 5/10/15/30/45/60/120/600 Sekunden sowie freie Eingabe
- Stoppuhr, Pause und Reset
- Punktestand lokal im Browser gespeichert (nicht in GitHub)
- Offline nach erfolgreichem erstem Online-Aufruf und Cache-Installation
- Icon und eigener Startbildschirm-Modus unter iOS

## Kostenlos über GitHub Pages veröffentlichen

1. Bei [github.com](https://github.com/) anmelden.
2. Auf **+ → New repository** gehen; Namen **`funino-challenge`** eingeben und **Public** auswählen (GitHub Pages ist im Free-Plan für öffentliche Repositories verfügbar). Repository erstellen.
3. Im leeren Repository **uploading an existing file** wählen (sonst **Add file → Upload files**).
4. **Den Inhalt dieses Ordners entpackt hochladen, nicht die ZIP-Datei**: `index.html`, `manifest.webmanifest`, `sw.js`, die drei `.png`-Icons und optional `.nojekyll`, `README.md`. Darauf achten, dass `index.html` im Repository-Stammverzeichnis liegt.
5. Unten auf **Commit changes** klicken.
6. **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root) → Save**.
7. Nach der Veröffentlichung die Adresse öffnen: `https://DEIN-GITHUB-NAME.github.io/funino-challenge/`. Die erste Veröffentlichung kann einige Minuten dauern.

## Auf iPhone installieren

1. Den HTTPS-Link **in Safari** auf dem iPhone öffnen (nicht eine lokale HTML-Datei).
2. Teilen-Symbol → **Zum Home-Bildschirm hinzufügen** → **Hinzufügen**. Falls „Als Web-App öffnen“ angeboten wird, aktivieren.
3. Einmal online laden, danach auch offline nutzbar (vorausgesetzt, das iPhone hat den Cache nicht gelöscht).

**Datenschutz:** Nur der Quellcode der Challenge ist bei einem öffentlichen Repository sichtbar. Punktestände liegen ausschließlich lokal auf deinem iPhone; es sind keine Nutzerkonten, Tracking-Skripte oder Server-Aufrufe für die Spielstände eingebaut.

**Wichtig für Training:** iOS kann Ton im Hintergrund drosseln. Das Signal bei Zeitablauf ist nur zuverlässig, wenn die App im Vordergrund ist und das Gerät Audioausgabe zulässt. Ein gesperrtes Display kann den Timer optisch unterbrechen; beim Entsperren wird die tatsächliche vergangene Zeit aus der Geräteuhr neu berechnet.
