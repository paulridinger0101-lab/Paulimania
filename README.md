# Schneppenhausen

(Repo: Paulimania)

Orga-Tool für den Montagskick (11 gegen 11).

## Phase 1 – für den Organisator

- **Spieler:** Erst nur Namen eintragen (mehrere mit Komma), Positionen und Bewertung kommen später über „Bewerten“. Spieler mit Hauptposition und beliebig vielen Nebenpositionen (TW, LV, IV, RV, ZM, ZOM, LF, ST, RF) und elf Kriterien (je 1–10) anlegen: Kondition, Tempo, Ballbehandlung, Passspiel, Spielverständnis, Zweikampfbereitschaft, Härte, Abschluss, Erfahrung & Sicherheit, Torwartspiel, Charakter. Torhüter (Hauptposition TW) haben eigene Kriterien: Reflexe, Stellungsspiel, Fangsicherheit, Eins gegen Eins, Strafraumbeherrschung, Sprungkraft & Beweglichkeit, Mut, Konzentration & Nerven, Abwurf & Abschlag, Fußspiel, Kommunikation, Charakter. Daraus berechnet die App die Gesamtstärke. Die Spielerliste ist nach Nachnamen sortiert. Charakter zählt nicht zur Stärke, wird aber gleichmäßig auf die Teams verteilt. Bewertungen lassen sich jederzeit ändern, die Entwicklung wird mitgespeichert. Spieler, die eine Weile fehlen (z. B. verletzt), lassen sich pausieren.
- **Spieltag:** Ankreuzen, wer dabei ist. „Alle von letzter Woche“ übernimmt die Spieler mit Vorrecht.
- **Faire Teams:** Der Generator verteilt Gesamtstärke, jedes einzelne Kriterium und die Positionen gleichmäßig, mit je einem Torwart pro Team. Er mischt außerdem anders als letzte Woche. „Neu mischen“ liefert eine andere, ebenso faire Aufteilung. Spieler lassen sich von Hand tauschen.
- **WhatsApp-Text:** Die Teams werden als Text kopiert, ohne Stärkewerte.
- **Statistik:** Gespeicherte Spieltage mit Ergebnis. Pro Spieler steht dort, wie oft er gespielt hat, wann zuletzt, und wie seine Bilanz aussieht (Siege-Unentschieden-Niederlagen). Außerdem ein Status: Vorrecht, Ersatz oder länger weg.

- **Mehrere Bewerter:** Jeder aus dem Orga-Team bewertet die Spieler selbst. Für die Teams zählt der Durchschnitt pro Kriterium. Oben bei „Ich bin“ wählt jedes Orga-Mitglied einmal seinen Namen (Paul, Louis, Kevin, Jonas). Im geteilten Artifact wird der Name fest an das Claude-Konto gebunden: Jeder schreibt nur in sein eigenes Bewertungsdokument `ratings/<Konto-ID>`, das erzwingt der Speicher. Der Besitzer kann einen falsch gewählten Namen unter „Orga-Team verwalten“ wieder freigeben. Niemand bewertet sich selbst: Ein Orga-Mitglied (im Spielerformular unter „Orga-Mitglied“ verknüpft, sonst automatisch per Vorname) wird von den anderen drei bewertet. Zahlen eines Spielers erscheinen erst, wenn alle, die ihn bewerten sollen, bewertet haben; bis dahin steht nur, wer schon bewertet hat und wer fehlt. Einzelwerte anderer sind nie sichtbar. Positionen: Jedes Orga-Mitglied gibt seine eigene Einschätzung ab (nicht für sich selbst). Hauptposition = die meisten Stimmen als Hauptposition (Gleichstand: die in der Positionsliste vordere), Nebenposition = von mindestens zwei Orga-Mitgliedern als Nebenposition gewählt. Name und Aktiv-Status sind gemeinsam.

## Benutzen

`index.html` im Browser öffnen. Lokal liegen die Daten im Browser (localStorage). Über „Sicherung kopieren / einfügen“ im Kader lassen sie sich auf ein anderes Gerät übertragen.
Als claude.ai-Artifact veröffentlicht, nutzt die App einen gemeinsamen Speicher. Dann sind die Daten auf allen Geräten gleich. Orga-Mitglieder werden über das Teilen-Menü als Editor eingeladen, 

## Soccerhalle (Reiter „Halle“)

Für die Hallenturniere im Winter: 2, 3 oder 4 Teams à 5 Spieler (Rot, Blau, Gelb, Grün), ohne Torwart, je Team 3 Defensive und 2 Offensive. Defensiv zählen TW, LV, IV, RV, ZM, offensiv ZOM, LF, RF, ST (Hauptposition). Bei genau 10 oder 15 Abgehakten wird die Teamzahl automatisch angepasst. Tauschen durch Antippen, WhatsApp-Text und Bild mit allen Teams. Eigene Auswahl in `meta/hall`, unabhängig von Groß- und Kleinfeld.

## Nächste Phasen (Ideen)

2. Link für alle Spieler zum Zu- und Absagen, mit Vorrecht-Frist und Warteliste.
3. Stärkewerte passen sich anhand der Ergebnisse automatisch an.

---

# Unser Einkauf (`einkauf/`)

Gemeinsame Einkaufsliste mit einer Liste pro Markt (Rewe, Aldi, Lidl, Kaufland, DM, Egal wo). Läuft über GitHub Pages ohne Anmeldung, die Daten liegen in Firebase Firestore und gleichen sich live zwischen allen Handys ab, auch offline im Laden.

- Adresse: https://paulridinger0101-lab.github.io/Paulimania/einkauf/
- Wer den Link mit dem Haushalts-Code (`#…`) hat, kann mitschreiben.
- Firebase-Zugangsdaten stehen oben in `einkauf/index.html` (`FIREBASE_CONFIG`), die Sicherheitsregeln in `einkauf/firestore.rules`.
- Ohne `FIREBASE_CONFIG` speichert die App nur im Browser des jeweiligen Geräts.
