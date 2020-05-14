## রোবটটি কে চোখ দান করুন 

আসুন আপনার রোবটটি কে চোখ দিন!

+ [এই ট্রিংকেটটি খুলুন](http://jumpto.cc/web-robot) {:target="_ blank"}।
    
    আপনার প্রকল্প এমন দেখতে হওয়া উচিত:
    
    ![স্ক্রীনশট](images/robot-starter.png)

এই প্রকল্পের প্রতিটি চিত্রের নিজস্ব নাম আছে (অথবা **`id`**)। উদাহরণস্বরূপ, মুখ এবং চোখের চিত্রগুলিকে সম্বোধনের জন্য এইচটিএমএল কোড ('চেহারা', 'চোখ 1', এবং 'চোখ 2') এর মতো দেখাচ্ছে যা আপনার কোডের ৮ নাম্বার লাইন এ দেখা যাচ্ছে: 

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

সিএসএস (CSS) এবং `#` চিন্হ ব্যবহার করে একটা ছবির `id` দিয়ে আপনার নিজস্ব ধরণ দিতে পারেন। আপনি প্রতিটা ছবির আলাদা আলাদা ধরণ বানাতে পারেন।

`style.css` ফাইলটির ওপর ক্লিক করুন। লক্ষ্য করুন রোবটের মুখের আকার এবং অন্যান্য চিত্রগুলি কিভাবে আলাদা।

![স্ক্রীনশট](images/robot-id.png)

+ রোবটের চোখের স্টাইল করতে এই সিএসএস (CSS) কোড যোগ করুন:
    
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