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