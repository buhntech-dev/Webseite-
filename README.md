# Bedarfsmelder – Leitstellen-Webseite

Moderne responsive Leitstellenoberfläche für den Discord-Bedarfsmelder.

## Veröffentlichung mit GitHub Pages
1. Repository → **Settings** → **Pages** öffnen.
2. Unter **Build and deployment** die Quelle **GitHub Actions** auswählen.
3. Der Workflow `.github/workflows/pages.yml` veröffentlicht die Seite bei jedem Push.
4. Die Webseite ist danach unter `https://buhntech-dev.github.io/Webseite-/` erreichbar.

## Verbindung zum Discord-Bot
- Bot-Adresse: öffentliche HTTPS-Adresse des Railway-Dienstes.
- Webhook-Schlüssel: derselbe Wert wie `ALARM_WEBHOOK_SECRET` in Railway.
- Die Webseite speichert den Schlüssel nicht. Er bleibt nur im geöffneten Browser-Tab.
- Railway-Variable `WEB_ALLOWED_ORIGINS` sollte `https://buhntech-dev.github.io` enthalten.
- Der MP3-Test spielt die Datei `assets/alarm.mp3` aus dem Bedarfsmelder-Repository direkt im Browser ab.

**Wichtig:** Der Browser-Testton ist nur eine lokale Vorschau. Für den Ton im Discord-Sprachkanal muss der Bot die Discord-Voice-Verbindung erfolgreich herstellen.
