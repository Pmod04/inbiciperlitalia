# Come scrivere un articolo

Il modo più semplice per pubblicare senza usare Git:

1. Vai su **github.com** → il repository del blog
2. Entra nella cartella `_posts/`
3. Clicca **Add file → Create new file**
4. Scrivi il nome: `2001-10-11-titolo-articolo.md`
5. Incolla l'intestazione e cambia titolo e data
6. Scrivi quello che devi
7. Clicca **Commit changes**

## Intestazione necessaria

Ogni file DEVE iniziare con questo blocco: 

copia e incolla tutto all'inizio di ogni file puoi cambiare i campi title,date,author e tags ma non il campo layout

```yaml
---
layout: postx
title: "titolo"
date: 2001-10-11
author: Tommy
gpx: /assets/gpx/postx.gpx
tags:
---
```

## Aggiungere GPX (mappa)

Per aggiungere la mappa vai su [onthegomap](onthegomap.com) e segna il percorso che hai fatto, quando hai completato clicca su "export as GPX" e rinomina il file .gpx come esempio "post1.gpx" poi carichi il file su git in /assests/gpx

Poi nell'intestazione del post (quella qua sopra che devi copiare ogni volta, adesso c'è un parametro nuovo) devi mettere nel campo gpx: il percorso che sara appunto /assets/gpx/post1.gpx in questo esempio

Fatto ora nel post c'è la mappa


## Aggiungere Link

Per aggiungere un link metti il testo del link nelle parentesi quadre e l'url nelle tonde subito dopo, per esempio questa sintassi qua :

```
[sito di in bici per l'italia](https://pmod04.github.io/inbiciperlitalia/)
```
diventa :

[sito di in bici per l'italia](https://pmod04.github.io/inbiciperlitalia/)

## Aggiungere immagini

Carica le immagini nella cartella `assets/images/` e poi nel testo scrivi:

>Ho risolto la questione delle foto, per caricarne una incolla quello che c'è scritto qua sotto cambiando \[descrizione] con la descrizione della foto attuale e fra i due apostrofi '' dove ora c'è /assets/images/YYYY_MM_GG_titolopost_titolofoto.jpg ci metti /assets/images/ilnomedellafoto

> puoi semplicemente copiare il nome della foto se dopo averla caricata su github vai nella cartella /assets/images e la trovi lì, mi raccomando non modificare altre cose nel testo (tipo tolgiere apostrofi o parentesi) che copi da qua sotto sennò non funziona comunque se hai dubbi scrivimi

```markdown
![descrizione]({{ '/assets/images/YYYY_MM_GG_titolopost_titolofoto.jpg' | relative_url }})
```

> Ti conviene dare un nome ad ogni foto relativo al posst nella qualela foto si trova quindi per esempi se il post si chiama "post 3" la foto si chiama "2026_04_16_post3_amaca" e poi la carichi