# Album Diary – Mobile Album Tracker

Ein persönlicher, mobiler Album-Tracker für Musik-Alben, Queue, Album Cards, Standout Tracks, Mood-Playlists und Top-30-Songs.

Die App ist eine einzelne statische HTML-Datei (`index.html`). Sie funktioniert ohne Login, ohne Server und ohne Datenbank.

Das Design basiert auf einer Pinterest-Collage (siehe Quelle: https://de.pinterest.com/pin/3729612228359468/).

## Was kann die App?

- Alben in einer **Queue** sammeln
- Apple-Music-Albumlinks (alternativ auch Spotify- oder iTunes-Albumlink) einfügen und Albumdaten importieren
- Alben aus der Queue in einzelne **Album Cards** übertragen
- pro Album eigene Tracks, Standout Tracks, Mood, Ratings und Notizen speichern
- Standout Tracks nach Mood in Playlists sammeln
- eine allgemeine **Top 30 Songs** Playlist führen
- Songs schnell in Apple Music oder Spotify öffnen
- Daten lokal im Browser speichern
- Backup kopieren, herunterladen und wieder importieren

## Wichtig: Werden meine Daten mit anderen geteilt?

Nein.

Der veröffentlichte Code enthält nur die Grund-App. Persönliche Daten wie Queue, Ratings, Notes oder Album Cards werden lokal im Browser der jeweiligen Person gespeichert.

Das bedeutet:

- Wenn du die App benutzt, werden deine Einträge nur auf deinem Gerät gespeichert.
- Andere Nutzerinnen und Nutzer sehen deine Einträge nicht.
- Wenn jemand anderes die App benutzt, verändert das meine Daten nicht.
- Wenn jemand den Code forkt oder kopiert, verändert das nicht mein Repository und nicht meine Website-Adresse.

Bitte lade keine persönlichen Backup-Dateien in ein öffentliches Repository hoch.

## Option 1: Die App direkt nutzen

Wenn du nur die App nutzen möchtest, öffne den veröffentlichten Link der App im Browser.

Auf dem iPhone:

1. Öffne den App-Link in **Safari**.
2. Tippe unten auf das Teilen-Symbol.
3. Wähle **Zum Home-Bildschirm**.
4. Gib der App einen Namen, zum Beispiel `Album Diary`.
5. Tippe auf **Hinzufügen**.

Danach liegt die App wie eine normale App auf deinem Home-Bildschirm.

## Option 2: Eigene Kopie erstellen

Wenn du den Code selbst anpassen oder unter deiner eigenen Adresse veröffentlichen möchtest, erstelle bitte eine eigene Kopie.

### Variante A: Repository forken

1. Klicke oben rechts auf **Fork**.
2. GitHub erstellt eine Kopie in deinem eigenen Account.
3. Arbeite nur in deiner Kopie.
4. Ändere nicht das Original-Repository.
5. Sende keinen Pull Request, wenn du nur deine private Version verändern möchtest.

### Variante B: Datei herunterladen und eigenes Repository erstellen

1. Lade die Datei `index.html` herunter.
2. Erstelle ein neues GitHub-Repository.
3. Lade `index.html` in dein neues Repository hoch.
4. Veröffentliche es mit GitHub Pages.

## Veröffentlichung mit GitHub Pages

Damit die App online erreichbar ist, kann sie mit GitHub Pages veröffentlicht werden.

1. Stelle sicher, dass die Hauptdatei exakt `index.html` heißt.
2. Gehe in deinem Repository zu **Settings**.
3. Öffne links **Pages**.
4. Wähle bei **Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
5. Speichern.
6. Warte kurz, bis GitHub Pages die Website veröffentlicht.
7. Öffne die angezeigte GitHub-Pages-Adresse.

Die Adresse sieht ungefähr so aus:

```text
https://DEINNAME.github.io/REPOSITORY-NAME/
```

## iPhone-Nutzung als Home-Bildschirm-App

Nachdem GitHub Pages aktiv ist:

1. Öffne die GitHub-Pages-Adresse auf dem iPhone in **Safari**.
2. Tippe auf das Teilen-Symbol.
3. Wähle **Zum Home-Bildschirm**.
4. Tippe auf **Hinzufügen**.

Nutze danach immer dieses Home-Screen-Icon. Dann bleibt die Nutzung am stabilsten.

## Wie werden Daten gespeichert?

Die App speichert Daten lokal im Browser über `localStorage`.

Das heißt:

- Daten werden nicht automatisch auf GitHub gespeichert.
- Daten werden nicht mit anderen Nutzerinnen und Nutzern geteilt.
- Daten bleiben normalerweise erhalten, wenn du die App später wieder über dieselbe Website-Adresse öffnest.
- Wenn du Safari-Website-Daten löschst, können deine Einträge verloren gehen.
- Wenn sich die Website-Adresse ändert, erkennt der Browser das als neue App und zeigt die alten lokalen Daten dort nicht automatisch an.

## Backup erstellen

Im Dashboard gibt es einen Backup-Bereich.

Empfohlen:

- regelmäßig **Backup kopieren** nutzen und den Text in Notizen speichern
- oder **Backup-Datei** herunterladen
- Backup niemals öffentlich ins Repository hochladen

## Backup wiederherstellen

1. Öffne die App.
2. Gehe zum Dashboard.
3. Wähle **Backup einfügen / importieren**.
4. Füge den vollständigen Backup-Text ein.
5. Bestätige den Import.

Achtung: Beim Import werden die aktuellen lokalen Daten durch das Backup ersetzt.

## Für Entwicklerinnen und Entwickler

Die App besteht aus einer einzigen Datei:

```text
index.html
```

Enthalten sind:

- HTML-Struktur
- CSS-Design
- JavaScript-Logik
- lokales Speichern über `localStorage`

Es wird kein Backend benötigt.

## Was du nicht tun solltest

- keine persönlichen Daten direkt in `index.html` speichern
- keine Backup-Dateien ins öffentliche Repository hochladen
- nicht am Original-Repository arbeiten, wenn du eine eigene Version möchtest
- nicht die Website-Adresse ändern, wenn du deine lokalen Daten behalten möchtest, ohne vorher ein Backup zu machen

## Eigene Anpassungen

Du kannst in deiner eigenen Kopie zum Beispiel ändern:

- Farben
- Schriftgrößen
- Texte
- Anzahl der Queue-Slots
- Design-Details
- Felder und Kategorien

Bitte mache solche Änderungen in deinem eigenen Fork oder eigenen Repository, nicht im Original.

## Lizenz / Nutzung

Du darfst den Grundcode für deine eigene Album-Sammlung nutzen und anpassen. Wenn du die App öffentlich teilst, achte darauf, keine persönlichen Daten oder Backups mitzuveröffentlichen.
