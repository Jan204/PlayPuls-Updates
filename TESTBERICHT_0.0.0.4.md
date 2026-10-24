# PlayPuls 0.0.0.4 – Prüfstand vom 24.10.2026

Dieser Nachweis betrifft das freigegebene Windows-x64-Setup und das darin enthaltene Modpaket 0.0.0.4. Historische Berichte gelten für ihre damaligen Dateien.

- App: vollständige lokale Suite **861 bestanden**; zunächst 14 gezielte Tests zu Hilfe, Installer und Build bestanden.
- Mod/Companion: **469 LS25-Regressionstests bestanden**, vor dem Git-Abschluss erneut ausgeführt.
- Installer isoliert installiert: 1.028 Dateien bytegleich mit dem geprüften Paket. Readme im Programmordner und als Hilfedatei sowie beide Portable-Kopien bytegleich.
- Binärer Selbsttest mit isoliertem Profil bestanden; 30 eingefrorene App-Module und 16 Modquelldateien mit dem Quellstand abgeglichen.
- Isoliertes Upgrade und Deinstallation bestanden; fremde synthetische Benutzerdatei blieb erhalten.
- Offline-Aufgabe, Handel, Fuhrpark und Neustart wurden im lokalen Spiel ohne geöffnete App geprüft. Kein Nachweis einer Verteilung zwischen Mitspielern.
- Öffentliches Release enthält SHA-256-Sidecars und signierte Updateinformationen; keine Authenticode-Herausgebersignatur.

## Grenzen

Ein gemeinsamer Test mit Host und weiterem Spieler bleibt offen. Die Tests sind kein unabhängiges Sicherheitsaudit. Der Feldexport schreibt bestätigte Werte lokal; ein neuer eigenständiger Website-Transport ohne App ist nicht enthalten. Die Fläche von Feld 135 wurde je nach Bezugsfläche mit 1.004731 bzw. 1.02 ha angezeigt; diese Abweichung ist nicht abschließend geklärt.

Die vollständige Bot-Gesamtsuite wurde für diesen Abschluss nicht nochmals ausgeführt: ihr vorheriger Lauf dauerte über 41 Minuten und enthält gesondert dokumentierte Befunde außerhalb dieses Auftrags. Der relevante LS25-Bereich wurde vollständig geprüft. Parallele Webänderungen gehören nicht zu diesem Release.

## Sicherheitsprüfung und Freigabe

Finaler Installer: **1/68**, enthaltene EXE: **5/70** bei VirusTotal. Funde sind nicht als Fehlalarme bestätigt. Jan hat die Veröffentlichung nach Mitteilung dieser Ergebnisse ausdrücklich freigegeben. Alle Fundnamen, nicht auswertbaren Engines, exakten Prüfsummen und Quellen stehen im [VirusTotal-Nachweis](VIRUSTOTAL_0.0.0.4.md). Die Binärdateien wurden danach nicht verändert.

Kein SSH, kein Serverdeployment, keine produktiven Datenänderungen oder Datenbankmigrationen in diesem Auftrag. GitHub-Release und Git-Upload sind die ausdrücklich freigegebenen Veröffentlichungen.
