# 📝 Blog su GitHub Pages

Blog statico con Jekyll, hostato gratuitamente su GitHub Pages.

---

## 🚀 Setup iniziale (una volta sola)

### 1. Crea il repository su GitHub

1. Vai su [github.com](https://github.com) e accedi
2. Clicca **New repository**
3. Scegli un nome (es. `blog`, o `username.github.io` per URL più corta)
4. Metti **Public** ✅
5. **Non** aggiungere README (li carichi tu)
6. Clicca **Create repository**

### 2. Carica i file

```bash
# Clona il repo vuoto
git clone https://github.com/TUO-USERNAME/NOME-REPO.git
cd NOME-REPO

# Copia tutti i file di questo progetto nella cartella
# poi esegui:
git add .
git commit -m "Primo commit: setup blog"
git push origin main
```

### 3. Abilita GitHub Pages

1. Vai su **Settings** del repository
2. Sezione **Pages** (nella barra laterale sinistra)
3. Source: **Deploy from a branch**
4. Branch: `main` → cartella `/` (root)
5. Clicca **Save**

Il sito sarà live in 1-2 minuti su:
`https://TUO-USERNAME.github.io/NOME-REPO`

### 4. Modifica _config.yml

Apri `_config.yml` e cambia:
```yaml
title: "Nome del Tuo Blog"
description: "La tua descrizione"
url: "https://TUO-USERNAME.github.io"
baseurl: "/NOME-REPO"   # vuoto "" se il repo si chiama username.github.io
```

---

## ✍️ Come pubblicare un articolo

### Formato del nome file

Crea un file `.md` nella cartella `_posts/` con questo formato:

```
ANNO-MESE-GIORNO-titolo-separato-da-trattini.md
```

Esempi:
- `2024-03-15-la-mia-vacanza.md`
- `2024-04-01-ricetta-della-pasta.md`

### Intestazione obbligatoria (front matter)

Ogni file DEVE iniziare con questo blocco:

```yaml
---
layout: post
title: "Il Titolo del Mio Articolo"
date: 2024-03-15
author: Il Tuo Nome
tags: [tag1, tag2]
---

Qui inizia il testo dell'articolo...
```

| Campo | Obbligatorio | Descrizione |
|-------|:---:|-------------|
| `layout` | ✅ | Sempre `post` |
| `title` | ✅ | Titolo mostrato sul sito |
| `date` | ✅ | Data nel formato YYYY-MM-DD |
| `author` | ❌ | Nome dell'autore |
| `tags` | ❌ | Lista di tag tra parentesi quadre |

### Sintassi Markdown supportata

```markdown
## Titolo sezione
### Sottotitolo

**grassetto**, *corsivo*, `codice inline`

- Elemento lista
- Altro elemento

1. Lista numerata
2. Secondo punto

[Testo link](https://example.com)

![Descrizione immagine](/assets/images/nome-file.jpg)

> Testo in evidenza / citazione

```codice multiriga```
```

### Aggiungere immagini

1. Carica l'immagine nella cartella `assets/images/`
2. Nel testo dell'articolo scrivi:
   ```markdown
   ![Descrizione](/assets/images/nome-file.jpg)
   ```

---

## 📂 Struttura del progetto

```
blog/
├── _config.yml          ← Configurazione sito
├── _layouts/
│   ├── default.html     ← Layout base (header/footer)
│   ├── home.html        ← Lista articoli
│   └── post.html        ← Pagina singolo articolo
├── _posts/              ← ⭐ QUI vanno gli articoli .md
│   ├── 2024-01-15-benvenuto.md
│   └── 2024-02-08-altro-articolo.md
├── assets/
│   ├── css/main.scss    ← Stili del sito
│   └── images/          ← ⭐ QUI vanno le immagini
├── index.md             ← Home page
├── chi-siamo.md         ← Pagina "Chi siamo"
└── Gemfile              ← Dipendenze Jekyll
```

---

## 🔄 Workflow per il tuo amico

Il modo più semplice per pubblicare senza usare Git:

1. Vai su **github.com** → il repository del blog
2. Entra nella cartella `_posts/`
3. Clicca **Add file → Create new file**
4. Scrivi il nome: `2024-03-20-titolo-articolo.md`
5. Incolla il contenuto con il front matter
6. Clicca **Commit changes**
7. In 1-2 minuti l'articolo è live! 🎉

Per le immagini, stessa cosa nella cartella `assets/images/`.

---

## 🛠 Test in locale (opzionale)

```bash
gem install bundler
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```
