# PlayPuls 0.0.0.4 – VirusTotal, SmartScreen und Datenzugriff

Prüfstand: 24.10.2026, Europe/Berlin. Dieser Nachweis gilt ausschließlich
für die unten genannten SHA-256-Prüfsummen. Er ist keine Garantie, dass eine
Datei ungefährlich ist. Die Befunde sind **nicht als Fehlalarme bestätigt**.

## Warum zwei Dateien geprüft wurden

Installer und Programmdatei enthalten unterschiedliche ausführbare Strukturen.
Deshalb wurden der finale Installer und die darin enthaltene `PlayPuls.exe`
getrennt hochgeladen. Die geprüfte EXE stimmt mit der EXE im Installer und
Portable-Paket überein. Bei einer späteren Änderung der Binärdateien sind neue
Prüfungen nötig; eine unveränderte Versionsnummer reicht nicht als Nachweis.

| Datei | SHA-256 | Abschließender Bericht |
| --- | --- | --- |
| Installer | `c7997e2571d94055abf5732875042fe1f22ce3b45fe91df884f92fd0c7f7d274` | [2 von 69 Engines melden einen Verdacht](https://www.virustotal.com/gui/file/c7997e2571d94055abf5732875042fe1f22ce3b45fe91df884f92fd0c7f7d274) |
| PlayPuls.exe | `de35bff8f191f23051ccc13c70432627b034b6761707a6555fe1374df08ddcb6` | [5 von 70 Engines melden einen Verdacht](https://www.virustotal.com/gui/file/de35bff8f191f23051ccc13c70432627b034b6761707a6555fe1374df08ddcb6) |

Analysezeiten laut abgeschlossenen Berichten: Installer 24.10.2026 – 19:06:33,
EXE 24.10.2026 – 19:06:58 (Europe/Berlin). Nicht jede Engine hat ein
verwertbares Ergebnis geliefert. Diese Berichte ersetzen die Links des früheren
Builds mit derselben Versionsnummer.

Installer: Trapmine `Suspicious.low.ml.score` und Zillya
`Trojan.Blank.Script.2228`; 67 Engines ohne Erkennung.
ClamAV und TEHTRIS: Zeitüberschreitung.
Avast-Mobile, BitDefenderFalx, Symantec Mobile Insight und Trustlook:
Dateityp nicht unterstützt. Diese Ergebnisse zählen nicht als „sauber“.

EXE: 65 Engines ohne Erkennung. Gemeldete Funde:

| Engine | Bezeichnung |
| --- | --- |
| Arctic Wolf | `Unsafe` |
| Microsoft | `Trojan:Win32/Wacatac.C!ml` |
| SecureAge | `Malicious` |
| Skyhigh (SWG) | `BehavesLike.Win64.Backdoor.vc` |
| Zillya | `Trojan.Blank.Script.2228` |

Jiangmin: Prüfungsfehler. Dieselben vier mobilen Engines unterstützen den
Dateityp nicht. VirusTotal sammelt die Bewertungen unabhängiger Hersteller;
die Bewertung eines einzelnen Herstellers kann VirusTotal nicht aufheben.
[Erklärung von VirusTotal](https://docs.virustotal.com/docs/false-positive).

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
  Abgleiche. Lokale Feldexporte sind kein Beleg für eine automatische Übertragung
  dieses Exports an die Webseite.
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
