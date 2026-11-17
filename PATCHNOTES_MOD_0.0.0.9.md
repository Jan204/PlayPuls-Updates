# PlayPuls-Mod 0.0.0.9

- **Spielstand-Sync.** Die Mod erkennt beim Selbsthosten denselben Spielstand auch nach normalem Speichern und erneutem Laden. PlayPuls Tool 1.0.0.2 merkt sich dadurch „Ja“ oder „Nein“ für den Spielstand und die Serverzuordnung. Bei einem neuen oder erkannten importierten Spielstand fragt die App erneut.
- **Speichern.** Die Mod verwendet die XML-Funktionen von LS25 für die Spielstandkennung. Das behebt die `io.open`-Warnung und erhält die gespeicherte Sync-Freigabe.
- **HUD.** Bei pausierter Spielstand-Synchronisierung zeigt die Mod „Spielstand-Sync pausiert“ und blendet die Serveraufgaben aus.
