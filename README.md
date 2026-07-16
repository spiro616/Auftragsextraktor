# SAP PDF Extraktor – Südostbayernbahn

Ein rein clientseitiges Tool (HTML/JS, keine Installation nötig), das zwei bisherige Extraktoren kombiniert:

1. **Auftragsnummern aus PDF** – findet 9-stellige IH-/Inspektionsauftrag-Nummern (Text-Layer + OCR-Fallback, überspringt Befundlisten & Blatt 2+).
2. **TP/Fehler-Liste (SPOOL) → Excel** – liest SPOOL-PDF-Exporte und erzeugt eine `.xlsx` mit Spalte A (TP) / Spalte B (Fehler).

Über die zwei Checkboxen oben wählst du aus, welche der beiden Suchen auf die hochgeladenen PDFs angewendet werden soll (auch beide gleichzeitig möglich).

Alles läuft im Browser – es wird nichts hochgeladen oder gespeichert.

## Auf GitHub Pages veröffentlichen

1. Erstelle ein neues GitHub-Repository (z. B. `sap-pdf-extraktor`).
2. Lade diese zwei Dateien in das Repo hoch (per Weboberfläche: "Add file" → "Upload files"):
   - `index.html`
   - `logo.png`
3. Gehe zu **Settings → Pages**.
4. Unter "Build and deployment" wähle **Source: Deploy from a branch**, Branch: `main`, Ordner `/ (root)`.
5. Speichern. Nach ca. 1 Minute ist die Seite erreichbar unter:
   `https://<dein-username>.github.io/<repo-name>/`

Fertig – kein Server, kein Backend nötig, alles läuft lokal im Browser des Nutzers.
