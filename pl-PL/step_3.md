## Dodawanie oczu

Dodajmy oczy twojemu robotowi!

+ Otwórz [edytor trinket](http://jumpto.cc/web-robot).
    
    Projekt powinien wyglądać następująco:
    
    ![zrzut ekranu](images/robot-starter.png)

Każdy obrazek w projekcie ma swoją nazwę (albo **`id`**). Na przykład kod HTML odwołujący się do grafik twarzy i oczu ('face', 'eyes1' i 'eyes2', zaczynając od linii 8 twojego kodu) wygląda następująco:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Możesz użyć `id` grafiki, aby nadać jej własne style, używając CSS i symbolu `#`. To pozwoli ci ostylować każdy obrazek z osobna.

Kliknij na plik `style.css`. Widzisz, że rozmiar grafiki twarzy robota różni się od rozmiarów innych grafik?

![zrzut ekranu](images/robot-id.png)

+ Dodaj ten kod CSS aby ostylować oczy robota:
    
        #eyes1 {
        width: 200px;
        }
        

Zauważ, że używając `#eyes1` w swoim kodzie CSS ostylujesz tylko grafikę `eyes1`. Jeżeli wolisz użyć innych oczu, możesz skorzystać z selektorów `#eyes2` albo `#eyes3`!

![zrzut ekranu](images/robot-eyes-width.png)

Widzisz, jak obrazki są wyświetlane jeden po drugim? To nazywa się pozycjonowanie **relatywne**. Jeżeli chcesz poinstruować przeglądarkę, gdzie dokładnie powinny zostać umieszczone oczy robota, będziesz musiał użyć pozycjonowania **absolutnego**.

+ Dodaj te trzy linie do kodu CSS dla grafiki `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Powinieneś zobaczyć, jak oczy twojego robota przemieściły się w oczekiwane miejsce.

![zrzut ekranu](images/robot-eyes-position.png)

Ten kod CSS mówi przeglądarce, jak daleko od górnego lewego rogu strony wyświetlić obrazek.

![zrzut ekranu](images/robot-eyes-position2.png)

Możesz użyć `bottom` zamiast `top`, aby powiedzieć przeglądarce jak daleko od dołu ekranu pokazać grafikę, jak również `right` zamiast `left`, aby pozycjonować ją względem prawej krawędzi.