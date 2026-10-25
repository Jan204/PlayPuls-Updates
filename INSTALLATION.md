# PlayPuls 0.0.0.5 einrichten

Windows 64-Bit (x64). [Download](https://github.com/Jan204/PlayPuls-Updates/releases/tag/v0.0.0.5) · [Patchnotes und Hilfe](https://github.com/Jan204/PlayPuls-Updates/releases/download/v0.0.0.5/readme.txt) · [VirusTotal und SmartScreen](VIRUSTOTAL_0.0.0.5.md)

Installer verwenden oder das Portable-ZIP vollständig entpacken und PlayPuls.exe öffnen. Zugehörige Unterordner müssen erhalten bleiben.

## Erste Schritte

### 1. Mit Discord anmelden

Oben in der App auf „Mit Discord anmelden“ klicken. Im Browser mit deinem eigenen Discord-Konto anmelden und die Freigabe für PlayPuls bestätigen. Danach zur App zurückkehren. Oben erscheint dein Name.

### 2. Community, Server und Bereich / Hof wählen

Unter Spielwelt → Server die gewünschte Community, den LS-Server und den Bereich / Hof auswählen. Fehlt die Auswahl, muss dir die Communityverwaltung den passenden Zugriff freigeben.

### 3. Spiel und Modordner vorbereiten

LS25 vollständig schließen. In Einstellungen das LS25-Profil und die Spielanwendung prüfen. Unter Tools → Modordner ein Ordnerprofil mit Name und Pfad anlegen oder auswählen und aktivieren. Die optionale Zuordnung bestimmt, zu welchem Server der Ordner gehört. Ohne Zuordnung bleibt der lokale Spielstart möglich. Über die Ordnereinstellungen „PlayPuls Mod herunterladen und einfügen“ wählen. Host und Mitspieler benötigen dieselbe Mod-ZIP.

Alternativ unter Einstellungen → Mod & Updates → „PlayPuls Mod speichern unter…“ die Mod an einem beliebigen Ort speichern und selbst in den Modordner kopieren. Vorhandene Moddateien nur bei geschlossenem Spiel ersetzen.

### 4. LS25 starten

Die PlayPuls-Mod für den gewünschten Spielstand aktivieren und den Spielstand laden. Für Online-Funktionen muss die App geöffnet bleiben. Offline kannst du die Mod ohne App verwenden.

### 5. Eigenen Verbindungscode anfordern

In der App Einstellungen → Mod & Updates → Mod-ID · Eigene Spielverbindung öffnen. Die Community und den Server prüfen; bei Bedarf über „Community / Server wählen…“ ändern. „Eigenen Code anfordern“ und anschließend „Kopieren“ wählen. Der Code ist fünf Minuten gültig und gehört zu deinem Konto. Nicht weitergeben.

### 6. Code in der Mod eingeben

Mit Strg+P das PlayPuls-HUD öffnen. Mit der mittleren Maustaste den Mauszeiger aktivieren. Im HUD „Einstellungen“ öffnen, den Code eingeben und „Discord verbinden“ wählen. Die bestätigte Verbindung abwarten.

Discord-Anmeldung in der App und Spielverbindung per Code sind zwei getrennte Schritte. Die bestätigte Spielverbindung bleibt auf diesem PC gespeichert. Bei unveränderter und weiterhin berechtigter Zuordnung brauchst du nach einem normalen Neustart keinen neuen Code. Bei einer anderen Community, einem anderen Server oder Aufgabenbereich einen neuen Code anfordern und in der Mod eingeben. Ein neuer Code kann die alte Verbindung ersetzen. Ein Hofwechsel innerhalb desselben Aufgabenbereichs benötigt keinen neuen Code.


## Offline-Modus

Im Mod-HUD unter Einstellungen „Offline-Modus“ einschalten. Aufgaben und Handelsaufträge werden auf diesem PC je Spielstand und Spielhof gespeichert. Der Fuhrpark kommt direkt aus dem Spiel. App und Verbindungscode sind dafür nicht nötig. Es werden keine Daten zur Webseite übertragen.

Für eine spätere Übertragung die App öffnen, das gewünschte Ziel auswählen und einen neuen Code in der Mod verbinden. Erst nach ausdrücklicher Bestätigung in der App werden offene lokale Planungen als neue offene Einträge übertragen. Passende Ziele und Früchte müssen im Online-Bereich vorhanden sein. Erledigte Arbeitsschritte, Lieferungen und Geld werden nicht nachgebucht. Lokale Planungen werden nicht zwischen Mitspielern verteilt.


## Serververwaltung und Sync

Unter Tools → Serververwaltung einen Server mit Name, Adresse, zugeordnetem Modordner und Webinterface-Zugang anlegen. Die Anzeige und verfügbaren Aktionen richten sich nach den tatsächlich bestätigten Webinterface-Rechten. Das Administratorpasswort benötigt Game-Admin-Berechtigung.

HTTP bleibt nutzbar, überträgt Daten jedoch unverschlüsselt. Nutze HTTPS, wenn dein Webinterface es anbietet.

Sync einschalten, um den Serverstand alle drei Minuten abzugleichen. Beim 1:1-Sync hat der Server Vorrang: Auch lokal geänderte Mod-ZIPs werden durch den Serverstand ersetzt; zusätzliche lokale Mod-ZIPs werden entfernt. Andere Dateien und Unterordner bleiben bestehen. Sichere eigene Modänderungen vorher außerhalb dieses Ordners. Während LS25 läuft, wartet der automatische Download.

Ein früher eingerichteter ergänzender Abgleich wird erst durch bewusstes Aus- und Wiedereinschalten von Sync auf 1:1 umgestellt. Manuelle Mod-Downloads bleiben ergänzend.


## Bedienung und Hilfe

- Strg+P: HUD ein- oder ausblenden.
- Mittlere Maustaste: Mausfunktion bei geöffnetem HUD ein- oder ausschalten.
- HUD-Kopfzeile ziehen: HUD verschieben.
- „Alle Anzeigen“: größere Übersicht zum gewählten Reiter öffnen.
- „Version 0.0.0.5“ unter Info & Hilfe: diese Datei öffnen.

Wenn Daten fehlen, zuerst Community, Server, Bereich / Hof und Rechte prüfen. Anschließend den Verbindungsstatus unter Einstellungen → Verbindung & Diagnose ansehen. Bei einem abgelaufenen Code einen neuen anfordern. „Verbindung trennen“ entfernt den lokalen Zugang auch dann, wenn eine Online-Abmeldung nicht bestätigt werden kann.

Im Offline-Modus werden keine Kontodaten aus der Webseite geladen. Eine leere Offline-Liste bedeutet nicht, dass Online-Aufgaben gelöscht wurden. Neue Offline-Planungen bleiben getrennt von den Online-Daten.

Ist das Spiel noch geöffnet, können Modinstallation, Ordnerwechsel und automatische Downloads warten. LS25 vollständig beenden und danach erneut versuchen.

Nach Updates wird diese Datei nicht automatisch geöffnet. Du kannst sie jederzeit über Info & Hilfe → Version 0.0.0.5 aufrufen. Der interaktive Installer bietet „readme.txt öffnen?“ als freiwillige, zunächst nicht aktivierte Auswahl an.

Weitere Anleitung und FAQ: https://play-puls.de/ls-tool
PlayPuls: https://play-puls.de
Game News, Guides uvm.: https://dein-gamepuls.de


## Programm aktualisieren

Unter Einstellungen auf „Updates prüfen“ klicken. Bei einem verfügbaren neueren Update mit „Ja“ herunterladen oder mit „Später“ aufschieben. Nach dem geprüften Download „Jetzt neu starten“ oder „Später neu starten“ wählen. Ein automatisch heruntergeladenes Update wartet ebenfalls auf die Neustartbestätigung. Während LS25 läuft, wird nicht installiert.

Wer bereits ein lokales Testpaket 0.0.0.5 nutzt, installiert den öffentlichen Installer manuell: Dieselbe Versionsnummer löst keinen automatischen Versionshinweis aus. Beim Portable-Paket einen frisch entpackten Ordner verwenden. Host und Mitspieler benötigen dieselbe Mod-ZIP; dieselbe Versionsnummer allein genügt bei unterschiedlichen Dateien nicht.

## Automatische Feldübertragung

App und Mod auf 0.0.0.5 aktualisieren. Nach der Code-Verbindung werden vollständige, frische Dedicated-Feldproben automatisch zur Website übertragen. Die App übernimmt eine von der Websiteverwaltung eingerichtete Feldquelle und Serverzeitzone automatisch. Zusätzliche Kennungseingabe und Ingame-Admin-Anmeldung sind nicht erforderlich. Im Offline-Modus erfolgt keine Feldübertragung.

[Bekannte Einschränkungen und Patchnotes](PATCHNOTES_0.0.0.5.md).
