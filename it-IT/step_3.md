## Disegnare gli occhi al tuo robot

Diamo al tuo robot degli occhi!

+ Apri [questo trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Il progetto dovrebbe assomigliare a questo:
    
    ![screenshot](images/robot-starter.png)

Ogni immagine in questo progetto ha il proprio nome (o **`id`**). Ad esempio, il codice HTML per cambiare le immagini del viso e degli occhi ("face", "eyes1" e "eyes2", a partire dalla riga 8 del codice) ha il seguente aspetto:

    <img id="face"...>
    <img id="eyes1"...>
    <img id="eyes2"...>
    

Puoi utilizzare l'`ID` dell'immagine per dargli un proprio stile, usando CSS e il simbolo `#`. Questo ti permette di personalizzare ogni immagine separatamente.

Clicca sul file `style.css`. Nota come la dimensione della faccia del robot e le altre immagini sono diverse?

![screenshot](images/robot-id.png)

+ Aggiungi questo codice CSS per modellare gli occhi del robot:
    
        #eyes1 {
        width: 200px;
        }
        

Nota che stai modellando solo l'immagine `#eyes1` se usi `#eyes1` nel tuo codice CSS. Se preferisci avere occhi diversi, puoi usare `#eyes2` o `#eyes3`!

![screenshot](images/robot-eyes-width.png)

Hai notato come le immagini vengono visualizzate una dopo l'altra? Questo è chiamato posizionamento **relativo**. Invece, se vuoi dire al browser esattamente dove posizionare gli occhi del tuo robot, dovrai usare il posizionamento **assoluto**.

+ Aggiungi queste tre linee al codice CSS per la tua immagine `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Dovresti vedere che gli occhi si spostano nella posizione corretta sul tuo robot.

![screenshot](images/robot-eyes-position.png)

Questo codice CSS indica al browser quanto deve essere lontana l'immagine da visualizzare dall'angolo in alto a sinistra della pagina web.

![screenshot](images/robot-eyes-position.png)

Puoi usare `bottom` al posto di `top` per dire al browser quanto lontana l'immagine deve essere dalla parte inferiore dello schermo, così come `right` al posto di `left`.