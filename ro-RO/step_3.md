## Pune-i ochi robotului tău

Hai sa îi punem robotului tău niște ochi!

+ Deschide [acest fișier trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Proiectul ar trebui să arate astfel:
    
    ![captură de ecran](images/robot-starter.png)

Fiecare imagine din acest proiect are propriul ei nume (sau **`id`**). Spre exemplu, codul HTML pentru accesarea imaginilor care reprezintă față sau ochii (‘face’, ‘eyes1’, and ‘eyes2’, începând de pe linia 8 a codului tău) arată astfel:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Poți folosi `id`-ul unei imagini pentru a-i crea propriul stil, folosind CSS și simbolul `#`. Acest lucru îți va permite să stilizezi fiecare imagine separat.

Apasă pe fișierul `style.css`. Ai observat că exista o diferență între dimensiunea feței robotului și alte imagini?

![captură de ecran](images/robot-id.png)

+ Adaugă acest cod CSS pentru a modela ochii robotului:
    
        #eyes1 {
        width: 200px;
        }
        

Observă cum modelezi doar imaginea `eyes1`, folosind `#eyes1` în codul tău CSS. Dacă preferi alți ochi, folosește în schimb `#eyes2` sau `#eyes3`!

![captură de ecran](images/robot-eyes-width.png)

Observi cum fiecare imagine este afișată una după alta? Aceasta se numește poziționare**relative**. Dacă vrei să-i spui browserului exact unde vrei să pui ochii robotului, va trebui sa folosești poziționarea **absolute**.

+ Adaugă aceste trei linii codului tău CSS pentru imaginea ochilor `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Ar trebui să vezi că ochii robotului se mișcă către poziția corectă.

![captură de ecran](images/robot-eyes-position.png)

Acest cod CSS indică browserului cât de departe să afișeze imaginea față de colțul din stânga sus al paginii web.

![captură de ecran](images/robot-eyes-position2.png)

Poți folosi `bottom` în loc de `top` pentru a-i spune browserului cât de departe este, față de partea de jos a ecranului, pentru a afișa imaginea, la fel și pentru `right` în loc de `left`.