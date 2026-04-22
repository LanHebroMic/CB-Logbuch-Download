# CB-Logbuch v1.0.5


Ein modernes und effizientes Logbuch-Programm für CB-Funk und Amateurfunk, entwickelt in Python mit Tkinter.

## Features

- **QSO-Management**: Schnelle Erfassung von Funkkontakten mit automatischer Entfernungsberechnung (Maidenhead Locator).
- **CAT-Interface**: Unterstützung für Hamlib (`rigctld`), um Frequenz und Modus automatisch vom Funkgerät zu übernehmen.
- **Auto-Import**: Überwacht ADIF-Dateien von Drittsoftware wie WSJT-X, JS8Call oder wsjt-cb und importiert neue Kontakte automatisch.
- **Live-ADIF Export**: Schreibt QSOs in Echtzeit in eine ADIF-Datei für externes Logging.
- **Datenbank**: Nutzt SQLite für zuverlässige lokale Datenspeicherung.
- **Backup-System**: Erstellt beim Beenden automatisch Backups der Datenbank.
- **Export/Import**: Volle Unterstützung für ADIF- und CSV-Formate.

## Installation

### Windows
1. Paket herunterladen.
2. CB-Logbuch_Setup_1.0.5.exe installieren:per Doppelklick starten.
Dadurch wird das Programm im Startmenü registriert und alle Abhängigkeiten automatisch installiert.

### Linux (Debian/Ubuntu/Raspberry Pi OS)
Der einfachste Weg ist das Debian-Paket:
1. Paket herunterladen.
2. Installieren mit:
   ```bash
   sudo apt install ./cb-logbuch_1.0.5_all.deb
   ```
Dadurch wird das Programm im Startmenü registriert und alle Abhängigkeiten automatisch installiert.

## Bedienung & Tastenkürzel

- **Speichern**: `Enter` in den Eingabefeldern (Skip, MHz, etc.) speichert das QSO direkt.
- **Löschen**: Markierten Eintrag in der Liste auswählen und die `Entf`-Taste drücken.
- **Bearbeiten**: Ein Doppelklick auf einen Eintrag lädt die Daten zurück in die Maske.
- **Suche**: Das Suchfeld im Archiv filtert alle Spalten (Skip, Land, Kommentar, etc.) in Echtzeit.

## Konfiguration

Alle Einstellungen (eigener Locator, Rufzeichen, Pfade für den Auto-Import) können bequem im Tab **Setup** vorgenommen werden. Die Konfiguration wird in `settings.json` gespeichert.

## Haftungsausschluss

Die Nutzung erfolgt auf eigene Gefahr. Bitte erstelle regelmäßig manuelle Sicherheitskopien der Datei `funk_log.db`.

---
*Entwickelt für die Funk-Community - April 2026*