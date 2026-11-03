# Paulimania

Orga-Tool für den Montagskick (11 gegen 11).

## Phase 1 – für den Organisator

- **Spieler:** Erst nur Namen eintragen (mehrere mit Komma), Positionen und Bewertung kommen später über „Bewerten“. Spieler mit Hauptposition und beliebig vielen Nebenpositionen (TW, LV, IV, RV, LAV, RAV, ZDM, LM, ZM, RM, ZOM, LF, MS, ST, RF) und elf Kriterien (je 1–10) anlegen: Kondition, Tempo, Ballbehandlung, Passspiel, Spielverständnis, Zweikampfbereitschaft, Härte, Abschluss, Erfahrung & Sicherheit, Torwartspiel, Charakter. Daraus berechnet die App die Gesamtstärke. Charakter zählt nicht zur Stärke, wird aber gleichmäßig auf die Teams verteilt. Bewertungen lassen sich jederzeit ändern, die Entwicklung wird mitgespeichert. Spieler, die eine Weile fehlen (z. B. verletzt), lassen sich pausieren.
- **Spieltag:** Ankreuzen, wer dabei ist. „Alle von letzter Woche“ übernimmt die Spieler mit Vorrecht.
- **Faire Teams:** Der Generator verteilt Gesamtstärke, jedes einzelne Kriterium und die Positionen gleichmäßig, mit je einem Torwart pro Team. Er mischt außerdem anders als letzte Woche. „Neu mischen“ liefert eine andere, ebenso faire Aufteilung. Spieler lassen sich von Hand tauschen.
- **WhatsApp-Text:** Die Teams werden als Text kopiert, ohne Stärkewerte.
- **Statistik:** Gespeicherte Spieltage mit Ergebnis. Pro Spieler steht dort, wie oft er gespielt hat, wann zuletzt, und wie seine Bilanz aussieht (Siege-Unentschieden-Niederlagen). Außerdem ein Status: Vorrecht, Ersatz oder länger weg.

- **Mehrere Bewerter:** Jeder aus dem Orga-Team bewertet die Spieler selbst. Für die Teams zählt der Durchschnitt pro Kriterium. Oben bei „Ich bin“ wählt jedes Orga-Mitglied einmal seinen Namen (Paul, Louis, Kevin, Jonas), das Gerät merkt ihn sich. Sichtbar sind nur der Durchschnitt und wer schon bewertet hat, nicht die einzelnen Werte. Name und Positionen sind gemeinsam.

## Benutzen

`index.html` im Browser öffnen. Lokal liegen die Daten im Browser (localStorage). Über „Sicherung kopieren / einfügen“ im Kader lassen sie sich auf ein anderes Gerät übertragen.
Als claude.ai-Artifact veröffentlicht, nutzt die App einen gemeinsamen Speicher. Dann sind die Daten auf allen Geräten gleich. Orga-Mitglieder werden über das Teilen-Menü als Editor eingeladen, Die Bewertungen liegen pro Name in `ratings/<Name>`.

## Nächste Phasen (Ideen)

2. Link für alle Spieler zum Zu- und Absagen, mit Vorrecht-Frist und Warteliste.
3. Stärkewerte passen sich anhand der Ergebnisse automatisch an.
