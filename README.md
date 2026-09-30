# Dori English

A Bulgarian ↔ English vocabulary flashcard web app, built as a single
self-contained HTML page (`index.html`) with an editable `.xlsx` word
database (`rechnik.xlsx`).

## How it works

- Open `index.html` in a browser (or serve the repo, e.g. via GitHub Pages).
- The app ships with an embedded copy of the word list, and on every load
  it also checks `rechnik.xlsx` in this repo and loads the latest version
  automatically — no manual upload needed, as long as the browser is online.
- To add or edit words: open `rechnik.xlsx`, edit the **думи** sheet (or any
  other sheet), and push the change to this repo's `main` branch. The app
  will pick it up automatically the next time it's opened.
- **Any extra sheet** in `rechnik.xlsx` (besides `думи` and `Инструкции`)
  automatically becomes its own practice category with a matching button in
  the app — for example `AI`, `HPE`, `HPE Objectives`. Add a new sheet with
  the same columns (`Word`, `Meaning`, ...) to create a new category; no code
  changes are needed.
- You can also download/upload the `.xlsx` file directly from within the app
  ("Свали речника" / "Качи речник") to work on it locally before pushing.

See the `Инструкции` sheet inside `rechnik.xlsx` for the full column format.
