# Paulimania

Orga-Tool für den Montagskick (11 gegen 11).

## Phase 1 – für den Organisator

- **Kader:** Spieler mit Position (Torwart, Abwehr, Mittelfeld, Sturm) und Stärke 1–10 anlegen. Spieler, die eine Weile fehlen (z. B. verletzt), lassen sich pausieren.
- **Spieltag:** Ankreuzen, wer dabei ist. „Alle von letzter Woche“ übernimmt die Spieler mit Vorrecht.
- **Faire Teams:** Der Generator verteilt Stärke und Positionen gleichmäßig, mit je einem Torwart pro Team. Er mischt außerdem anders als letzte Woche. „Neu mischen“ liefert eine andere, ebenso faire Aufteilung. Spieler lassen sich von Hand tauschen.
- **WhatsApp-Text:** Die Teams werden als Text kopiert, ohne Stärkewerte.
- **Verlauf und Übersicht:** Gespeicherte Spieltage mit Ergebnis. Im Kader steht pro Spieler, wie oft er gespielt hat, wann zuletzt, und wie seine Bilanz aussieht (Siege-Unentschieden-Niederlagen). Außerdem ein Status: Vorrecht, Ersatz oder länger weg.

## Benutzen

`index.html` im Browser öffnen. Lokal liegen die Daten im Browser (localStorage). Über „Sicherung kopieren / einfügen“ im Kader lassen sie sich auf ein anderes Gerät übertragen.
Als claude.ai-Artifact veröffentlicht, nutzt die App einen gemeinsamen Speicher. Dann sind die Daten auf allen Geräten gleich.

## Nächste Phasen (Ideen)

2. Link für alle Spieler zum Zu- und Absagen, mit Vorrecht-Frist und Warteliste.
3. Stärkewerte passen sich anhand der Ergebnisse automatisch an.
