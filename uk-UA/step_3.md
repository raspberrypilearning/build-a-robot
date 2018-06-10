## Дайте Вашому роботу очі

Давайте дамо Вашому роботу очі!

+ Відкрийте [this trinket](http://jumpto.cc/web-robot).
    
    Проект повинен виглядати так:
    
    ![screenshot](images/robot-starter.png)

Кожне зображення в цьому проекті має своє ім'я (або **`id`**). Наприклад, HTML-код для адреси обличчя та очей ("face", "eyes1" і "eyes2", починаючи з 8-го рядка вашого коду) виглядає так:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Ви можете використовувати `id` для зображення, щоб надати йому свій стиль, використовуючи CSS та символ ` # </ 0>. Це дозволяє стиснути кожне зображення окремо.</p>

<p>Натисніть на файл <code> style.css </ 0>. Зверніть увагу, як розмір обличчя робота та інших зображень відрізняються</p>

<p><img src="images/robot-id.png" alt="screenshot" /></p>

<ul>
<li><p>Додайте цей CSS-код, для стилю очей робота:</p>

<pre><code>#eyes1 {
ширина: 200 пікс;
}
`</pre></li> </ul> 

Зверніть увагу, що ви використовуєтелише стиль зображення ` eyes1 </ 0>, використовуючи <code> # eyes1 </ 0> у вашому CSS-коді. Якщо ви віддаєте перевагу різним очам, ви можете використовувати <code> # eyes2 </ 0> або <code> # eyes3 </ 0>!</p>

<p><img src="images/robot-eyes-width.png" alt="screenshot" /></p>

<p>Зверніть увагу, як кожне зображення появляється одне за одним? Це називається <strong>relative</strong>позиціонування. Якщо ви хочете сказати браузеру, де саме розмістити очі вашого робота, вам слід скористатися позиціонуванням  <strong>absolute</strong>.</p>

<ul>
<li><p>Додайте ці три рядки до коду CSS для свого зображення <code> eyes1 </ 0>:</p>

<pre><code>розміщення: абсолютно;
зверху: 200 пікселів;
ліворуч: 100 пікселів;
`</pre></li> </ul> 

Ви повинні побачити, що очі вашого робота рухаються до правильного місця на вашому роботі.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.