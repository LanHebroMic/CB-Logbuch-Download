# CB-Logbuch v1.3.1
**Entwickler: LanHebroMic**

Ein modernes und effizientes Logbuch-Programm für CB-Funk und Amateurfunk, entwickelt in Python mit Tkinter.

## Features

- **QSO-Management**: Schnelle Erfassung von Funkkontakten mit automatischer Entfernungsberechnung (Maidenhead Locator) und Länder-Combobox mit allen verfügbaren Ländern.
- **SOTA / POTA / BOTA / IOTA / WWFF**: Volle Unterstützung für spezielle Funk-Referenzen – auch für die eigene Aktivierer-Seite (MY_SOTA_REF, MY_POTA_REF, MY_WWFF_REF).
- **ADIF-Standard (72 Felder)**: Vollständiger Import und Export nach ADIF v3 – inkl. DXCC, CQ-/ITU-Zone, Kontinent, GPS-Koordinaten, LoTW/eQSL-Status, Funkwetter (A/K-Index, SFI), QSL-Nachricht, TIME_OFF und alle Contest-Felder.
- **Solar-Wetter & Propagation**: Live-Abfrage von SFI, A- und K-Index inkl. automatischer Bewertung der Ausbreitungsbedingungen für das aktive Band.
- **Erweitertes CAT-Interface**: Unterstützung für Hamlib (`rigctld`) mit automatischem Hintergrund-Start, Modellauswahl und bidirektionaler Synchronisation von Frequenz und Modus.
- **Split-Betrieb**: Getrennte Erfassung von RX- und TX-Frequenzen sowie gesendeten Rapporten.
- **Automatische Ländererkennung**: Bestimmung des Landes anhand von Rufzeichen-Präfixen und CB-Divisionen während der Eingabe.
- **Auto-Import**: Überwacht ADIF-Dateien von Drittsoftware (WSJT-X, JS8Call, WSJT-CB) und importiert neue Kontakte automatisch mit intelligenter Dublettenprüfung.
- **Live-ADIF Export**: Schreibt QSOs in Echtzeit in eine ADIF-Datei für externes Logging (Thread-sicher via Queue).
- **Contest-Modus**: Vollständiges Contest-Logging mit Dublettenprüfung, Zeitfenster-Überwachung, Exchange-Feldern und Export als ADIF oder Cabrillo.
- **Datenbank**: SQLite für lokale Speicherung oder optional MySQL – beide werden beim Start automatisch auf neue Felder migriert.
- **Backup-System**: Erstellt beim Beenden automatisch Backups der Datenbank (max. 10 rotierende Backups).
- **Export/Import**: ADIF (vollständig/selektiert/Contest), CSV (Excel-kompatibel, UTF-8-BOM) und Cabrillo.
- **Kartenansicht**: Visualisierung von Kontakten auf einer Weltkarte mit optionaler Offline-Unterstützung und Klick-Statistiken für Locator-Regionen.
- **Update-Check**: Automatische Prüfung auf neue Versionen beim Programmstart direkt über die GitHub-API.
- **Modernes UI**: Unterstützung verschiedener Design-Themes, Kontextmenüs für alle Textfelder und dynamische Spaltenanpassung.

## Installation

### Windows
1. Paket herunterladen.
2. `CB-Logbuch_Setup_1.3.1.exe` per Doppelklick starten.

Dadurch wird das Programm im Startmenü registriert und alle Abhängigkeiten automatisch installiert.

### Linux (Debian/Ubuntu/Raspberry Pi OS)
Der einfachste Weg ist das Debian-Paket:
1. Paket herunterladen.
2. Installieren mit:
   ```bash
   sudo apt install ./cb-logbuch_1.3.1_all.deb
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

Die Nutzung erfolgt auf eigene Gefahr. Bitte erstelle regelmäßig manuelle Sicherheitskopien der Datenbank. Für MySQL-Datenbanken obliegt die Sicherung dem Nutzer. Weitere Details im Programm unter **Info → Haftungsausschluss**.

---
*Entwickelt für die Funk-Community – Juni 2026 · v1.3.1*
