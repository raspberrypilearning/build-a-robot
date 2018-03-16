## المقدمة

في هذا المشروع، ستتعلم كيف تحدِّد مواضع الصور لتنشئ روبوتًا!

![screenshot](images/robot-final.png)

### معلومات إضافية لقادة النادي

إذا كنت بحاجة إلى طباعة هذا المشروع، فيُرجى استخدام [نسخة سهلة الطباعة](https://projects.raspberrypi.org/en/projects/build-a-robot/print).


--- collapse ---
---
title: ملاحظات قادة النادي
---


## المقدمة:
في هذا المشروع، سيتعرَّف الأطفال على خاصية الموضع بلغة CSS عن طريق تصميم الروبوت.

## الموارد المتوفرة على الإنترنت

نوصي باستخدام [trinket](https://trinket.io/) لكتابة ملفات HTML وCSS على الإنترنت. يحتوي هذا المشروع على ملفات trinket التالية:

+ ['صمِّم روبوتًا' مشروع البدء -- jumpto.cc/web-robot](http://jumpto.cc/web-robot)

يمكن أن يستخدم الأطفال أيضًا ملف trinket الفارغ هذا [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) لكتابة ملفات HTML و CSS، أو يمكنهم استخدام قالب trinket هذا [(jumpto.cc/html-template)](http://jumpto.cc/html-template).

كما يوجد مشروع trinket يحتوي على نموذج حل للتحديات:

+ [مشروع 'صمِّم روبوتًا' مُكتمل -- trinket.io/html/00736c0e18](https://trinket.io/html/00736c0e18)

## الموارد المتوفرة دون اتصال بالإنترنت
بالنسبة إلى هذا المشروع، يمكن [إكماله دون اتصال بالإنترنت](https://www.codeclubprojects.org/en-GB/resources/webdev-working-offline/) إذا كنت تفضل ذلك. يمكنك الوصول إلى موارد المشروع من خلال النقر فوق رابط "مواد المشروع" الخاص بهذا المشروع. يحتوي هذا الرابط على قسم "موارد المشروع"، الذي يتضمن الموارد التي يحتاج إليها الأطفال لإكمال هذا المشروع دون اتصال بالإنترنت. تأكد من أن كل طفل لديه حق الوصول إلى نسخة من هذه الموارد. يتضمن هذا القسم الملفات التالية:

+ template/index.html
+ template/style.css
+ robot/index.html
+ robot/style.css
+ صور كثيرة بصيغة png

يمكنك أيضًا العثور على نسخة كاملة من تحديات هذا المشروع في قسم "موارد المتطوعين" الذي يحتوي على:

+ robot-finished/index.html
+ robot-finished/style.css
+ صور robot-finished كثيرة بصيغة png

(جميع الموارد المذكورة أعلاه قابلة للتنزيل أيضًا كملفات .zip للمشاريع والمتطوعين).

## أهداف التعلم
+ سمة id للغة HTML؛
+ الكتابة بلغة CSS:
	+ سمة محدد id `#`؛
	+ سمة position؛
	+ سمة top؛
	+ سمة left.

يتناول هذا المشروع عناصر من الصفوف التالية من [المناهج الرقمية الخاصة بـ Raspberry Pi](http://rpf.io/curriculum):

+ [الأصول الأساسية للتصميمات ثنائية الأبعاد وثلاثية الأبعاد](https://www.raspberrypi.org/curriculum/design/creator).

## التحديات:
+ "صمِّم روبوتك الخاص" - استخدام خاصية الموضع في لغة CSS لإنشاء روبوت؛
+ "أضف صورًا من عندك" - إضافة المزيد من الصور، باستخدام سمة id للغة HTML وتعليمة CSS البرمجية المقترنة.

## إكمال هذا المشروع دون اتصال بالإنترنت
إذا كان الأطفال يكملون هذا المشروع دون اتصال بالإنترنت، فسيحتاجون إلى حفظ الصور التي يخططون لاستخدامها في المجلد نفسه كملف `Robot.html`.

يمكنهم إضافة اسم الملف في أوسمة `<img>` فقط:

```
<img id="hat" src="hat.png" />
```

--- /collapse ---


--- collapse ---
---
title: مواد المشروع
---
## موارد المشروع
* [ملف .zip يحتوي على كل موارد المشروع](resources/robot-project-resources.zip)
* [Trinket عبر الإنترنت يحتوي على كل موارد المشروع 'صمِّم روبوتًا'](http://jumpto.cc/web-robot)
* [قالب Trinket عبر الإنترنت](http://jumpto.cc/trinket-template)
* [Trinket فارغ عبر الإنترنت](http://jumpto.cc/trinket-blank)
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

## موارد قادة النادي
[ملف .zip يحتوي على كل موارد المشاريع المكتملة](resources/robot-volunteer-resources.zip)
* [مشروع Trinket المكتمل على الإنترنت](https://trinket.io/html/00736c0e18)
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