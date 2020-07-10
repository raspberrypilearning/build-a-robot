## तुमच्या रोबोटला डोळे देवूया

चला तुमच्या रोबोटला काही डोळे दाखवू या !

+ [हे trinket](http://jumpto.cc/web-robot){:target="_blank"} उघडा.
    
    प्रकल्प असा दिसायला हवा:
    
    ![screenshot](images/robot-starter.png)

या प्रकल्पातील प्रत्येक प्रतिमेचे स्वतःचे नाव आहे (किंवा **`id`**). उदाहरणार्थ, चेहरा आणि डोळ्याच्या प्रतिमांना संबोधित करण्यासाठी (‘face’, ‘eyes1’, आणि ‘eyes2’, तुमच्या कोडच्या 8 व्या ओळीपासून सुरू होईल) HTML कोड असे दिसते:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

तुम्ही प्रतिमेचा `id` वापरुन त्यास त्याची स्वतःची शैली देण्यासाठी, CSS आणि `#` चिन्ह वापरू शकता. हे तुम्हाला प्रत्येक प्रतिमा स्वतंत्र शैलीत करण्याची परवानगी देते.

`style.css` फाईल वर क्लिक करा. रोबोटच्या चेहर्‍याचा आणि इतर प्रतिमांचा आकार कसा वेगळा आहे ते पहा?

![screenshot](images/robot-id.png)

+ रोबोटच्या डोळ्यांना शैली देण्यासाठी हा CSS कोड जोडा:
    
        #eyes1 {
        width: 200px;
        }
        

लक्षात घ्या की आपण फक्त `eyes1` प्रतिमेला शैली देत आहोत, आपल्या CSS कोडमध्ये `#eyes1` वापरुन. जर तुम्ही वेगळ्या प्रकारच्या डोळ्यांना प्राधान्य देत असल्यास, तुम्ही त्याऐवजी `#eyes2` किंवा `#eyes3` वापरू शकता !

![screenshot](images/robot-eyes-width.png)

एकामागून एक प्रतिमा कशी दाखवली जाते ते पहा. This is called **relative** positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.