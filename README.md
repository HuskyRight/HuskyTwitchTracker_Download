# 🐺 HuskyTwitchTracker

Ein modernes, Python-basiertes Desktop-Tool zum Tracking von Twitch-Followern. Vergleiche Scans, identifiziere neue Follower und sehe sofort, wer entfolgt ist.

![Aesthetic](https://img.shields.io/badge/UI-CustomTkinter-blue?style=for-the-badge)
![API](https://img.shields.io/badge/Twitch-API-9146FF?style=for-the-badge&logo=twitch)

## ✨ Funktionen

- **Modernes Dashboard:** Sauberes Dark-Mode Design für beste Übersicht.
- **Input-Speicherung:** Merkt sich automatisch den zuletzt gescannten Kanal über Neustarts hinweg.
- **Update-Benachrichtigung:** Prüft bei jedem Start automatisch auf neue Versionen und bietet einen direkten Download-Link.
- **Echtzeit-Vergleich:** Markiert neue Follower in **Grün** und Unfollower in **Rot**.
- **Historie & Archiv:** Alle Scans werden geloggt. Aktivitäten älter als 7 Tage werden automatisch ins Archiv verschoben.
- **Sichere Verwaltung:** API-Credentials werden lokal in einer `.env` Datei gespeichert (über das Settings-Menü).
- **Standalone EXE:** Kann als einzelne Datei ohne Python-Installation genutzt werden.

---

## 🛠️ Installation

### Voraussetzungen

- Ein Twitch Developer Account ([dev.twitch.tv](https://dev.twitch.tv/))

---

## 🔑 Twitch API Keys erhalten

Um den Tracker zu nutzen, musst du eine App bei Twitch registrieren:

1. Gehe zur [Twitch Developer Console](https://dev.twitch.tv/console).
2. Registriere eine neue Anwendung (Name beliebig, z.B. `HuskyTracker`).
3. Setze die **OAuth Redirect URL** auf `http://localhost:17563`.
4. Kopiere die **Client ID**.
5. Generiere ein **Client Secret** und kopiere es ebenfalls.
6. Trage beide Werte in der App unter **Settings** ein oder erstelle manuell eine `.env` Datei im Hauptverzeichnis:
   ```env
   TWITCH_CLIENT_ID=deine_id
   TWITCH_CLIENT_SECRET=dein_secret
   ```

## 💡 Wichtige Hinweise zur API

Da Twitch den öffentlichen Zugriff auf Follower-Listen eingeschränkt hat, wird dich die App beim ersten Scan auffordern, dich **im Browser bei Twitch anzumelden**. Dies ist notwendig, damit die App die Berechtigung erhält, die Liste deines Kanals (oder Kanäle, die du moderierst) abzurufen.

---



*Entwickelt für Husky-Fans und Twitch-Streamer.* 🐾
