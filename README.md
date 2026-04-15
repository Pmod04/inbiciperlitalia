---
layout: post
title: "Primo post - TEST"
date: 2026-04-14
author: Modena Pietro
tags: [test]
---

# Come scrivere un articolo

Il modo più semplice per pubblicare senza usare Git:

1. Vai su **github.com** → il repository del blog
2. Entra nella cartella `_posts/`
3. Clicca **Add file → Create new file**
4. Scrivi il nome: `2024-03-20-titolo-articolo.md`
5. Incolla il contenuto con il front matter
6. Clicca **Commit changes**

## Intestazione necessaria

Ogni file DEVE iniziare con questo blocco: 

copia e incolla tutto all'inizio di ogni file puoi cambiare i campi title,date,author e tags ma non il campo layout

```yaml
---
layout: post
title: "Il titolo del mio articolo"
date: 2024-03-20
author: Il Tuo Nome
tags: [tag1, tag2]
---
```

## Aggiungere Link

Per aggiungere un link metti il testo del link nelle parentesi quadre e l'url nelle tonde subito dopo, per esempio questa sintassi qua :

```
[sito di in bici per l'italia](https://inbiciperlitalia.com)
```
diventa :

[sito di in bici per l'italia](https://inbiciperlitalia.com)

## Aggiungere immagini

Carica le immagini nella cartella `assets/images/` e poi nel testo scrivi:

```markdown
![Descrizione immagine](/assets/images/nome-file.jpg)
```

> Ti conviene o fare delle sottocartelle per ogni post e poi usare quelle come reference, per esempio

>/asset/images/ <--- crei la nuova cartella qua
>quindi adesso hai /assets/images/post01/ e carichi le foto di quel post qua dentro
dopo per linkarle usi 
``` markdown
/assets/images/post01/nome-file.jpg
```
