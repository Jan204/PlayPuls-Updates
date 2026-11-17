# PlayPuls 1.0.0.2 – VirusTotal-Prüfung des Testsetups

Die folgenden Berichte gehören zum Testsetup vom 17.11.2026 mit Mod 0.0.0.9, Revision 5, und dem Fix für Windows-Fehler 5. Der Build stammt von Commit `49334f83f7dbaae0d1df324670729d5335eceae6` auf dem Vorbereitungsbranch. Beide Analysen sind abgeschlossen. Die auf VirusTotal angezeigten SHA-256 stimmen mit den lokal berechneten Prüfsummen überein.

| Datei | Analyse am 17.11.2026 (MEZ) | SHA-256 | Meldungen bei Engines mit Ergebnis | Bericht |
| --- | --- | --- | --- | --- |
| `PlayPuls-1.0.0.2-Setup.exe` | 17:39:52 | `34a3f20ee80cae35ecc2db10637b077e117cee9b5bf041113e2baed568646659` | 1 von 67 | [Installer](https://www.virustotal.com/gui/file/34a3f20ee80cae35ecc2db10637b077e117cee9b5bf041113e2baed568646659) |
| `PlayPuls.exe` | 17:40:07 | `763ce53cab26e8d72ef7bbef040f416eea662f871b1228eba48502ca41bd98ac` | 3 von 71 | [Programmdatei](https://www.virustotal.com/gui/file/763ce53cab26e8d72ef7bbef040f416eea662f871b1228eba48502ca41bd98ac) |

- **Installer.** Trapmine meldet `Suspicious.low.ml.score`. ClamAV, Skyhigh (SWG), Trellix ENS und TrendMicro beendeten ihre Prüfung mit Zeitüberschreitung.
- **Programmdatei.** Arctic Wolf meldet `Unsafe`, SecureAge `Malicious` und Skyhigh (SWG) `BehavesLike.Win64.Backdoor.wc`. Der Bericht listet keine Zeitüberschreitung.
- **Dateityp.** BitDefenderFalx, Symantec Mobile Insight und Trustlook konnten den Dateityp beider Dateien nicht prüfen.

Die vier Fundnamen und Anbieter stimmen mit Version 1.0.0.1 überein. Jan hatte die Meldungen bei 1.0.0.1 als bereits untersuchte Fehlalarme eingeordnet. [Früherer Prüfbericht](https://github.com/Jan204/PlayPuls-Updates/blob/main/VIRUSTOTAL_1.0.0.1.md)
