# VirusTotal-Prüfung für PlayPuls 1.0.0.3

Beide Analysen für den korrigierten Paketstand vom 21.11.2026 sind abgeschlossen. Die SHA-256 stimmen mit dem Windows-Setup und der darin enthaltenen Programmdatei überein.

| Datei | Analysezeit (MEZ) | SHA-256 | Meldungen bei Engines mit Ergebnis | Bericht |
| --- | --- | --- | --- | --- |
| `PlayPuls-1.0.0.3-Setup.exe` | 15:00:39 | `e5a3aa70f17d25690b6a8b118f2fe7844d313e9ec7bfbbc961349640365fe42e` | 1 von 68 | [Installer](https://www.virustotal.com/gui/file/e5a3aa70f17d25690b6a8b118f2fe7844d313e9ec7bfbbc961349640365fe42e) |
| `PlayPuls.exe` | 15:00:50 | `a421af9b4f113e4504a243a62d486012abd9733387566927a620263b037c4767` | 2 von 70 | [Programmdatei](https://www.virustotal.com/gui/file/a421af9b4f113e4504a243a62d486012abd9733387566927a620263b037c4767) |

- **Installer.** Trapmine meldet `Suspicious.low.ml.score`. ClamAV, TrendMicro und Zillya meldeten eine Zeitüberschreitung.
- **Programmdatei.** Arctic Wolf meldet `Unsafe`, SecureAge meldet `Malicious`. Skyhigh (SWG) meldete eine Zeitüberschreitung.
- **Dateityp.** BitDefenderFalx, Symantec Mobile Insight und Trustlook konnten den Dateityp bei beiden Dateien nicht prüfen.

VirusTotal meldet dieselben drei Fundnamen wie beim ersten Paketstand von 1.0.0.3. Die Übereinstimmung der Bezeichnungen allein belegt keinen Fehlalarm. [Prüfung des ersten Paketstands](https://github.com/Jan204/PlayPuls-Updates/blob/148881ea42812b4f4c074b1a68ab9d97238dacf9/VIRUSTOTAL_1.0.0.3.md)
