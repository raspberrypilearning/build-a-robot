## Dodavanje očiju

Dodajmo tvom robotu oči!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Projekat treba da izgleda ovako:
    
    ![screenshot](images/robot-starter.png)

Svaka slika u ovom projektu ima svoj naziv (ili **`id`**). Na primjer, HTML kôd za slike lica i očiju ('face', 'eyes1' i 'eyes2', koji počinje u 8. redu tvog kôda) izgleda ovako:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Možeš koristiti `id` slike da joj dodijeliš njen sopstveni stil, koristeći CSS i znak `#`. Ovo ti omogućava da svaku sliku posebno stilizuješ.

Klikni na `style.css` datoteku. Primjećuješ li da postoji razlika u veličini robotovog lica i ostalih slika?

![screenshot](images/robot-id.png)

+ Dodaj ovaj CSS kôd kojim ćeš stilizovati robotove oči:
    
        #eyes1 {
        width: 200px;
        }
        

Imaj u vidu da stilizuješ samo sliku `eyes1`, koristeći `#eyes1` u svom CSS kôdu. Ako želiš drugačije oči, možeš koristiti `#eyes2` ili `#eyes3`!

![screenshot](images/robot-eyes-width.png)

Primjećuješ li kako se slike prikazuju jedna za drugom? To se zove **relativno** pozicioniranje. Ako želiš da kažeš pregledaču gdje tačno da postavi robotove oči, umjesto relativnog, treba da koristiš **apsolutno** pozicioniranje.

+ CSS kôdu za sliku `eyes1` dodaj sljedeća tri reda:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Vidjećeš da se oči tvog robota pomjeraju na ispravno mjesto.

![screenshot](images/robot-eyes-position.png)

Ovaj CSS kôd pokazuje pregledaču koliko daleko od lijevog gornjeg ugla veb-stranice treba prikazati sliku.

![screenshot](images/robot-eyes-position2.png)

Umjesto `top`, možeš koristiti `bottom` da kažeš pregledaču koliko daleko od dna ekrana treba prikazati sliku. Isto tako, možeš da koristiš `right` umjesto `left`.