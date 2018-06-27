## Disegnare gli occhi del robot

Diamo al tuo robot gli occhi!

+ Apri [ questo trinket ](http://jumpto.cc/web-robot)
    
    Il progetto dovrebbe assomigliare a questo:
    
    ![screenshot](images/robot-starter.png)

Ogni immagine in questo progetto ha il proprio nome (o **` id `** ). Ad esempio, il codice HTML per cambiare le immagini del viso e degli occhi ("volto", "occhi1" e "occhi2", a partire dalla riga 8 del codice) ha il seguente aspetto:

    <img id="volto"...>
    <img id="occhi1"...>
    <img id="occhi2"...>
    

Puoi utilizzare l'ID ` dell'immagine ` per dargli un proprio stile, usando CSS e il simbolo ` # `. Questo ti permette di personalizzare ogni immagine separatamente.

Clicca sul file ` style.css `. Fai attenzione: come cambiano le dimensioni del viso del robot e le altre immagini?

![screenshot](images/robot-id.png)

+ Add this CSS code to style the robot’s eyes:
    
        #eyes1 {
        width: 200px;
        }
        

Notice that you’re styling just the `eyes1` image, by using `#eyes1` in your CSS code. If you prefer different eyes, you can use `#eyes2` or `#eyes3` instead!

![screenshot](images/robot-eyes-width.png)

Notice how each image is displayed one after the other? This is called **relative** positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.