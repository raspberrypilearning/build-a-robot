## أعطي روبوتك عيون

لنعطي روبوتك بعض العيون!

+ لنفتح هذا القوس {:target="_blank"}.
    
    يجب ان يبدو الملف مثل هذا:
    
    ![لقطة الشاشة](images/robot-starter.png)

كل صوره في المشروع تملك اسماً خاصاً (او id). على سبيل المثال, كود الHTML الذي يحدد صور الوجه والعين (‘face’, ‘eyes1’, ‘eyes2 يبدا في السطر 8 من الكود الخاص بك) يبدوا مثل هذا:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

يمكنك استعمال ال id الخاص باحدى الصوره لأعطاء الشكل لها, باستعمال CSS و رمز #. هذا يتيح لك لاعطاء الشكل لكل صوره بشكل منفصل.

انقر على ملف "style.css". لاحظ كيف يختلف حجم وجه الروبوت و حجم الصور الاخرى؟

![لقطة الشاشة](images/robot-id.png)

+ ضع كود ال CSS هذا لتعديل شكل عيون الروبوت:
    
        #eyes1 {
        width: 200px;
        }
        

لاحظ انك تغير شكل صورة العين الاولى فقط eyes1, بأستعمال eyes1 # في ملف الCSS. If you prefer different eyes, you can use `#eyes2` or `#eyes3` instead!

![لقطة الشاشة](images/robot-eyes-width.png)

Notice how each image is displayed one after the other? This is called **relative** positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![لقطة الشاشة](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![لقطة الشاشة](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.