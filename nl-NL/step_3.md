## Geef ogen aan je robot

Laten we je robot een paar ogen geven!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    Het project zou er als volgt uit moeten zien:
    
    ![screenshot](images/robot-starter.png)

Elke afbeelding in dit project heeft een eigen naam (of een**` ID`**). Bijvoorbeeld, de HTML-code om naar de afbeeldingen van het gezicht en de ogen te verwijzen ('face', 'eyes1' en 'eyes2', beginnend op regel 8 van de code) ziet er als volgt uit:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Je kunt het `id` van een afbeelding gebruiken om er een stijl aan te geven, door CSS te gebruiken met het `#` teken. Hiermee kun je elke afbeelding apart opmaken.

Klik op het `style.css` bestand. Kun je zien dat er een verschil is tussen de grootte van het gezicht van de robot en de andere afbeeldingen?

![screenshot](images/robot-id.png)

+ Voeg deze CSS-code toe om de ogen van de robot een andere stijl te geven:
    
        #eyes1 {
        width: 200px;
        }
        

Je ziet dat je alleen `eyes1` aan het opmaken bent door `#eyes1` te gebruiken in de CSS-code. Als je andere ogen wilt, kun je `#eyes2` of `#eyes3` in de plaats gebruiken.

![screenshot](images/robot-eyes-width.png)

Zie je dat de afbeeldingen naast elkaar staan? Dat heet **relatief **positioneren. Als je zelf wilt bepalen waar de ogen van de robot komen te staan gebruik je **absolute** positionering.

+ Voeg deze drie regels toe aan de CSS-code voor de` ogen1 ` afbeelding:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Je zou moeten zien dat de ogen naar de juiste plaats op je robot komen.

![screenshot](images/robot-eyes-position.png)

Deze CSS-code geeft door aan de browser hoe ver van de linkerbovenhoek van de webpagina de afbeelding wordt weergegeven.

![screenshot](images/robot-eyes-position2.png)

Je kunt ` bottom ` gebruiken, in plaats van ` top ` om aan de browser door te geven hoe ver van onder aan het scherm de afbeelding wordt weergegeven. Zoiets kun je ook doen met ` right ` in plaats van ` left `.