# PlayPuls 1.0.0 – VirusTotal-Prüfberichte

Dieser Prüfbericht bezieht sich auf die veröffentlichte Windows-Version 1.0.0.

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
