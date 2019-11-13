## أعطِ روبوتك عيوناً

لنعطِ روبوتك بعض العيون!

+ افتح [هذا الـ trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    يجب أن يظهر المشروع بالشكل التالي:
    
    ![لقطة الشاشة](images/robot-starter.png)

كل صورة في هذا المشروع تملك اسماً خاصاً (أو **`id`**). فمثلاً، كود الـ HTML اللازم لتحديد صور الوجه والعين (‘face’, ‘eyes1’, ‘eyes2 ابتداءً من السطر 8 من الكود الخاص بك) سيكون كالتالي:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

يمكنك استعمال `id` أي صورة لتعطيها تنسيقها الخاص، وذلك باستخدام CSS ورمز الـ `#`. يتيح لك هذا تنسيق كل صورة بشكل منفصل.

اضغط على ملف `style.css`. هل لاحظت الاختلاف بين حجم وجه الروبوت وأحجام الصور الأخرى؟

![لقطة الشاشة](images/robot-id.png)

+ أضف كود الـ CSS التالي لتعديل تصميم عيون الروبوت:
    
        #eyes1 {
        width: 200px;
        }
        

لاحظ أنك تقوم بتعديل تصميم صورة العين الأولى `eyes1` فقط عند استخدام `#eyes1` في كود الـ CSS. إذا كنت تفضل أعيناً مختلفة، بإمكانك استخدام `#eyes2` أو `#eyes3` بدلاً من ذلك!

![لقطة الشاشة](images/robot-eyes-width.png)

هل لاحظت كيف تم عرض كل صورة تلو الأخرى؟ هذا يسمى بالتوضّع **النسبي (relative)**. إذا أردت إخبار المتصفح أين يجب أن تظهر أعين الروبوت بالتحديد، يجب أن تستخدم التوضّع **المطلق (absolute)** بدلاً من ذلك.

+ قم بإضافة الأسطر الثلاثة التالية لكود الـ CSS الخاص بصورة العين `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![لقطة الشاشة](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![لقطة الشاشة](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.