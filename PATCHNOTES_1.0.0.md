# PlayPuls 1.0.0

PlayPuls bekommt eine neue Windows-Oberfläche. Die Übersicht zeigt den Serverstatus und den Datenstand auf einen Blick. In der Serververwaltung, bei Aufgaben, im Modordner und in den Logs stehen Liste und Details nebeneinander.

[Anleitung, Bilder und FAQ · PlayPuls · GamePuls](https://play-puls.de/ls-tool)

## Windows-App

- **Serverübersicht.** Online und Offline haben kompakte Statusmarken mit Punkt. Aktuell und Veraltet erscheinen als farbiger Text. Ein Klick auf einen Spaltenkopf sortiert die Tabelle. Ein weiterer Klick kehrt die Richtung um.
- **Serververwaltung und Modordner.** Breitere Listen lassen lange Profilnamen umbrechen. Das Entfernen eines lokalen Profils ist direkt erreichbar und wird weiterhin bestätigt. Bei freigegebener Serversteuerung bietet ein bestätigter Offline-Server „Starten“ und ein Online-Server „Stoppen“.
- **Aufgaben, Handel und Fuhrpark.** Aufgaben zeigen Ziel, Tätigkeit und Status in der Liste. Die Details und verfügbaren Aktionen stehen rechts. Bei leerem Fuhrpark erklärt die App, ob der Filter keine Treffer hat, sichtbare Fahrzeuge im gewählten Hof fehlen oder keine Datenquelle verfügbar ist.
- **Fuhrpark ohne laufendes Spiel.** Unter Server und Höfe zeigt die App berechtigten Administratoren mit Premium oder Lifetime den gespeicherten FTP-Fuhrpark mit Speicherslot und Abrufzeit. Bei ausgewähltem Hof gelten die vorhandenen Hofzuordnungen. Über „Aktualisieren“ kann der gespeicherte Spielstand erneut abgerufen werden. Bei aktiver Spielverbindung nutzt der Fuhrpark die bisherigen Spielmeldungen und Serverquellen.
- **Hofbestand unter Server und Höfe.** Der neue Reiter zeigt eigene Felder, Grundstücke, Tiere, Produktionen und sonstige Anlagen aus dem gespeicherten FTP-Spielstand. Der letzte berechtigte Stand wird verschlüsselt lokal gespeichert und beim Öffnen angezeigt, während der Abgleich im Hintergrund läuft. Speicherslot und Abrufzeit erscheinen kurz am Fensterrand. Für Felder ist eine eindeutige Feld-zu-Grundstück-Zuordnung im Spielstand erforderlich. Der Hofbestand benötigt eine Desktop-API mit Unterstützung für den neuen Abruf.
- **Darstellung der Serverübersicht.** Die Serverliste hat einen einfachen Rahmen, die Online- und Offline-Marken sind geglättet, und die Spielstart-Schaltflächen haben flache Kanten.
- **Logs und Einstellungen.** Logs zeigen die vollständige ausgewählte Meldung neben der Liste. In den Einstellungen stehen Spielverbindung, Tool-Updates und Mod-Updates in getrennten Bereichen.
- **Darstellung.** Neue Profile folgen standardmäßig dem Windows-Farbschema für Apps. In den Einstellungen stehen Hell, Dunkel und Windows sowie die Akzentfarben Blau, Rot, Gelb und Grün zur Auswahl. Änderungen erscheinen als Sofortvorschau. Die Linie unter einem Reiter wächst beim Überfahren von der Mitte nach außen. Das passende Hofmotiv liegt hinter den Tabellenzeilen in Aufgaben, Handel, Fuhrpark und Hofbestand. Es lässt sich ein- und ausblenden. „Auf Standard zurücksetzen“ wählt Windows, Blau und den eingeblendeten Hintergrund.
- **Serverübersicht und Hofbestand.** Die Übersicht zeigt beim Laden den letzten gespeicherten Serverstand. Das Hintergrundbild liegt gedämpft hinter der gesamten Serverliste und scheint auch unter den Zeilen durch. Im Hofbestand lassen sich Einträge suchen und nach den vorhandenen Angaben filtern. Die Spalte „Tierart“ nutzt die Kennungen aus dem FTP-Spielstand, sobald die Desktop-API sie liefert.
- **Schnellerer Seitenwechsel.** Bereits geöffnete Ansichten erscheinen beim Zurückwechseln mit ihrer bisherigen Auswahl und Scrollposition. Neue Daten werden in der vorhandenen Ansicht aktualisiert. Die Spielwelt baut weitere Reiter erst bei ihrem ersten Aufruf auf.
- **Hofbestand und Tools.** Suche und Filter stehen unter den Kategorien direkt über der Tabelle. Ein Rechtsklick auf einen Hofbestandseintrag öffnet die Auswahl zum Erstellen einer Aufgabe oder eines Handelsauftrags mit vorausgefüllten Angaben. Das Hofmotiv erscheint hinter den Zeilen der Logtabelle und um die einheitlichen Detailkarten in Modordner und Serververwaltung. Die Ladeanzeige sitzt in der Statuszeile und verwendet die Akzentfarbe.
- **Versionsübersicht.** Unter „Info & Hilfe → Version“ und am Ende der Installation lässt sich die Versionshistorie im Browser öffnen. Frühere Stände sind direkt erreichbar und aufklappbar.

## ModHub und Modabgleich

- **ModHub im lokalen Spiel.** Der ModHub-Reiter der Mod lädt die öffentliche Liste, solange die Windows-App geöffnet ist. Spielstanddaten und lokale Planungen bleiben dabei lokal.
- **Vorschau vor dem 1:1-Abgleich.** Beim Einschalten oder Fortsetzen von Sync erscheint die Vorschau nur bei Änderungen und geschlossenem LS25. Bei gleichem Bestand wird Sync direkt aktiv. Läuft das Spiel, wartet die App mit der Prüfung. Für das Hochladen einer lokal gewählten Version bleibt eine separate Bestätigung erforderlich.

## Installation

App und Setup tragen die Version **1.0.0**. Enthalten ist die **PlayPuls-Mod 0.0.0.7**. Wer bereits ein 1.0.0-Testsetup verwendet, installiert das freigegebene Setup manuell. Die automatische Updateprüfung bietet nur höhere Versionsnummern an.
