## Disegnare gli occhi al robot

Disegniamo gli occhi al robot!


+ Apri questo trinket: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>.

    Il progetto si presenta così:

	![screenshot](images/robot-starter.png)

+ Ogni immagine del progetto ha un nome (o __id__). Ad esempio, l’HTML per le immagini di volto e occhi ("face", "eyes1" ed "eyes2" che inizia alla riga 8 del codice) si presenta così:

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ Puoi utilizzare l’id di un’immagine per attribuirle uno stile, utilizzando il simbolo `#`. In questo modo, puoi creare uno stile per ciascuna immagine separatamente.

Fai clic sul file `style.css`. Vedi la differenza tra le dimensioni del volto del robot e delle altri immagini?

![screenshot](images/robot-id.png)

+ Aggiungi il seguente codice CSS per cambiare lo stile degli occhi del robot:

```
#eyes1 {
    width: 200px;
}
```

Stai modificando solo lo stile dell’immagine `eyes1`, usando `#eyes1` nella sintassi CSS. Se preferisci, puoi utilizzare `#eyes2` o `#eyes3`!

![screenshot](images/robot-eyes-width.png)

+ Vedi come ogni immagine viene visualizzata una dopo l’altra? Questo aspetto prende il nome di posizionamento __relative__ (relativo). Se invece vuoi comunicare al browser dove posizionare esattamente gli occhi del robot, dovrai utilizzare il posizionamento __absolute__ (assoluto).

Aggiungi le seguenti 3 righe di codice al CSS per l’immagine `eyes1`:

```
position: absolute;
top: 200px;
left: 100px;
```

Gli occhi del robot dovrebbero spostarsi nella posizione corretta.

![screenshot](images/robot-eyes-position.png)

Il codice CSS comunica al browser a quale distanza visualizzare l’immagine dall’alto (top) e da sinistra (left) della pagina Web.

![screenshot](images/robot-eyes-position2.png)

Puoi utilizzare `bottom` (basso) invece di `top` (alto) per comunicare al browser la distanza a cui mostrare l’immagine dalla parte inferiore della schermata o da `right` (destra) invece di `left` (sinistra).

