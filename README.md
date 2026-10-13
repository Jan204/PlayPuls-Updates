# PlayPuls – LS25 Tool

Die PlayPuls-App für **Windows 64-Bit (x64)** verbindet deinen PC und die PlayPuls-Mod für Landwirtschafts-Simulator 25 mit deiner PlayPuls-Community. Eine 32-Bit-Ausgabe wird nicht angeboten.

**App und Mod: Version 0.0.0.2.** Installer, Portable-Paket und LS25-Mod stehen im öffentlichen Release zum Download bereit.

[Programm, Bilder und FAQ](https://play-puls.de/ls-tool) · [Downloads](https://github.com/Jan204/PlayPuls-Updates/releases/latest) · [Installationsanleitung](INSTALLATION.md)

## Was bietet das Tool?

- **Übersicht:** Aufgaben offen/gesamt, Handel offen/gesamt/deine offenen Angebote und die Fuhrparkanzahl für den ausgewählten Bereich/Hof. Mausover erklärt die Kennzahlen.
- **Ingame-Mod:** Aufgaben auswählen, übernehmen und Arbeitsschritte erledigen; Handelsaufträge und Fuhrpark direkt im Spiel ansehen.
- **Aufgabenverwaltung:** Aufgaben mit Ziel, Beschreibung, Früchten, Planung und Arbeitsschritten in der App bearbeiten. Aktivierte Monatsreminder erinnern an den passenden Spielmonat.
- **Handel:** Handelsaufträge und Lieferungen mit Artikeln, Mengen, Einheiten, Preisen und Fristen verwalten.
- **Fuhrpark:** Mehrere Fahrzeuge und Geräte mit gemeldeten Füllmengen und Einheiten übersichtlich als Tabelle anzeigen.
- **Höfe:** Spielhöfe mit berechtigten PlayPuls-Höfen verknüpfen und die Hofzuordnung in App oder Ingame-Einstellungen verwalten.
- **Stammdaten:** Felder, Früchte, Grundstücke und eigene Produktionen manuell aus dem Spiel ergänzen. Eigene Stammdaten weiterhin im Web anlegen und bearbeiten.
- **Modordner:** Eigene Ordnerprofile für verschiedene Server oder Maps auswählen und den passenden Modordner aktivieren.
- **Logauswertung:** Die LS25-Logdatei einlesen, Warnungen und Fehler suchen, filtern und exportieren.

Welche Daten und Aktionen verfügbar sind, hängt von deiner Discord-Community, deinem LS-Rang, deinen Hofrechten und dem Abo der Community ab. Die App zeigt diese Zuordnung oben an.

## Download und Installation

Für Windows mit 64 Bit. Im Release stehen der `.exe`-Installer, das Portable-`.zip` sowie die passende LS25-Mod bereit. Jede Download-Datei und `update.json` haben eine eigene `.sha256`-Prüfsummendatei. Für das Portable-Paket den gesamten Inhalt entpacken und anschließend `PlayPuls.exe` öffnen.

[Zur Installation und Einrichtung](INSTALLATION.md)

Die aktuellen Pakete verwenden **0.0.0.3**. Der Update-Dialog bietet **Download** oder **Abbrechen** und nach dem geprüften Download **Jetzt neu starten** oder **Später neu starten**. Wenn 0.0.0.3 bereits installiert ist, lade den korrigierten Installer erneut herunter und installiere ihn manuell. Derselbe Versionsstand löst keinen automatischen Updatehinweis aus.

## Häufige Fragen

### Muss PlayPuls während des Spiels geöffnet bleiben?

Ja. Die App stellt die Verbindung zwischen Mod, PC und PlayPuls bereit. Ohne laufende App werden keine neuen Moddaten übertragen.

### Brauche ich bei jedem Start einen neuen Code?

Nein. Die bestätigte Spielverbindung bleibt geschützt auf deinem PC gespeichert. Solange sie gültig und berechtigt ist, wird sie bei weiteren Starts wieder verwendet. Nach Trennen, Ablauf oder Widerruf ist eine neue Verbindung erforderlich.

### Kann ich für verschiedene Server unterschiedliche Mods nutzen?

Ja. Unter **Tools → Modordner** kannst du mehrere benannte Ordnerprofile speichern und aktivieren. LS25 lädt nur den aktiven Modordner. Schließe das Spiel, bevor du den Ordner wechselst oder das Modpaket ersetzt.

### Werden meine Logs automatisch hochgeladen?

Die Logansicht liest Dateien nur auf deine Aktion hin lokal ein. Die Originaldatei wird dabei nicht verändert. Warnungen und Fehler kannst du selbst exportieren.

### Wie funktionieren Updates?

Öffne **Einstellungen → Updates prüfen**. Ein verfügbares Update wird im Programm heruntergeladen und vor der Installation geprüft. Dafür muss ein veröffentlichtes Paket mit digital signierten Updateinformationen vorliegen. Der Updater prüft die Signatur sowie Dateigröße und SHA-256 des Installers. Prüfsummen allein ersetzen keine Signatur. Änderungen mit derselben Versionsnummer lösen kein Versionsupdate aus. Während LS25 läuft, wird kein Toolupdate installiert.

Ab 0.0.0.3 entscheidest du nach dem Download, ob du **Jetzt neu starten** oder **Später neu starten** möchtest. Bei „Später“ bleibt die App geöffnet; unter **Einstellungen → Update herunterladen** kannst du die Installation später fortsetzen. Die optionale Automatik lädt nur herunter und wartet ebenfalls auf deine Neustartbestätigung.

### Kann ich ohne Verbindung alle gespeicherten Daten verwenden?

Private Daten aus dem lokalen Cache werden erst nach aktueller Rechteprüfung angezeigt und im Hintergrund aktualisiert. Ohne erfolgreiche Prüfung gibt es keine private Offlineansicht. Für Änderungen sind aktuelle Daten und Berechtigungen erforderlich.

## PlayPuls und GamePuls

- [PlayPuls](https://play-puls.de): Discord-Bot und Webverwaltung für deine Community, LS-Server, Höfe, Aufgaben und Handel.
- [GamePuls](https://dein-gamepuls.de): Gaming-News, Guides und Tests rund ums Gaming.

## Hilfe

Hilfe bekommst du im [Discord](https://discord.gg/uMnajk3Fnp) oder über das [Kontaktformular](https://dein-gamepuls.de/kontakt-gamepuls/).
Du kannst auch auf [PlayPuls](https://play-puls.de) **Support** öffnen und ein Ticket erstellen.
