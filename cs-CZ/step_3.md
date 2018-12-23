## Přidělej svému robotovi oči

Pojďme přidělat tvému robotovi nějaké oči!

+ Otevřete [tento trinket](http://jumpto.cc/web-robot).
    
    Projekt by měl vypadat přibližně takto:
    
    ![screenshot](images/robot-starter.png)

Každý obrázek v tomto projektu má své jméno (nebo **`id`**). Kupříkladu HTML kód, který představuje jednotlivé obrázky pro obličej a oči ('face', 'eyes1' a 'eyes2', začínající ve tvém kódu na řádku 8) vypadá takto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Můžeš také použít `id` obrázku a symbolu `#`, abys pomocí CSS stylů dodal obrázku vlastní styl. To ti umožňuje upravovat obrázky jeden po druhém.

Klikni na soubor `style.css`. Všimni si rozdílu ve velikost obličeje robota a jeho ostatními součáskami. Jsou přirozeně velké?

![screenshot](images/robot-id.png)

+ Přidej tento CSS kód, abys upravil robotovi oči:
    
        #eyes1 {
        width: 200px;
        }
        

Všimni si, že upravuješ pouze obrázek `eyes1`, a to právě díky `#eyes1` ve tvém CSS kódu. Pokud dáváš přednost jiným očím, můžeš namísto nich použít `#eyes2` nebo `#eyes3`!

![screenshot](images/robot-eyes-width.png)

Všiml sis, že jsou obrázky zobrazeny jeden za druhým? Tomuto se říká **relativní** pozicování. Chceš-li prohlížeči přesně říct, kam umístit robotovi oči, budeš namísto toho potřebovat použít **absolutní pozicování**.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.