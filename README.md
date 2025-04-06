# Federico Shin'ichi Archive

## Development Guide

Run a local copy of the github pages site by running `mkdocs serve`

## Deploying

When you run `mkdocs gh-deploy` the current changes will be pushed up to the `gh-pages` branch

---

```bash
git add .
git commit -m "Messaggio descrittivo del commit"
git push
```

### Spiegazione:

- `git add .` → aggiunge **tutti** i file modificati nella staging area (pronti per il commit)
    
- `git commit -m "messaggio"` → crea un **commit** con un messaggio che descrive cosa hai cambiato
    
- `git push` → invia il commit al **repository remoto** (es. su GitHub)
    

---