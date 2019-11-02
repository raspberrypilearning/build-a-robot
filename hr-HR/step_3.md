## Dajte robotu oči

Dajmo vašem robotu neke oči!

+ Otvorite [ovaj trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Projekt bi trebao izgledati ovako:
    
    ![screenshot](images/robot-starter.png)

Svaka slika u ovom projektu ima svoje ime (ili **`id`**). Na primjer, HTML kôd za rješavanje slika lica i oka ("face", "eyes1" i "eyes2", počevši od linije 8 koda) izgleda ovako:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Možete koristiti `id` slike kako bi im dali svoj vlastiti stil, koristeći CSS i `#` simbol. Ovo vam omogućava oblikovati svaku sliku zasebno.

Kliknite na `style.css` datoteke. Primijetite kako su veličine robotova lica i drugih slika različite.

![screenshot](images/robot-id.png)

+ Dodajte ovaj CSS kôd kako biste oblikovali oči robota:
    
        #eyes1 {
        width: 200px;
        }
        

Primijetite da oblikujete samo sliku `eyes1` koristeći `#eyes1` u vašem CSS kodu. Ako želite različite oči, možete koristiti `#eyes2` ili `#eyes3` umjesto toga!

![screenshot](images/robot-eyes-width.png)

Primijetite kako se svaka slika prikazuje jedna za drugom. To se zove **relativan** položaj. Ako želite reći pregledniku gdje da točno postavi oči vašeg robota, morat ćete umjesto toga koristiti **apsolutan** položaj.

+ Ove tri linije dodati CSS kodu za sliku `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Trebali biste vidjeti da se oči vašeg robota pomiču na ispravno mjesto na vašem robotu.

![screenshot](images/robot-eyes-position.png)

Ovaj CSS kôd govori pregledniku koliko daleko da prikaže sliku od gornjeg lijevog kuta web stranice.

![screenshot](images/robot-eyes-position2.png)

Možete upotrijebiti `bottom` umjesto `top` da biste pregledniku rekli koliko daleko od dna zaslona treba prikazati sliku, kao i `right` umjesto `left`.