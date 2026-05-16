# CB-Logbuch v1.2.1
**Entwickler: LanHebroMic**

Ein modernes und effizientes Logbuch-Programm für CB-Funk und Amateurfunk, entwickelt in Python mit Tkinter.

## Features

- **QSO-Management**: Schnelle Erfassung von Funkkontakten mit automatischer Entfernungsberechnung (Maidenhead Locator).
- **SOTA / POTA / BOTA / IOTA**: Volle Unterstützung für spezielle Funk-Referenzen direkt in der Eingabemaske.
- **Solar-Wetter & Propagation**: Live-Abfrage von SFI, A- und K-Index inkl. automatischer Bewertung der Ausbreitungsbedingungen für das aktive Band basierend auf Standort und Tageszeit.
- **Update-Check**: Automatische Prüfung auf neue Versionen beim Programmstart direkt über die GitHub-API.
- **Erweitertes CAT-Interface**: Unterstützung für Hamlib (`rigctld`) mit automatischem Hintergrund-Start, Modellauswahl und bidirektionaler Synchronisation von Frequenz und Modus.
- **Split-Betrieb**: Getrennte Erfassung von RX- und TX-Frequenzen sowie gesendeten Rapporten.
- **Automatische Ländererkennung**: Bestimmung des Landes anhand von Rufzeichen-Präfixen und CB-Divisionen während der Eingabe.
- **Auto-Import**: Überwacht ADIF-Dateien von Drittsoftware (WSJT-X, JS8Call etc.) und importiert neue Kontakte automatisch mit intelligenter Dublettenprüfung.
- **Live-ADIF Export**: Schreibt QSOs in Echtzeit in eine ADIF-Datei für externes Logging.
- **Datenbank**: Nutzt SQLite für lokale Speicherung oder optional MySQL für fortgeschrittene Setups.
- **Backup-System**: Erstellt beim Beenden automatisch Backups der Datenbank.
- **Export/Import**: Volle Unterstützung für ADIF- und CSV-Formate.
- **Kartenansicht**: Visualisierung von Kontakten auf einer Weltkarte mit optionaler Offline-Unterstützung und Klick-Statistiken für Locator-Regionen.
- **Modernes UI**: Unterstützung verschiedener Design-Themes, Kontextmenüs für alle Textfelder und dynamische Spaltenanpassung.

## Installation

### Windows
1. Paket herunterladen.
2. CB-Logbuch_Setup_1.2.1.exe installieren: per Doppelklick starten.
Dadurch wird das Programm im Startmenü registriert und alle Abhängigkeiten automatisch installiert.

### Linux (Debian/Ubuntu/Raspberry Pi OS)
Der einfachste Weg ist das Debian-Paket:
1. Paket herunterladen.
2. Installieren mit:
   ```bash
   sudo apt install ./cb-logbuch_1.2.1_all.deb
   ```
Dadurch wird das Programm im Startmenü registriert und alle Abhängigkeiten automatisch installiert.

## Bedienung & Tastenkürzel

- **Speichern**: `Enter` in den Eingabefeldern (Skip, MHz, etc.) speichert das QSO direkt.
- **Löschen**: Markierten Eintrag in der Liste auswählen und die `Entf`-Taste drücken.
- **Bearbeiten**: Ein Doppelklick auf einen Eintrag lädt die Daten zurück in die Maske.
- **Suche**: Das Suchfeld im Archiv filtert alle Spalten (Skip, Land, Kommentar, etc.) in Echtzeit.
- **Kontextmenü**: Rechtsklick in Textfelder für Ausschneiden, Kopieren und Einfügen.

## Konfiguration

Alle Einstellungen (eigener Locator, Rufzeichen, Pfade für den Auto-Import) können bequem im Tab **Setup** vorgenommen werden. Die Konfiguration wird in `settings.json` gespeichert.

## Haftungsausschluss

Die Nutzung erfolgt auf eigene Gefahr. Bitte erstelle regelmäßig manuelle Sicherheitskopien der Datei `funk_log.db`.

---
*Entwickelt für die Funk-Community - Mai 2026*