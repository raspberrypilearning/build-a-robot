## Geef ogen aan je robot

Laten we je robot een paar ogen geven!

+ Open [deze trinket](http://jumpto.cc/web-robot).
    
    Het project zou er als volgt uit moeten zien:
    
    ![screenshot](images/robot-starter.png)

Elke afbeelding in dit project heeft een eigen naam (of een**` ID`**). Bijvoorbeeld, de HTML-code om naar de afbeeldingen van het gezicht en de ogen te verwijzen ('gezicht', 'ogen1' en 'ogen2', beginnend op regel 8 van de code) ziet er als volgt uit:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Je kunt het `id` van een afbeelding gebruiken om er een stijl aan te geven, door CSS te gebruiken met het `#` teken. Hiermee kun je elke afbeelding apart opmaken.

Klik op het `style.css` bestand. Kun je zien dat er een verschil is tussen de grootte van het gezicht van de robot en de andere afbeeldingen?

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