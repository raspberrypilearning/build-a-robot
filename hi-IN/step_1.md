## भूमिका

इस प्रोजेक्ट में, आप अपना स्वयं का रोबोट बनाने के लिए छवियों की स्थिति निर्धारित करना सीखेंगे!

![screenshot](images/robot-final.png)

### क्लब लीडर्स के लिए अतिरिक्त जानकारी

यदि आप इस प्रोजेक्ट को प्रिंट करना चाहते हैं, तो कृपया [प्रिंटर के लिए अनुकूल संस्करण](https://projects.raspberrypi.org/en/projects/build-a-robot/print) का उपयोग करें।


--- collapse ---
---
title: क्लब लीडर के नोट्स
---


## भूमिका:
इस प्रोजेक्ट में, बच्चे अपना स्वयं का रोबोट बनाकर CSS के स्थिति-निर्धारण के बारे में जानेंगे।

## ऑनलाइन संसाधन

HTML और CSS को ऑनलाइन लिखने के लिए हम [trinket](https://trinket.io/) का उपयोग करने की अनुशंसा करते हैं। इस प्रोजेक्ट में निम्नलिखित ट्रिंकेट शामिल होते हैं:

+ ['रोबोट बनाएँ' प्रारंभिक बिंदु -- jumpto.cc/web-robot](http://jumpto.cc/web-robot)

बच्चे स्वयं का HTML और CSS लिखने के लिए इस [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) खाली ट्रिंकेट का भी उपयोग कर सकते हैं, या वैकल्पिक तौर पर वे इस टैंपलेट ट्रिंकेट का उपयोग कर सकते हैं [(jumpto.cc/html-template)](http://jumpto.cc/html-template)।

ऐसा ट्रिंकेट भी होता है, जिसमें चुनौतियों के लिए हल का नमूना शामिल होता है:

+ ['रोबोट बनाएँ' पूर्ण -- trinket.io/html/00736c0e18](https://trinket.io/html/00736c0e18)

## ऑफ़लाइन संसाधन
यदि चाहें तो इस प्रोजेक्ट को [ऑफ़लाइन पूरा किया जा सकता है](https://www.codeclubprojects.org/en-GB/resources/webdev-working-offline/)। आप इस प्रोजेक्ट के लिए 'प्रोजेक्ट सामग्री' लिंक पर क्लिक करके प्रोजेक्ट के स्रोतों का उपयोग कर सकते हैं। इस लिंक में 'प्रोजेक्ट संसाधन' भाग शामिल है, जिसमें ऐसे स्रोत शामिल हैं जिनकी आवश्यकता बच्चों को अपने प्रोजेक्ट ऑफ़लाइन पूरा करने के लिए हो सकती है। सुनिश्चित करें कि प्रत्येक बच्चे की इन स्रोतों तक पहुँच है। इस भाग में निम्नलिखित फाइलें शामिल हैं:

+ template/index.html
+ template/style.css
+ robot/index.html
+ robot/style.css
+ Lots of .png images

आप इस प्रोजेक्ट की चुनौतियों का पूर्ण संस्करण 'स्वैच्छिक संसाधन' भाग में भी देख सकते हैं, जिसमें ये शामिल हैं:

+ robot-finished/index.html
+ robot-finished/style.css
+ robot-finished/Lots of .png images

(उपर्युक्त सभी स्रोत प्रोजेक्ट और स्वैच्छिक `.zip` फाइलों के रूप में डाउनलोड योग्य हो सकते हैं।)

## अधिगम उद्देश्य
+ HTML id के गुण;
+ CSS लिखना:
	+ `#` id सिलेक्टर;
	+ स्थिति;
	+ शीर्ष;
	+ बाएँ।

इस प्रोजेक्ट में [Raspberry Pi डिजिटल निर्माण पाठ्यचर्या](http://rpf.io/curriculum) के निम्नलिखित गुणों के तत्व शामिल हैं:

+ [आधारभूत 2D और 3D संपदाएँ डिज़ाइन करें](https://www.raspberrypi.org/curriculum/design/creator).

## चुनौतियाँ
+ "अपना स्वयं का रोबोट डिज़ाइन करें" – रोबोट बनाने के लिए CSS की स्थिति लागू करना;
+ "अपनी स्वयं के छवियाँ जोड़ें" - HTML id गुण और संबंधित CSS द्वारा और छवियाँ जोड़ना।

## इस प्रोजेक्ट को ऑफ़लाइन पूरा करना
यदि बच्चे इस प्रोजेक्ट को ऑफ़लाइन पूरा कर रहे हैं, तो उन्हें उन छवियों को `Robot.html` फाइल वाले फ़ोल्डर में सहेजना होगा, जिनका वे उपयोग करना चाहते हैं।

इसके बाद वे बस `<img>` टैग में फाइल का नाम जोड़ सकते हैं:

```
<img id="hat" src="hat.png" />
```

--- /collapse ---


--- collapse ---
---
title: प्रोजेक्ट सामग्री
---
## प्रोजेक्ट संसाधन
* [सभी प्रोजेक्ट स्रोतों सहित .zip फाइल](resources/robot-project-resources.zip)
* [सभी 'रोबोट बनाएँ' प्रोजेक्ट संसाधनों सहित ऑनलाइन ट्रिंकेट](http://jumpto.cc/web-robot)
* [ऑनलाइन ट्रिंकेट टेम्प्लेट](http://jumpto.cc/trinket-template)
* [ऑनलाइन खाली ट्रिंकेट](http://jumpto.cc/trinket-blank)
* [template/index.html](resources/template-index.html)
* [template/style.css](resources/template-style.css)
* [robot/index.html](resources/robot-index.html)
* [robot/style.css](resources/robot-style.css)
* [robot/antenna.png](resources/robot-antenna.png)
* [robot/bird.png](resources/robot-bird.png)
* [robot/bowtie.png](resources/robot-bowtie.png)
* [robot/crown.png](resources/robot-crown.png)
* [robot/ears1.png](resources/robot-ears1.png)
* [robot/ears2.png](resources/robot-ears2.png)
* [robot/eyes1.png](resources/robot-eyes1.png)
* [robot/eyes2.png](resources/robot-eyes2.png)
* [robot/eyes3.png](resources/robot-eyes3.png)
* [robot/face.png](resources/robot-face.png)
* [robot/hair1.png](resources/robot-hair1.png)
* [robot/hair2.png](resources/robot-hair2.png)
* [robot/hair3.png](resources/robot-hair3.png)
* [robot/hair4.png](resources/robot-hair4.png)
* [robot/hat.png](resources/robot-hat.png)
* [robot/headphones.png](resources/robot-headphones.png)
* [robot/moustache.png](resources/robot-moustache.png)
* [robot/mouth1.png](resources/robot-mouth1.png)
* [robot/mouth2.png](resources/robot-mouth2.png)
* [robot/mouth3.png](resources/robot-mouth3.png)
* [robot/necklace.png](resources/robot-necklace.png)
* [robot/nose1.png](resources/robot-nose1.png)
* [robot/nose2.png](resources/robot-nose2.png)
* [robot/nose3.png](resources/robot-nose3.png)
* [robot/sunglasses.png](resources/robot-sunglasses.png)

## क्लब लीडर के संसाधन
* [सभी पूर्ण प्रोजेक्ट स्रोतों सहित .zip फाइल](resources/robot-volunteer-resources.zip)
* [ऑनलाइन पूर्ण ट्रिंकेट प्रोजेक्ट](https://trinket.io/html/00736c0e18)
* [robot-finished/index.html](resources/robot-finished-index.html)
* [robot-finished/style.css](resources/robot-finished-style.css)
* [robot-finished/antenna.png](resources/robot-finished-antenna.png)
* [robot-finished/bird.png](resources/robot-finished-bird.png)
* [robot-finished/bowtie.png](resources/robot-finished-bowtie.png)
* [robot-finished/crown.png](resources/robot-finished-crown.png)
* [robot-finished/ears1.png](resources/robot-finished-ears1.png)
* [robot-finished/ears2.png](resources/robot-finished-ears2.png)
* [robot-finished/eyes1.png](resources/robot-finished-eyes1.png)
* [robot-finished/eyes2.png](resources/robot-finished-eyes2.png)
* [robot-finished/eyes3.png](resources/robot-finished-eyes3.png)
* [robot-finished/face.png](resources/robot-finished-face.png)
* [robot-finished/hair1.png](resources/robot-finished-hair1.png)
* [robot-finished/hair2.png](resources/robot-finished-hair2.png)
* [robot-finished/hair3.png](resources/robot-finished-hair3.png)
* [robot-finished/hair4.png](resources/robot-finished-hair4.png)
* [robot-finished/hat.png](resources/robot-finished-hat.png)
* [robot-finished/headphones.png](resources/robot-finished-headphones.png)
* [robot-finished/moustache.png](resources/robot-finished-moustache.png)
* [robot-finished/mouth1.png](resources/robot-finished-mouth1.png)
* [robot-finished/mouth2.png](resources/robot-finished-mouth2.png)
* [robot-finished/mouth3.png](resources/robot-finished-mouth3.png)
* [robot-finished/necklace.png](resources/robot-finished-necklace.png)
* [robot-finished/nose1.png](resources/robot-finished-nose1.png)
* [robot-finished/nose2.png](resources/robot-finished-nose2.png)
* [robot-finished/nose3.png](resources/robot-finished-nose3.png)
* [robot-finished/sunglasses.png](resources/robot-finished-sunglasses.png)

--- /collapse ---