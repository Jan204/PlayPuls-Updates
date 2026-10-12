# PlayPuls einrichten

App und LS25-Mod: **0.0.0.2**. Voraussetzung ist ein Windows-PC mit 64 Bit und eine PlayPuls-Community, in der du für die gewünschten LS-Bereiche berechtigt bist.

## 1. Programm starten

Lade das freigegebene Paket auf der [Download-Seite](https://github.com/Jan204/PlayPuls-Updates/releases/latest).

- **Installer:** `PlayPuls-0.0.0.2-Setup.exe` installiert die App für dein Windows-Benutzerkonto.
- **Portable:** `PlayPuls-0.0.0.2-Portable.zip` vollständig entpacken. Öffne `PlayPuls.exe` im entpackten Ordner; die zugehörigen Unterordner müssen erhalten bleiben.

Melde dich über **Mit Discord anmelden** mit deinem eigenen Konto an. Wähle oben die **Discord-Community**, den **LS-Server** und den **Aufgabenbereich/Hof**. Sichtbar sind nur Bereiche, für die du berechtigt bist.

## Übersicht und Kennzahlen

Oberhalb der Servertabelle stehen die Kennzahlen für den ausgewählten Bereich/Hof:

- **Aufgaben Offen / Gesamt:** Offen zählt Aufgaben mit dem Status „Offen“. Gesamt umfasst alle sichtbaren, nicht archivierten Aufgaben einschließlich erledigter Aufgaben.
- **Handel Offen / Gesamt / Angeboten:** Offen und Gesamt zählen die sichtbaren, nicht archivierten Handelsaufträge. Angeboten zählt deine selbst erstellten, noch offenen Angebote.
- **Fuhrpark Anzahl:** Anzahl der Fahrzeuge und Geräte in der berechtigten Fuhrparkansicht. Jede aufgeführte Meldung zählt.

Halte den Mauszeiger über eine Überschrift, Zahl oder Beschriftung für eine kurze Erklärung. „—“ bedeutet, dass die Zählwerte noch nicht aktuell geladen oder nicht freigegeben sind. Alte Summen aus dem lokalen Cache werden erst nach einem aktuellen Abgleich angezeigt. Die Gesamtzahlen sind nicht auf die erste Listenseite mit 50 Einträgen begrenzt.

## 2. LS25 und den Modordner auswählen

In **Einstellungen** kannst du das LS25-Profil unter `Documents\My Games\FarmingSimulator2025` und die Spielanwendung auswählen.

Unter **Tools → Modordner** verwaltest du benannte Profile für unterschiedliche Server oder Maps. Nur der aktive Ordner wird von LS25 geladen. Vor einem Wechsel muss LS25 vollständig geschlossen sein; die Spielkonfiguration wird vor der Anpassung gesichert.

Über die Einstellungen eines Ordnerprofils kannst du **Mod herunterladen und einfügen** wählen. Das zum Programm gehörende, geprüfte Modpaket wird in diesen Ordner eingefügt. Alternativ kopiere `FS25_PlayPuls.zip` aus dem Release in den gewünschten Modordner. Eine vorhandene Datei erst ersetzen, wenn das Spiel geschlossen ist.

Für Multiplayer müssen Host und Mitspieler das identische Modpaket verwenden. Dieselbe Versionsnummer allein reicht bei unterschiedlichen Dateien nicht aus.

## 3. Spielverbindung herstellen

Fordere in **Einstellungen → Mod-ID** einen eigenen Verbindungscode an. Starte LS25, aktiviere die PlayPuls-Mod und löse den Code in den Einstellungen des Spiel-HUDs ein.

Die bestätigte Verbindung bleibt auf dem PC gespeichert. App- oder Spielneustarts benötigen keinen neuen Code, solange die Verbindung gültig und berechtigt ist. Die App muss während der Datenübertragung geöffnet bleiben. Der Code bindet die Verbindung an deine gewählte PlayPuls-Zuordnung; er ersetzt keine LS25-Anmeldung oder PlayPuls-Berechtigung.

## 4. HUD und App bedienen

- **Strg+P:** HUD ein- oder ausblenden. Beim Start ist es sichtbar.
- **Mittlere Maustaste:** Mausfunktion öffnen oder beenden, wenn das HUD sichtbar ist.
- **Kopfzeile ziehen:** HUD verschieben; die Position wird lokal gespeichert.
- **Aufgaben:** Zeile auswählen oder für Details doppelklicken. Verfügbare Aktionen richten sich nach Aufgabe und Berechtigung.
- **Aufgaben im HUD:** Ziel, aktuelle Tätigkeit, Beschreibung, Ersteller und Übernahme/Zuweisung ansehen. Neue Aufgaben benötigen Titel, Ziel und Tätigkeit.
- **Spielhöfe zuordnen:** In den HUD-Einstellungen die Hofliste laden, Spielhof und PlayPuls-Hof durch Anklicken wechseln und die Zuordnung speichern. Dafür sind passende Hofmeister- oder Administratorrechte erforderlich. Die Zuordnung wird mit App und Webseite geteilt und vergibt keine zusätzlichen Nutzerrechte.
- **Logs:** Manuell einlesen; gelbe Warnungen und rote Fehler suchen, filtern und exportieren.
- **Einstellungen:** Programmupdates prüfen, Status ansehen und ein verfügbares Update herunterladen.
- **Stammdaten:** Du kannst Stammdaten weiterhin im Web selbst anlegen und bearbeiten. Im Spiel unter Einstellungen „Stammdaten synchronisieren“ wählen. Nur dieser manuelle Vorgang ergänzt fehlende Felder, Früchte, Grundstücke und eigene Produktionen im erlaubten Aufgabenbereich. Vorhandene Namen und deaktivierte Einträge bleiben erhalten. Bereichsverwalter oder Administrator müssen die Aktion ausführen. Größere Imports werden in begrenzten Paketen übertragen; bei einer Unterbrechung wird der bisherige Fortschritt angezeigt und du kannst den Vorgang erneut manuell starten.
- **Handel:** Artikel aus den vorhandenen Web-Stammdaten wählen oder manuell eingeben. Menge, Einheit, Preisart, Beschreibung und Frist lassen sich nach aktuellen Rechten bearbeiten.
- **Fuhrpark:** Mehrere Fahrzeuge und Geräte mit gemeldeten Füllmengen, Kapazitäten und Einheiten ansehen. Nicht verfügbare Werte bleiben als „—“ gekennzeichnet.
- **Im Hintergrund starten:** „Beim Start minimieren“ in den Einstellungen aktivieren. Das Symbol neben der Uhr öffnet per Klick die App; sein Rechtsklickmenü bietet Öffnen und Beenden.

Sichtbare Arbeitsansichten werden automatisch etwa alle 15 Sekunden abgeglichen. Manuelles Aktualisieren unterliegt einer gemeinsamen Wartezeit von drei Sekunden je Community. Berechtigte lokale Daten können nach Rechteprüfung sofort erscheinen, während der aktuelle Stand im Hintergrund geladen wird.

## Wenn etwas fehlt

Prüfe zuerst Community, Server und Aufgabenbereich sowie deinen oben angezeigten LS-Rang. Fehlende Hofrechte oder eine fehlende Zuordnung können Aktionen einschränken. Prüfe danach die Spielverbindung in den Einstellungen und die Hinweise in der Fußzeile.

Bei einem längeren Verbindungsproblem bleiben zulässige letzte Daten lesbar; Schreibaktionen benötigen einen frischen Stand. Eine abgelehnte Berechtigung kann die private Ansicht entfernen.

Der Wechsel von der früheren Version `0.0.1` zur Versionsreihe `0.0.0.2` erfolgt über das vollständige Installationspaket. Der automatische Versionsvergleich betrachtet `0.0.1` als `0.0.1.0` und installiert deshalb `0.0.0.2` nicht als neueres Update.

EXE und Installer besitzen derzeit keine Windows-Herausgebersignatur (Authenticode). Die Prüfung der Updateinformationen und Dateiprüfsummen ersetzt diese Signatur nicht.

Zu Installer, Portable-ZIP, Mod-ZIP und `update.json` wird jeweils eine `.sha256`-Datei bereitgestellt. Der Updater prüft zusätzlich die digital signierten Updateinformationen und den SHA-256-Hash des heruntergeladenen Installers. Eine Prüfsummendatei allein schützt nicht gegen einen Austausch von Datei und Prüfsumme.

[Weitere Informationen und FAQ](https://play-puls.de/ls-tool)

## Monatsreminder und Rechtstexte

Aktiviere die Erinnerung einer Aufgabe und wähle den Erinnerungsmonat. Ohne eigenen Erinnerungsmonat gilt der Aufgabenmonat. Die App verwendet dieselben Monatsnamen wie die Webverwaltung. Wird der passende LS25-Spielmonat erreicht, erscheinen ein kurzer HUD-Hinweis und eine hervorgehobene Aufgabenzeile. Der Aufgabenhinweis bleibt bis zur Erledigung beziehungsweise Änderung oder Deaktivierung der Erinnerung. Kurze Erfolgsmeldungen verschwinden nach drei Sekunden; Fehler bleiben erkennbar.

Installer und Portable-Paket enthalten die Fremdsoftware-Lizenzen im Ordner `licenses`. Die [Nutzungsbedingungen](https://play-puls.de/nutzungsbedingungen) und die [Datenschutzerklärung](https://play-puls.de/datenschutz#ls-tool) beschreiben das PlayPuls-Angebot und die Verarbeitung durch App und Mod.
