# Songbuch – Offline-App fürs iPad

## Einmalig: App ins Netz stellen (GitHub Pages)
1. Auf github.com anmelden (oder kostenloses Konto anlegen).
2. Oben rechts „+“ → „New repository“. Name: `songbuch`, Sichtbarkeit: **Public** → „Create repository“.
3. Auf der leeren Seite auf „uploading an existing file“ klicken.
4. Alle Dateien aus diesem Ordner ins Browserfenster ziehen → unten „Commit changes“. (Es gibt keine Unterordner mehr.)
5. Im Repository: „Settings“ → links „Pages“ → bei „Branch“ `main` und `/ (root)` wählen → „Save“.
6. Nach 1–2 Minuten steht oben die Adresse, z. B. `https://DEINNAME.github.io/songbuch/`.

Deine PDFs und Notizen werden dabei NICHT hochgeladen. Online steht nur die leere App.

## Auf dem iPad installieren
1. Die Adresse in **Safari** öffnen.
2. Teilen-Symbol → „Zum Home-Bildschirm“ → „Hinzufügen“.
3. Ab jetzt nur noch über das Symbol öffnen. Einmal mit Internet öffnen, danach läuft sie offline.

Wichtig: Die App auf dem Home-Bildschirm hat ihren eigenen Speicher, getrennt vom Safari-Tab.
PDFs daher immer in der Home-Bildschirm-App hinzufügen.

## Bedienung kurz
- **Datei**: PDFs oder Textdateien (.txt, .cho, .chordpro) hinzufügen – oder einfach auf die App ziehen.
- **Songs / Sets**: oben in der Seitenleiste umschalten. Ein Song kann in mehreren Sets stehen und bleibt in der Hauptliste.
- **↕ A–Z / Zuletzt**: Sortierung der Hauptliste umschalten.
- **♭ Tonart ♯** in der Kopfleiste: transponiert Text-Songs in Halbtonschritten; die Einstellung bleibt pro Song gespeichert. Auf die Tonart tippen = zurück zum Original.
- **Set**-Knopf in der Kopfleiste: aktuellen Song in Sets aufnehmen oder entfernen.
- Wird ein Song aus einem Set geöffnet, zeigt eine Leiste Set-Name, Position, deine Notiz für diesen Auftritt und ‹ › zum Blättern.

## Sichern
- „Sichern“ erzeugt eine Datei `Songbuch-Sicherung_DATUM.songbuch` mit allen Songs, PDFs und Notizen.
  Im Teilen-Menü „In Dateien sichern“ → iCloud Drive wählen.
- „Einspielen“ holt eine Sicherung zurück (auch die alte `.json`-Exportdatei).
- Wird das Symbol vom Home-Bildschirm gelöscht, sind die Daten auf dem iPad weg – dann hilft nur die Sicherung.

## Neue Version einspielen
Geänderte Dateien in GitHub erneut hochladen. Die App lädt die neue Version beim nächsten Öffnen mit Internet;
danach einmal schließen und wieder öffnen.

## Update auf Version 4 (Fehler „pdfjs“ / „fake worker“)
Die PDF-Anzeige steckt komplett in `index.html` und lädt keine Zusatzdateien mehr; der Ordner `lib` wird nicht gebraucht.
Im GitHub-Repository `index.html` und `sw.js` durch die neuen Dateien ersetzen (Add file → Upload files → Commit).
Danach die App auf dem iPad einmal mit Internet öffnen, schließen und wieder öffnen.
