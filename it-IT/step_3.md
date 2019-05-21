## Disegnare gli occhi del robot

Diamo al tuo robot degli occhi!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Il progetto dovrebbe assomigliare a questo:
    
    ![screenshot](images/robot-starter.png)

Ogni immagine in questo progetto ha il proprio nome (o **` id`**). Ad esempio, il codice HTML per cambiare le immagini del viso e degli occhi ("volto", "occhi1" e "occhi2", a partire dalla riga 8 del codice) ha il seguente aspetto:

    <img id="volto"...>
    <img id="occhi1"...>
    <img id="occhi2"...>
    

Puoi utilizzare l'`ID` dell'immagine per dargli un proprio stile, usando CSS e il simbolo ` #`. Questo ti permette di personalizzare ogni immagine separatamente.

Clicca sul file ` style.css`. Hai fatto caso a come cambiano le dimensioni del viso del robot e le altre immagini?

![screenshot](images/robot-id.png)

+ Aggiungi questo codice CSS per modellare gli occhi del robot:
    
        #occhi1 {
        width: 200px;
        }
        

Fai caso al fatto che stai modellando solo l'immagine `#occhi1` nel tuo codice CSS. Se preferisci avere occhi diversi, puoi usare `#occhi2` o `#occhi3`!

![screenshot](images/robot-eyes-width.png)

Hai fatto caso a come ciascuna immagine viene visualizzata una dopo l'altra? Questo è chiamato il posizionamento **relativo**. Invece, se vuoi dire al browser esattamente dove posizionare gli occhi del tuo robot, dovrai usare il posizionamento ** assoluto**.

+ Aggiungi queste tre linee al codice CSS per la tua immagine ` occhi1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Dovresti vedere che gli occhi del tuo robot si spostano nella posizione corretta sul tuo robot.

![screenshot](images/robot-eyes-position.png)

Questo codice CSS indica al browser quanto deve essere lontana dall'angolo in alto a sinistra della pagina web l'immagine da visualizzare.

![screenshot](images/robot-eyes-position2.png)

Puoi usare `bottom` al posto di `top` per dire al browser quanto lontana dalla parte inferiore dello schermo l'immagine deve essere, così come `right` al posto di `left`.