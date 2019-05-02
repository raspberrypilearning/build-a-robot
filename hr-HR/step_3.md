## Dajte robotu oči

Dajmo vašem robotu neke oči!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Projekt bi trebao izgledati ovako:
    
    ![screenshot](images/robot-starter.png)

Svaka slika u ovom projektu ima svoje ime (ili **`id`**). Na primjer, HTML kôd za rješavanje slika lica i oka ("face", "eyes1" i "eyes2", počevši od linije 8 koda) izgleda ovako:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Možete koristiti slike u `id` dati svoj vlastiti stil, koristeći CSS i `#` simbol. Ovo vam omogućava stilu svaku sliku zasebno.

Kliknite na `style.css` datoteke. Primijetiti kako su različite veličine robot's lice i druge slike?

![screenshot](images/robot-id.png)

+ Dodajte ovaj CSS kôd kako biste oblikovali oči robota:
    
        #eyes1 {
        width: 200px;
        }
        

Primijetiti da ste stil samo `eyes1` slike, koristeći `#eyes1` u vaš CSS kod. Ako želite različite oči, možete koristiti `#eyes2` ili `#eyes3` umjesto!

![screenshot](images/robot-eyes-width.png)

Primijetite kako se svaka slika prikazuje jedan za drugim? To se zove **relativan** smještaj. Ako želite reći da je preglednik točno gdje želite smjestiti vaš robot oči, morat ćete koristiti **absolute** pozicioniranje umjesto toga.

+ Ove tri linije dodati CSS kod za sliku `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Trebali biste vidjeti da se oči vašeg robota kreću na ispravno mjesto na vašem robotu.

![screenshot](images/robot-eyes-position.png)

Ovaj CSS kôd govori pregledniku koliko daleko od gornjeg lijevog kuta web stranice za prikaz slike.

![screenshot](images/robot-eyes-position2.png)

Možete upotrijebiti `bottom` umjesto `top` da biste pregledniku rekli koliko daleko od dna zaslona treba prikazati sliku, kao i `right` umjesto `left`.