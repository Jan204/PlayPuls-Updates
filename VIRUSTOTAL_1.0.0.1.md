# PlayPuls 1.0.0.1 · VirusTotal-Prüfberichte

Der finale Installer und die enthaltene Programmdatei wurden am 15.11.2026 separat geprüft. Beide Analysen sind abgeschlossen. Die Berichte zeigen dieselben SHA-256 wie die lokalen Release-Dateien. Die Programmdatei im Setup und im Portable-Paket hat dieselbe SHA-256.

| Datei | Analyse (MEZ) | Größe in Byte | SHA-256 | Meldungen bei Engines mit Ergebnis | Bericht |
| --- | --- | ---: | --- | ---: | --- |
| `PlayPuls-1.0.0.1-Setup.exe` | 13:11:17 | 19.440.989 | `70ac9dce9ca01153effed7d3de4b643b6a0f78f5e36ed56336ce1a10da735041` | 1 von 70 | [Installer](https://www.virustotal.com/gui/file/70ac9dce9ca01153effed7d3de4b643b6a0f78f5e36ed56336ce1a10da735041) |
| `PlayPuls.exe` | 13:11:15 | 3.665.592 | `8771f47e31d8cba8755aad4ae4557b0c60e6bcc6ae324345b7f289ae2c5c9d0f` | 3 von 71 | [Programmdatei](https://www.virustotal.com/gui/file/8771f47e31d8cba8755aad4ae4557b0c60e6bcc6ae324345b7f289ae2c5c9d0f) |

## Funde

- **Installer.** Trapmine meldet `Suspicious.low.ml.score`.
- **Programmdatei.** Arctic Wolf meldet `Unsafe`, SecureAge `Malicious` und Skyhigh (SWG) `BehavesLike.Win64.Backdoor.wc`.

VirusTotal führt alle vier Meldungen in der Kategorie `malicious`. Bei beiden Dateien stehen insgesamt 75 Anbieter in der Liste. Avast-Mobile, BitDefenderFalx, Symantec Mobile Insight und Trustlook unterstützen den Dateityp bei beiden Dateien nicht. Beim Installer kommt eine Zeitüberschreitung bei ClamAV hinzu.

## Einordnung

Alle vier aktuellen Fundnamen sind im GitHub-Prüfbericht zur veröffentlichten Version 1.0.0 dokumentiert. Der Trapmine-Fund unterscheidet sich nur in der Großschreibung. Skyhigh meldete denselben Fundnamen. Die allgemeinen Einstufungen `Unsafe` und `Malicious` erschienen bei 1.0.0 unter Cylance und APEX. VirusTotal führt APEX als Engine von SecureAge. Arctic Wolf hat das Endpoint-Security-Geschäft von Cylance übernommen. Die Engine-Versionen der einzelnen Prüfungen bleiben offen. [GitHub-Prüfprotokoll 1.0.0](https://github.com/Jan204/PlayPuls-Updates/blob/main/VIRUSTOTAL_1.0.0.md#releasekandidat-mit-html-versionsübersicht) · [VirusTotal zu SecureAge APEX](https://blog.virustotal.com/2019/05/virustotal-secureage.html) · [Arctic Wolf zur Cylance-Übernahme](https://arcticwolf.com/resources/press-releases/arctic-wolf-and-blackberry-announce-closing-of-acquisition-for-cylance/)

Jan hat am 15.11.2026 bestätigt, dass die wiederkehrenden Meldungen bereits untersucht und als Fehlalarme eingeordnet wurden. Die finale Setup-Datei und die enthaltene Programmdatei besitzen keine Windows-Herausgebersignatur.
