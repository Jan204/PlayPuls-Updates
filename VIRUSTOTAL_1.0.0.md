# PlayPuls 1.0.0 – VirusTotal-Prüfberichte

Stand 11.11.2026. Die Dateien stammen aus dem lokalen Testbuild
`PlayPuls-Windows-Standard-1.0.0` zu Programmstand `5e04fec`.
Beide Dateien wurden separat bei VirusTotal eingereicht. Beide Analysen
sind abgeschlossen.

| Datei | Größe in Byte | SHA-256 | Bericht |
| --- | ---: | --- | --- |
| `PlayPuls-1.0.0-Setup.exe` | 19.418.261 | `798673b42dc4188a8570bc975813377cddc6aaea0fb5d7b8156dba5c09fce6c2` | [Installer](https://www.virustotal.com/gui/file/798673b42dc4188a8570bc975813377cddc6aaea0fb5d7b8156dba5c09fce6c2) |
| `PlayPuls/PlayPuls.exe` | 3.648.184 | `c62b8cc8d7e8b9d2e49e38a436bb500005ae30c0a576345d44a6fa81814b80a8` | [Programmdatei](https://www.virustotal.com/gui/file/c62b8cc8d7e8b9d2e49e38a436bb500005ae30c0a576345d44a6fa81814b80a8) |

Beide Dateien liegen im App-Arbeitsverzeichnis unter
`artifacts/PlayPuls-Windows-Standard-1.0.0/`. Die Programmdatei aus der
isolierten Installation und die aus dem Portable-Paket haben dieselbe
SHA-256 wie die hier aufgeführte `PlayPuls.exe`.

## Ergebnisse

| Datei | Analyse vom 11.11.2026 (MEZ) | Meldungen je Engines mit Ergebnis | Insgesamt aufgeführte Engines |
| --- | --- | --- | --- |
| Installer | 17:48:47 | 1 von 65 | 71 |
| Programmdatei | 17:48:49 | 3 von 68 | 71 |

Die Quote zählt die Engines mit einem Ergebnis. Zeitüberschreitungen
und ein nicht unterstützter Dateityp sind unten separat aufgeführt.
[VirusTotal-Kategorien](https://docs.virustotal.com/reference/analyses-object)

**Installer**

- Trapmine meldete `suspicious.low.ml.score` in der Kategorie `malicious`.
- Zeitüberschreitung bei ClamAV, TrellixENS und Elastic.
- Trustlook, SymantecMobileInsight und BitDefenderFalx unterstützen den Dateityp nicht.

**Programmdatei**

- Skyhigh meldete `BehavesLike.Win64.Backdoor.wc`, APEX `Malicious`
  und Cylance `Unsafe`. Alle drei stehen in der Kategorie `malicious`.
- Trustlook, SymantecMobileInsight und BitDefenderFalx unterstützen den Dateityp nicht.

## Vergleich mit den früheren Befunden

| Dokumentierter Prüfstand | Installer | Programmdatei |
| --- | ---: | ---: |
| [0.0.0.4 vom 24.10.2026](VIRUSTOTAL_0.0.0.4.md) | 2 von 69 | 5 von 70 |
| [0.0.0.6 vom 28.10.2026](VIRUSTOTAL_0.0.0.6.md) | 1 von 70 | 4 von 71 |
| 1.0.0 vom 11.11.2026 | 1 von 65 | 3 von 68 |

- **Installer.** Trapmine meldete in beiden früheren Prüfungen
  `Suspicious.low.ml.score`. Die aktuelle Meldung entspricht diesem Fund
  bis auf die Großschreibung. Bei 0.0.0.4 meldete Zillya zusätzlich
  `Trojan.Blank.Script.2228`. Im aktuellen Bericht führt VirusTotal
  Zillya als `undetected`.
- **Programmdatei.** Skyhigh meldete bei 0.0.0.4 und 0.0.0.6
  `BehavesLike.Win64.Backdoor.vc`. Der aktuelle Fundname endet auf `.wc`.
  Microsoft führte bei beiden älteren Ständen `Trojan:Win32/Wacatac.C!ml`,
  Zillya bei 0.0.0.4 `Trojan.Blank.Script.2228`. Im aktuellen Bericht
  stehen Microsoft und Zillya auf `undetected`.
- **Engine-Namen.** Die älteren Berichte führten SecureAge mit
  `Malicious` und Arctic Wolf mit `Unsafe`. Aktuell erscheinen dieselben
  Labels bei APEX und Cylance. VirusTotal dokumentiert APEX als Engine von
  SecureAge. Arctic Wolf hat Cylance übernommen. Welche Engine-Versionen
  hinter den Bezeichnungen in den einzelnen Berichten stehen, bleibt offen.
  [SecureAge APEX bei VirusTotal](https://blog.virustotal.com/2019/05/virustotal-secureage.html) · [Arctic Wolf zur Cylance-Übernahme](https://arcticwolf.com/resources/press-releases/arctic-wolf-and-blackberry-announce-closing-of-acquisition-for-cylance/)

Für 0.0.0.7 ist in den Notizen die Prüfung als ausstehend vermerkt.
[Notiz zu 0.0.0.7](VIRUSTOTAL_0.0.0.7.md)

## Einordnung und Freigabe

Trapmine meldet einen niedrigen ML-Verdachtswert für den Installer.
Skyhigh meldet einen Backdoor-Verdacht für die Programmdatei. APEX und
Cylance geben allgemeine Einstufungen an. Die vier Befunde sind offen.
Die Freigabe des Testbuilds zur Veröffentlichung steht aus.

Die SHA-256 in beiden abgeschlossenen Berichten stimmt mit den lokalen
Dateien überein. Die Uploadbelege und vollständigen JSON-Berichte liegen
unter `artifacts/pruefnachweis-Windows-Standard-1.0.0/virustotal/`.

## Releasekandidat mit HTML-Versionsübersicht

Die Prüfdateien liegen unter `artifacts/PlayPuls-Releasekandidat-1.0.0/`.
Die Dateien zum Programmstand `91f6683` wurden am 12.11.2026 separat
eingereicht. Beide Analysen sind abgeschlossen. Die SHA-256 in den
Berichten stimmen mit den lokalen Prüfdateien überein.

| Datei | SHA-256 | Bericht |
| --- | --- | --- |
| `PlayPuls-1.0.0-Setup.exe` | `194369e40a09e4c8862382349f607db6b882121a358b5191c6d513d90cd4b1af` | [Installer](https://www.virustotal.com/gui/file/194369e40a09e4c8862382349f607db6b882121a358b5191c6d513d90cd4b1af) |
| `PlayPuls/PlayPuls.exe` | `301f3726d092c43b70e5f800f22b2a307ab89a416fc60c21cdd1357bb29f8825` | [Programmdatei](https://www.virustotal.com/gui/file/301f3726d092c43b70e5f800f22b2a307ab89a416fc60c21cdd1357bb29f8825) |

| Datei | Analyse am 12.11.2026 (MEZ) | Meldungen bei Engines mit Ergebnis | Insgesamt aufgeführte Engines |
| --- | --- | --- | --- |
| Installer | 14:29:30 | 1 von 67 | 71 |
| Programmdatei | 14:29:32 | 3 von 68 | 71 |

**Installer**

- Trapmine meldet `suspicious.low.ml.score` in der Kategorie `malicious`.
- Zeitüberschreitung bei ClamAV.
- Nicht unterstützter Dateityp bei Trustlook, SymantecMobileInsight und
  BitDefenderFalx.
- Der Fundname entspricht dem Windows-Standard-Testbuild. Diesmal haben
  67 statt 65 Engines ein Ergebnis geliefert.

**Programmdatei**

- Skyhigh meldet `BehavesLike.Win64.Backdoor.wc`, Cylance `Unsafe`
  und APEX `Malicious`. Alle drei Meldungen stehen in der Kategorie
  `malicious`.
- Nicht unterstützter Dateityp bei Trustlook, SymantecMobileInsight und
  BitDefenderFalx.
- Die drei Fundnamen entsprechen dem Windows-Standard-Testbuild.
  Die Einstufung als Fehlalarm bleibt offen.

Die vollständigen Berichte und Uploadbelege liegen unter
`artifacts/pruefnachweis-Releasekandidat-1.0.0/virustotal/`.
