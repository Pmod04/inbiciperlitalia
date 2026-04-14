---
layout: post
title: "Primo post - TEST"
date: 2026-04-14
author: Modena Pietro
tags: [test]
---

Questo è il **primo articolo** del blog. Questo file di esempio mostra come scrivere un post.

## Come fare

Crea un file `.md` nella cartella `_posts/` con il formato del nome:

```
ANNO-MESE-GIORNO-titolo-articolo.md
```

Ad esempio: `2024-03-20-il-mio-nuovo-articolo.md`

## Intestazione necessaria

Ogni file deve iniziare con questo blocco (chiamato *front matter*):

```yaml
---
layout: post
title: "Il titolo del mio articolo"
date: 2024-03-20
author: Il Tuo Nome
tags: [tag1, tag2]
---
```

## Formattazione supportata

Puoi usare tutta la sintassi Markdown:

- **grassetto**, *corsivo*, `codice`
- Liste come questa
- [Link](https://example.com)
- Immagini (vedi sotto)

## Aggiungere immagini

Carica le immagini nella cartella `assets/images/` e poi nel testo scrivi:

```markdown
![Descrizione immagine](/assets/images/nome-file.jpg)
```

> Questa è una citazione. Puoi usarla per evidenziare frasi importanti.

E questo è tutto — benvenuto nel blog!
