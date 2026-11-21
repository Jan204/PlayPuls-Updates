# VirusTotal-Prüfung für PlayPuls 1.0.0.3

Die Analysen des finalen Windows-Installers und der enthaltenen Programmdatei sind am 21.11.2026 abgeschlossen. Die SHA-256 stimmen mit dem geprüften Release-Kandidaten überein.

| Datei | Analysezeit (MEZ) | SHA-256 | Meldungen bei Engines mit Ergebnis | Bericht |
| --- | --- | --- | --- | --- |
| `PlayPuls-1.0.0.3-Setup.exe` | 14:23:41 | `49d7f0dee893285bcf87b5bbd912560caf377a9f11b676f519da26c1e36b4109` | 1 von 68 | [Installer](https://www.virustotal.com/gui/file/49d7f0dee893285bcf87b5bbd912560caf377a9f11b676f519da26c1e36b4109) |
| `PlayPuls.exe` | 14:24:00 | `e514b75b0614aac30bb2b6699f75167a8e7ce5b886267114a3eab49d73dbd56c` | 2 von 65 | [Programmdatei](https://www.virustotal.com/gui/file/e514b75b0614aac30bb2b6699f75167a8e7ce5b886267114a3eab49d73dbd56c) |

- **Installer.** Trapmine meldet `Suspicious.low.ml.score`. Zeitüberschreitung bei ClamAV, Trellix ENS, TrendMicro.
- **Programmdatei.** Arctic Wolf meldet `Unsafe`, SecureAge meldet `Malicious`. Zeitüberschreitung bei Avast, AVG, Google, MaxSecure, Skyhigh (SWG), Trellix ENS.
- **Dateityp.** BitDefenderFalx, Symantec Mobile Insight und Trustlook konnten die Dateitypen beider Dateien nicht prüfen.

Die drei aktuellen Fundnamen wurden bereits bei 1.0.0.2 gemeldet. Skyhigh (SWG) hatte bei der Programmdatei diesmal eine Zeitüberschreitung. Die wiederkehrenden Bezeichnungen allein belegen keinen Fehlalarm.
