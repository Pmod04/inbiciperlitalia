---
layout: post
title: "Primo post - TEST"
date: 2026-04-14
author: Pietro
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
title: "titolo"
date: 2001-10-11
author: Tommy
tags:
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
![Descrizione immagine](assets/images/2026_04_16_post3_pastaalsugo)
```

> Ti conviene dare un nome ad ogni foto relativo al posst nella qualela foto si trova quindi per esempi se il post si chiama "post 3" la foto si chiama "2026_04_16_post3_pastaalsugo" e poi la carichi

Test immagine 

![rayman](assets/images/rayman.png)
