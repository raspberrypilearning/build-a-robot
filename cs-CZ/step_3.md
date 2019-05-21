## Přidání robotových očí

Pojďme přidělat tvému robotovi nějaké oči!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Projekt by měl vypadat přibližně takto:
    
    ![screenshot](images/robot-starter.png)

Každý obrázek v tomto projektu má své jméno (nebo **`id`**). Kupříkladu HTML kód, který představuje jednotlivé obrázky pro obličej a oči ('face', 'eyes1' a 'eyes2', začínající ve tvém kódu na řádku 8) vypadá takto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Můžeš také použít `id` obrázku a symbolu `#`, abys pomocí CSS stylů dodal obrázku vlastní styl. To ti umožňuje upravovat obrázky jeden po druhém.

Klikni na soubor `style.css`. Vidíš jak se liší velikost robotova obličeje a ostatních obrázků?

![screenshot](images/robot-id.png)

+ Přidej tento CSS kód, abys upravil robotovi oči:
    
        #eyes1 {
        width: 200px;
        }
        

Všimni si, že upravuješ pouze obrázek `eyes1`, a to právě díky `#eyes1` ve tvém CSS kódu. Pokud dáváš přednost jiným očím, můžeš namísto nich použít `#eyes2` nebo `#eyes3`!

![screenshot](images/robot-eyes-width.png)

Všiml sis, že jsou obrázky zobrazeny jeden za druhým? Tomuto se říká **relativní** pozicování. Chceš-li prohlížeči přesně říct, kam umístit robotovi oči, budeš namísto toho potřebovat použít **absolutní** pozicování.

+ Přidej tyto tři řádky CSS kódu pro obrázek `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Měl by jsi vidět, že oči tvého robota se přesunuly na správnou pozici.

![screenshot](images/robot-eyes-position.png)

Tento CSS kód říká prohlížeči jak daleko od levého horního okraje webové stránky se má zobrazit obrázek.

![screenshot](images/robot-eyes-position2.png)

Můžeš použít `bottom` namísto `top`, abys prohlížeči řekl, že má obrázek umisťovat od spodního okraje webové stránky. To samé platí pro `right` namísto `left` pro umísťování od pravého okraje.