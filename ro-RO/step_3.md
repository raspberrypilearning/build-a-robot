## Pune-i robotului tău, ochii

Haideți sa-inpunem robotului niște ochi!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Proiectul ar trebui să arate astfel:
    
    ![captură de ecran](images/robot-starter.png)

Fiecare imagine din acest proiect are propriul ei nume (or **`id`**). Spre exemplu, codul HTML pentru accesarea imaginilor cu față sau ochi (‘face’, ‘eyes1’, and ‘eyes2’, starting on line 8 of your code) arată astfel:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Poți folosi imaginea `id` penttu a creea stilul tău peopriu, folosind CSS și simbolul `#` symbol. Asta îți va permite să modifici fiecare imagine separat.

Apasă pe fișierul `style.css`. Ai observat diferența dintre dimensiunea feței robotului și alte imagini sunt diferite?

![captură de ecran](images/robot-id.png)

+ Adăugați acest cod CSS pentru a modela ochii robotului:
    
        #eyes1 {
        width: 200px;
        }
        

Observi ca modelezi doar imaginea `eyes1`, folosind `#eyes1` în codul tăuin CSS. Dacă preferi alți ochi, folosește în schimb `#eyes2` or `#eyes3`!

![captură de ecran](images/robot-eyes-width.png)

Observați cum este afișată fiecare imagine una după alta? Aceasta se numește pozitionare**relative**. Dacă vrei să-i spui browserului exact unde vrei sa pui ochii robotului, va trebui sa dolosești pozitionarea **absolute**.

+ Adaugă aceste trei linii codului tău CSS pentru imaginea `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Ar trebui să veI că ochii robotului se mișcă către poziția corectă.

![captură de ecran](images/robot-eyes-position.png)

Acest cod CSS indică browserului cât de departe este, față de colțul din stânga sus al paginii web, pentru a afișa imaginea.

![captură de ecran](images/robot-eyes-position2.png)

Poți folosi `bottom` în loc de `top` pentru a-i spune browserului cât de departe este, față de partea de jos a ecranului, pentru a afișa imaginea, la fel și pentru `right` în loc de `left`.