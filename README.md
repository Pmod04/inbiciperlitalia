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
[sito di in bici per l'italia](https://pmod04.github.io/inbiciperlitalia/)
```
diventa :

[sito di in bici per l'italia](https://pmod04.github.io/inbiciperlitalia/)

## Aggiungere immagini

Carica le immagini nella cartella `assets/images/` e poi nel testo scrivi:

>Ho risolto la questione delle foto, per caricarne una incolla quello che c'è scritto qua sotto cambiando "amaca" con la descrizione della foto attuale e fra i due apostrofi '' dove ora c'è /assets/images/2026_04_16_Prova_per_scrivere_Amaca.jpg ci metti /assets/images/nomedellafotoblablabla.estnsione puoi semplicemente copiare il nome della foto se dopo averla caricata su github vai nella cartella /assets/images e la trovi lì, mi raccomando non modificare altre cose nel testo che copi da qua sotto sennò non funziona comunque se hai dubbi scrivimi

```markdown
![amaca]({{ '/assets/images/2026_04_16_Prova_per_scrivere_Amaca.jpg' | relative_url }})
```

> Ti conviene dare un nome ad ogni foto relativo al posst nella qualela foto si trova quindi per esempi se il post si chiama "post 3" la foto si chiama "2026_04_16_post3_pastaalsugo" e poi la carichi