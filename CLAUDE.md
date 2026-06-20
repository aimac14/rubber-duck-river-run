# Rubber Duck River Run — Projekt-Regeln

Minigame für die **SKAILE Academy Building Challenge** (Theme: Gummiente). Eigenständiges Projekt — **kein** Vierzehn-/Naylo-CI, keine Firmen-Vorlagen.

## Push-Disziplin (wichtig — wird von der Jury geprüft)
- Nach **jedem** abgeschlossenen Arbeitsschritt sofort committen und zu `origin` pushen: `git add -A`, kurze klare Message, `git push`.
- Sehr regelmäßig pushen — an den Fortschritt gekoppelt, nicht am Ende alles auf einmal (der Push-Verlauf zählt, nicht das Commit-Datum).
- **Immer nur zu `origin`** (mein eigenes Repo `aimac14/rubber-duck-river-run`) pushen. Ziel nie ändern.
- Zu Beginn jeder neuen Session zuerst `git log --oneline` und `git status` anschauen, kurz orientieren, dann nahtlos weiterbauen.

## Tech-Constraints (aus dem Briefing)
- **Eine Datei:** `index.html` mit inline CSS + JS. Kein Build-Step, keine externen Libraries, kein CDN.
- HTML5 Canvas, vanilla JS, `requestAnimationFrame`-Loop mit Delta-Time.
- **Mobile only**, Portrait ~9:16. Canvas skaliert responsiv (fit width).
- Pixel-Art-Look: niedrige interne Auflösung (180×320), hochskaliert mit `imageSmoothingEnabled = false`.
- Audio nur synthetisiert (Web Audio API), keine Audio-Dateien.
- `localStorage` für Highscore.

## Deploy
- Ziel: **Vercel** (statische Seite). Pfade case-sensitive & relativ halten.

## Stil
- Deutsch kommunizieren. Code-Kommentare auf Deutsch (technische Begriffe bleiben englisch).
- Code in klare Sektionen kommentieren (loop, input, spawning, collision, render, audio, persistence), damit später leicht erweiterbar.
