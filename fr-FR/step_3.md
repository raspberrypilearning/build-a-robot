## Donner des yeux à ton robot

Donnons des yeux à ton robot !

+ Ouvre [ce trinket](http://jumpto.cc/web-robot).
    
    Le projet doit ressembler à ça:
    
    ![screenshot](images/robot-starter.png)

Chaque image dans le projet a son propre nom (ou **`id`**). Par exemple, le code HTML pour traiter le visage et les images d'yeux ('visage', 'yeux1' et 'yeux2', à partir de la ligne 8 de ton code) resselle à ça:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Tu peux utiliser les `id` des images pour leur donner leur propre style, en utilisant du CSS grâce au symbole `#`. Cela te permet de changer le style de chaque image séparément.

Clique sur le fichier `style.css`. As-tu remarqué comment la taille du visage du robot et des autres images est différente ?

![screenshot](images/robot-id.png)

+ Ajoute ce code CSS pour modifier le style des yeux du robot :
    
        #yeux1 {
        width: 200px;
        }
        

Note que tu ne modifies l'apparence que de l'image `yeux1` en utilisant `#yeux1` dans ton code CSS. Si tu préfères des yeux différents, tu peux utiliser `#yeux2` ou `yeux3` à la place !

![screenshot](images/robot-eyes-width.png)

As-tu remarqué comment chaque image est affichée l'une après l'autre ? On appelle ceci positionnement **relatif**. Si tu souhaites dire au navigateur où placer exactement les yeux de ton robot, tu devras utiliser des positionnements **absolus** à la place.

+ Ajoute ces trois lignes à ton code CSS pour ton image `yeux1` :
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.