# TamaPoke – Dennis-Build 4.1.1

Web-Installer für das **Waveshare ESP32-S3-Touch-AMOLED-1.75** mit TamaPoke.
Basis: [eperdemes TamaPoke 4.0](https://github.com/eperdeme/TamaPoke) und sein Web-Installer, mit deutscher Oberfläche und Ergänzungen.

**Installer öffnen: https://joop0810.github.io/tamapoke/**

Du brauchst nur Chrome oder Edge am PC oder Mac (Firefox und Safari können kein Web Serial) und ein USB-**Daten**kabel. Du musst nichts herunterladen oder installieren.

## Was diese Version kann

- Deutsche Oberfläche und deutsche Pokémon-Namen (Einstellungen → Sprache)
- Alle neun Regionen. Eine Region erscheint im Spiel, sobald ihre Bilder auf der SD-Karte sind.
- Erfahrung aus Kämpfen, Fangchance im Beutel, rotes NEU bzw. kleiner Pokéball für schon gefangene Arten
- Geld und Laden (Menü → BEUTEL → LADEN): kaufen und verkaufen
- Box: Haken für fertige Reihen und Doppelte, Knopf AUFRAEUMEN
- Lockstoff: Die nächsten 10 wilden Begegnungen sind Arten, die dir noch fehlen.
- Ruhmeshalle (Pokédex → RUHMESHALLE), Vitrinen-Modus (Einstellungen)
- Shinys im Kampf: Funkeln, eigener Kampftext, gelber Stern auf dem Namensschild

## Erstinstallation

1. Board per Datenkabel anschließen und die Installer-Seite öffnen.
2. Schritt 01: **Install firmware** → Board wählen → Install.
3. Schritt 02: **Connect board**, Regionen anhaken, **Install selected**. Pro Region dauert das etwa 5–8 Minuten.

## Firmware aktualisieren (Spielstand bleibt)

1. Schritt 01: **Back up save** → Board wählen. Die Sicherung landet im Download-Ordner.
2. Schritt 01: **Install firmware** → Board wählen → Install.
   **Bei „Erase device“ das Kästchen NICHT anhaken**, nur „Next“. Angehakt wird der ganze Chip gelöscht, also auch Spielstand und Ruhmeshalle.
3. Nach „Connect board“ steht oben rechts die neue Version.

## Sichern

- **Spielstand:** „Back up save“ (Schritt 01) oder „Download save“ (Schritt 03). Enthält Pokémon, Team, Box, Beutel, Geld, Orden und Pokédex.
- **Ruhmeshalle:** eigene Knöpfe in Schritt 03. Sie ist nicht im Spielstand enthalten.
- **Speicher prüfen** (Schritt 03) zeigt, ob das Speichern klappt und wie voll der Speicher ist.

## Gut zu wissen

- Wenn du das USB-Kabel einsteckst, startet das Board neu.
- Board wird nicht gefunden: BOOT halten, RESET tippen, BOOT loslassen. Achte darauf, dass es ein Datenkabel ist.
- Es kann immer nur ein Programm oder Browser-Tab mit dem Board verbunden sein.
- Ein Update über eperdemes offizielle Seite ersetzt diese Version wieder.

## Inhalt

| Datei/Ordner | Zweck |
|---|---|
| `index.html`, `*.js`, `style.css` | eperdemes Installer mit deutschen Ergänzungen |
| `manifest.json`, `firmware/` | Firmware 4.1.1 und welche Teile an welche Adresse kommen |
| `sprites-*.pak`, `paks.json` | Bilder-Pakete aller neun Regionen mit Prüfsummen |
| `quellcode/` | Änderungen gegenüber eperdeme 4.0 (Firmware-Patch, Installer-Diff) |
| `docs/release-notes/` | Versionshinweise |

## Lizenz und Credits

Der Code steht unter MIT-Lizenz (siehe [LICENSE](LICENSE)) und stammt von eperdeme und den Mitwirkenden in [CREDITS.md](CREDITS.md).
Die Pokémon-Grafiken sind Fan-Artwork (PMD SpriteCollab) auf Basis von Nintendo-/Game-Freak-Material. Nur privat und nicht kommerziell verwenden.
Pokémon ist eine Marke von Nintendo, Creatures Inc. und Game Freak. Dies ist ein inoffizielles Fanprojekt.
