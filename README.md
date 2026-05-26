# Extended Methods Website - Workflow

Dieses Repository enthält den Quellcode für die Website: [https://whennig2000.github.io/extended-methods/](https://whennig2000.github.io/extended-methods/)

## Workflow für Änderungen an der Website

Wenn du Inhalte auf der Website ändern oder aktualisieren möchtest, gehst du in folgenden Schritten vor:

### 1. Änderungen lokal vornehmen
Öffne die entsprechenden Dateien (meistens `.qmd`-Dateien wie z.B. `index.qmd`) in deinem Code-Editor (wie VS Code oder RStudio) und bearbeite die Inhalte.

### 2. Website lokal rendern (Vorschau)
Um zu überprüfen, ob die Änderungen richtig übernommen wurden, kannst du dir lokal eine Vorschau ansehen. Öffne dein Terminal im Ordner `website` und führe folgenden Befehl aus:

```bash
quarto render
```
*(Alternativ kannst du auch den "Render"-Button in RStudio verwenden).*

Dies aktualisiert den versteckten bzw. generierten `_site` Ordner mit den neuen HTML-Dateien.

### 3. Änderungen speichern und auf GitHub veröffentlichen (Publish)
Sobald du mit der Vorschau zufrieden bist, musst du die Änderungen auf GitHub übertragen, damit die Live-Website aktualisiert wird. 

Speichere die Änderungen (Commit) und lade sie auf deinen `main` Branch hoch (Push):

```bash
git add .
git commit -m "feat: Manuelle Zählweise aus Überschriften entfernt"
git push
```

**Wie geht es dann online?**
Sobald der Code auf GitHub gepusht wurde, übernimmt GitHub (in Kombination mit GitHub Pages oder Quarto Pub) automatisch den Rest und die Website unter deiner `.github.io` URL wird aktualisiert. *(Falls du die Veröffentlichung manuell via Terminal machst, nutzt du stattdessen `quarto publish gh-pages` oder `quarto publish quarto-pub`).*
