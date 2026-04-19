# CB-Logbuch v1.0.2

Ein modernes und effizientes Logbuch-Programm für CB-Funk und Amateurfunk, entwickelt in Python mit Tkinter.

## Features

- **QSO-Management**: Schnelle Erfassung von Funkkontakten mit automatischer Entfernungsberechnung (Maidenhead Locator).
- **CAT-Interface**: Unterstützung für Hamlib (`rigctld`), um Frequenz und Modus automatisch vom Funkgerät zu übernehmen.
- **Auto-Import**: Überwacht ADIF-Dateien von Drittsoftware wie WSJT-X oder JS8Call und importiert neue Kontakte automatisch.
- **Live-ADIF Export**: Schreibt QSOs in Echtzeit in eine ADIF-Datei für externes Logging.
- **Datenbank**: Nutzt SQLite für zuverlässige lokale Datenspeicherung.
- **Backup-System**: Erstellt beim Beenden automatisch Backups der Datenbank.
- **Export/Import**: Volle Unterstützung für ADIF- und CSV-Formate.

## Installation

Das Programm benötigt Python 3.x. Es werden keine externen Bibliotheken außerhalb der Standard-Distribution benötigt (Tkinter ist unter Windows standardmäßig dabei).

1. Python installieren.
2. Das Skript `logbuch.py` ausführen:
   ```bash
   python logbuch.py
   ```

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