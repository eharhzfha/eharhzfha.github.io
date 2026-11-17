# eharhzfha.github.io

Landing page personale (biglietto da visita) pubblicata con **GitHub Pages**.

## Struttura

```
eharhzfha.github.io/
├── index.html          # contenuto della pagina
├── assets/css/style.css # stile (tema chiaro + scuro automatico)
└── README.md
```

## Cosa modificare

Apri `index.html` e sostituisci i punti marcati con `TODO`:

| Elemento | Dove |
| --- | --- |
| Nome e titolo `<title>` | `<head>` |
| Nome grande (`<h1>`) e ruolo (`.role`) | corpo |
| Biografia (`.bio`) | corpo |
| Link LinkedIn | `href` del secondo `.link` |
| Email | `href="mailto:..."` e `<small>` del terzo `.link` |

Il pulsante "Disponibile per nuovi progetti" si rimuove cancellando il blocco
`<p class="status">…</p>`.

## Pubblicazione su GitHub Pages

Il nome della repository deve essere **esattamente** `<username>.github.io`,
cioè `eharhzfha.github.io`, perché GitHub serva il sito dalla radice del dominio.

```powershell
cd "C:\Users\MOHAMMED DAMINE\eharhzfha.github.io"
git init -b main
git add .
git commit -m "Add personal landing page"
git remote add origin https://github.com/eharhzfha/eharhzfha.github.io.git
git push -u origin main
```

Poi su GitHub: **Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)` → Save**.

Dopo 1–2 minuti il sito sarà online su:

```
https://eharhzfha.github.io
```

## Anteprima locale

Apri `index.html` nel browser, oppure avvia un server statico:

```powershell
python -m http.server 8000
# poi visita http://localhost:8000
```

## Note

- Nessuna build, nessuna dipendenza: solo HTML e CSS.
- Tema scuro automatico via `prefers-color-scheme`.
- Font: Instrument Serif + Inter (Google Fonts), con fallback di sistema.
