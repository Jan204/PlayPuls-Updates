# PlayPuls 0.0.0.6 – VirusTotal, SmartScreen und Datenzugriff

Prüfstand: 28.10.2026, Europe/Berlin. Die Berichte gelten ausschließlich für die unten genannten SHA-256-Prüfsummen. Verdachtsmeldungen sind **nicht als Fehlalarme bestätigt**. Ein Scan ist keine Sicherheitsgarantie.

## Geprüfte Dateien

Installer und die enthaltene Programmdatei wurden separat geprüft. Die Programmdatei ist bytegleich mit der EXE im Portable-Paket und der beim Installerbau verwendeten EXE. Bei veränderten Dateien sind neue dateispezifische Prüfungen erforderlich.

[VirusTotal-Prüfbericht für PlayPuls 0.0.0.6 – Installer](https://www.virustotal.com/gui/file/57c2040962a06650008cb8e21a28f18ad6b45d4d364db37a2b5d1c0ec5409663) – 1 von 70 Engines meldet einen Verdacht.

[VirusTotal-Prüfbericht für PlayPuls 0.0.0.6 – Programmdatei](https://www.virustotal.com/gui/file/5d5da299f6836f08d858cd611f33b3a3e5247fb88c6ac95d0028b9657bdf94d6) – 4 von 71 Engines melden einen Verdacht.

[VirusTotal-Prüfbericht für PlayPuls 0.0.0.6 – Portable-Paket](https://www.virustotal.com/gui/file/6ca66a4305d06e6d22da467385da9c47edf640e4bacf83a108f42e4cbf4964cf) – Keine Erkennung bei 67 Engines.

Die Verdachtsmeldungen sind nicht als Fehlalarme bestätigt. [Befunde, Datenzugriffe und Lizenzhinweis](https://github.com/Jan204/PlayPuls-Updates/blob/main/VIRUSTOTAL_0.0.0.6.md).

### Installer

SHA-256: `57c2040962a06650008cb8e21a28f18ad6b45d4d364db37a2b5d1c0ec5409663`

Analysezeit: 28.10.2026 – 14:49:19 (Europe/Berlin).

- Trapmine: `Suspicious.low.ml.score`

Zeitüberschreitung: Skyhigh (SWG).

Dateityp nicht unterstützt: Avast-Mobile, BitDefenderFalx, Symantec Mobile Insight, Trustlook.

### PlayPuls.exe

SHA-256: `5d5da299f6836f08d858cd611f33b3a3e5247fb88c6ac95d0028b9657bdf94d6`

Analysezeit: 28.10.2026 – 14:43:34 (Europe/Berlin).

- Arctic Wolf: `Unsafe`
- Microsoft: `Trojan:Win32/Wacatac.C!ml`
- SecureAge: `Malicious`
- Skyhigh (SWG): `BehavesLike.Win64.Backdoor.vc`

Dateityp nicht unterstützt: Avast-Mobile, BitDefenderFalx, Symantec Mobile Insight, Trustlook.

### Portable-Paket

SHA-256: `6ca66a4305d06e6d22da467385da9c47edf640e4bacf83a108f42e4cbf4964cf`

Analysezeit: 28.10.2026 – 14:51:27 (Europe/Berlin).


Zeitüberschreitung: ClamAV.

Dateityp nicht unterstützt: Arctic Wolf, BitDefenderFalx, Palo Alto Networks, SecureAge, Symantec Mobile Insight, TEHTRIS, Trapmine.

Nicht abgeschlossene oder nicht unterstützte Prüfungen zählen nicht als „sauber“. VirusTotal weist beim mehrteiligen Portable-Archiv über 3 MiB auf Einschränkungen beim Prüfen enthaltener Dateien hin. Sein Archivbericht ersetzt deshalb nicht die separate EXE-Prüfung.

## Einordnung

Die App wird mit PyInstaller gebündelt und der Installer mit NSIS erstellt. Das erklärt den Aufbau der Dateien, beweist aber nicht, dass konkrete Verdachtsmeldungen falsch sind. Der Abgleich der gebündelten Module mit den Quellen und bestandene Funktionstests ersetzen keine unabhängige Sicherheitsprüfung. Auch Bezeichnungen mit „ml“ oder „BehavesLike“ erlauben keine abschließende Entwarnung. Eine Bestätigung der jeweiligen Sicherheitsanbieter, dass die Funde Fehlalarme sind, liegt nicht vor. Die Dateien wurden nicht zur Umgehung von Erkennungen verändert.

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
- **Modupdates:** Die App prüft einen öffentlichen signierten Modkanal auf GitHub. Dafür werden keine Konto- oder Serverzugangsdaten mitgesendet. Heruntergeladene Pakete werden vor der Verwendung auf Signatur, Kompatibilität, Größe und Inhalt geprüft.
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
geschützt“; die Meldung beweist weder Schadcode noch Unbedenklichkeit und ersetzt keine VirusTotal-Prüfung.
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
