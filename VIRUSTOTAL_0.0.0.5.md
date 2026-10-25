# PlayPuls 0.0.0.5 – VirusTotal, SmartScreen und Datenzugriff

Prüfstand: 25.10.2026, Europe/Berlin. Die Berichte gelten ausschließlich für
die genannten SHA-256-Prüfsummen. Die Verdachtsmeldungen sind **nicht als
Fehlalarme bestätigt**; die Prüfung ist keine Sicherheitsgarantie.

## Geprüfte Dateien

Installer und enthaltene Programmdatei wurden separat geprüft. Die geprüfte
EXE ist bytegleich mit der EXE im getesteten Installer und Portable-Paket.
Bei veränderten Dateien sind neue dateispezifische Prüfungen erforderlich.

| Datei | SHA-256 | Bericht |
| --- | --- | --- |
| Installer | `712108c13a3b1b7f73b5e081abf5bf74a387a51118aa871a2c66ea195b4331e3` | [1 von 69 Engines meldet einen Verdacht](https://www.virustotal.com/gui/file/712108c13a3b1b7f73b5e081abf5bf74a387a51118aa871a2c66ea195b4331e3) |
| PlayPuls.exe | `8ba7234d3c2fe5817fc168e316d5ac0e998cc8bf89aaad9e494a29bf35519590` | [4 von 71 Engines melden einen Verdacht](https://www.virustotal.com/gui/file/8ba7234d3c2fe5817fc168e316d5ac0e998cc8bf89aaad9e494a29bf35519590) |

Analysezeiten: Installer 25.10.2026 – 01:58:17; EXE 25.10.2026 – 01:49:32
(Europe/Berlin).

Installer: Trapmine meldet `Suspicious.low.ml.score`; 68 Engines ohne Erkennung.
ClamAV und TEHTRIS: Zeitüberschreitung. Avast-Mobile, BitDefenderFalx,
Symantec Mobile Insight und Trustlook: Dateityp nicht unterstützt.

Programmdatei: 67 Engines ohne Erkennung. Gemeldete Funde:

| Engine | Bezeichnung |
| --- | --- |
| Arctic Wolf | `Unsafe` |
| Microsoft | `Trojan:Win32/Wacatac.C!ml` |
| SecureAge | `Malicious` |
| Skyhigh (SWG) | `BehavesLike.Win64.Backdoor.vc` |

Avast-Mobile, BitDefenderFalx, Symantec Mobile Insight und Trustlook unterstützen
den Dateityp nicht. Nicht verwertbare Ergebnisse zählen nicht als „sauber“.

Portable-Archiv: 1 von 66 Engines meldet einen Verdacht; Zillya meldet
`Trojan.Blank.Script.2228`. Analysezeit: 25.10.2026 – 02:01:20 (Europe/Berlin).
ClamAV: Zeitüberschreitung; Trustlook: Prüfungsfehler. Arctic Wolf,
BitDefenderFalx, Palo Alto Networks, SecureAge, Symantec Mobile Insight,
TEHTRIS und Trapmine unterstützen den Dateityp nicht.

Ein Archivbericht ersetzt keine
Prüfung aller enthaltenen Dateien: VirusTotal weist bei diesem Mehrdateien-ZIP
über 3 MiB auf Einschränkungen beim Scannen des Archivinhalts hin.
[Portable-Bericht](https://www.virustotal.com/gui/file/07c253b76cf79b930d19f91917dbc8373ecc38888f5372c7b9752f1196f1a1a8).

## Mögliche technische Erklärung – kein Ursachenbeweis

Die App wird mit **PyInstaller 6.22.3** als Windows-Programm gebündelt, der
Installer mit NSIS erstellt. Der gemeinsame Python-Startcode solcher Pakete
kann auch in schädlicher Software vorkommen. Das PyInstaller-Projekt beschreibt
bekannte Antivirus-Fehlalarme bei gebündelten Anwendungen und verweist zur
Klärung an die jeweiligen Sicherheitsanbieter.
[Hinweis der PyInstaller-Maintainer](https://github.com/pyinstaller/pyinstaller/issues/6062).

Das ist eine plausible Erklärung für heuristische Erkennungen, **kein Nachweis,
dass genau diese Meldungen falsch sind**. Auch Bezeichnungen mit `ml` oder
`BehavesLike` erlauben keine abschließende Entwarnung. Funktionstests, der
Abgleich der gebündelten App-Module mit dem Quellstand und bestandene
Funktionstests belegen die geprüfte Funktion und Herkunft des Builds; sie ersetzen
keine unabhängige Sicherheitsprüfung. Die Binärdateien wurden nicht verändert,
um Erkennungen zu umgehen. Eine Herstellerprüfung der Funde steht aus.

## Welche Daten PlayPuls tatsächlich liest

„PlayPuls liest keine Daten“ wäre falsch. Die Funktionen benötigen folgende
Zugriffe; sie sind von einem Auslesen privater Browserdaten zu unterscheiden:

- **Anmeldung und Rechte:** Die App erhält nach der Discord-Freigabe über die
  PlayPuls-API die zugehörige Kontozuordnung und berechtigten Community-/Server-/
  Hofdaten. Die Discord-Anmeldung erfolgt im Browser.
- **LS25 und Modordner:** Gewählte Profilpfade, Spielkonfiguration und Mod-ZIPs
  werden für Ordnerauswahl, Versionsprüfung und Installation gelesen. Beim
  aktivierten 1:1-Sync werden abweichende ZIPs ersetzt und zusätzliche Mod-ZIPs
  gelöscht. Das ist eine ausdrücklich aktivierte Verwaltungsfunktion.
- **Spieldaten:** Die Mod liest unter anderem Fahrzeuge, Füllmengen, Felder,
  Früchte, Grundstücke und Spielhofzuordnungen für die angebotenen Anzeigen und
  Abgleiche. Vollständige, frische Feldzustände des Dedicated-Servers werden bei gültiger
  Code-Verbindung über die App automatisch an die eingerichtete Website-Feldquelle
  übertragen. Karten-, Slot- und Sitzungsgrenzen bleiben erhalten.
- **Aufgaben und Handel:** Online werden berechtigte Daten im gewählten Kontext
  geladen und bestätigte Aktionen an die PlayPuls-API übertragen. Die Mod schreibt
  dazu lokale Austauschdateien; die App verarbeitet die passende Sitzung.
- **Serververwaltung:** Der Nutzer richtet einen GIANTS-Webinterface-Zugang ein.
  Die App verwendet dafür eigene Sitzungscookies und liest freigegebene
  Serverinformationen einschließlich Join-/Adminpasswort nach aktueller
  Rechteprüfung. Das sind keine Cookies aus einem privaten Browserprofil.
- **Logs:** Die gewählte LS25-Logdatei wird auf Nutzeraktion lokal gelesen.
  Die Logansicht enthält keinen automatischen Upload der Logdatei.
- **Lokaler Schutz:** Konto-/Spielzugänge und Serverprofile werden mit dem
  vorhandenen Windows-DPAPI-Speicher geschützt. Verschlüsselung begrenzt den
  Zugriff, ist aber keine Garantie gegen Schadsoftware im selben Benutzerkonto.

In den hierfür geprüften App-Modulen finden sich keine Zugriffe auf Chrome-/
Firefox-Passwortspeicher, Browser-Verläufe oder private Browser-Cookie-Datenbanken.
`game_running()` prüft Prozessnamen, um ein laufendes LS25 zu erkennen; diese
Funktion liest keinen fremden Prozessspeicher. Diese gezielte Quellprüfung ist
kein vollständiges Audit sämtlicher Drittanbieterbibliotheken.

Im **Offline-Modus der Mod** bleiben Aufgaben und Handel lokal. Es werden
keine Mod-Spieldaten an die Webseite übertragen. Nach einer späteren Verbindung
werden offene lokale Planungen erst nach ausdrücklicher Bestätigung übernommen.
Die separat geöffnete App kann unabhängig davon ihre aktivierten Online-Funktionen
nutzen, beispielsweise Serverabgleich oder öffentliche ModHub-/Updateabrufe.

## SmartScreen: Herausgebersignatur ist keine Nutzungslizenz

Installer und EXE haben im geprüften Stand **keine Authenticode-
Herausgebersignatur** (`Get-AuthenticodeSignature`: `NotSigned`). SmartScreen
berücksichtigt Signaturen und die Reputation des konkreten Dateihashes.
Eine neue oder unsignierte Datei kann daher als unbekannte App erscheinen.
Das erklärt eine mögliche Ursache der Meldung „Der Computer wurde durch Windows
geschützt“; die Meldung beweist weder Schadcode noch Unbedenklichkeit und
entkräftet die obigen VirusTotal-Funde nicht.
[Microsoft zur SmartScreen-Reputation](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation).

Davon getrennt gelten die [PlayPuls-Nutzungsbedingungen](https://play-puls.de/nutzungsbedingungen)
und die mitgelieferten Fremdsoftware-Lizenztexte im Ordner `licenses`
(Python, Tk, PyInstaller und cryptography). Eine Nutzungslizenz ist kein
Windows-Signierzertifikat. Signierte Updateinformationen und SHA-256-Prüfsummen
prüfen Herkunft beziehungsweise Integrität im jeweiligen Verfahren, ersetzen
aber weder eine Authenticode-Signatur noch eine Schadsoftwareprüfung.

Der [Datenschutzhinweis für das LS-Tool](https://play-puls.de/datenschutz)
beschreibt die Verarbeitung. Dieser technische Nachweis ändert keine Lizenz
und gibt keine zusätzlichen Nutzungsrechte.
