## 给你的机器人一双眼睛

让我们来给你的机器人一双眼睛！



+ 打开这个 trinket：<a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>。

    此项目应如下所示：

	![screenshot](images/robot-starter.png)

+ 本项目中的每张图片都有自己的名字（或者 __id__）。例如，面部和眼睛图片的 HTML（始于代码第 8 行的‘face’、‘eyes1’和‘eyes2’）如下所示：

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ 你可以通过使用 `#` 符号，来运用图片的 id 表现其自身的样式。这使你能分别设计每个图片的样式。

点击 `style.css` 文件。注意机器人面部与其他图片的尺寸有什么不同？

![screenshot](images/robot-id.png)

+ 添加以下 CSS 代码来设置机器人眼睛的样式：

```
## eyes1 {
    width: 200px;
}
```

请注意，你现在使用 CSS 中的 `## eyes1` 所设置的仅仅是 `eyes1` 图片的样式。如果你愿意，你可以使用 `#eyes2` 或 `#eyes3`！

![screenshot](images/robot-eyes-width.png)

+ 注意每张图片是如何依次显示的？这就叫做__相对__定位。如果你想告诉浏览器放置机器人眼睛的准确位置，你将需要使用__绝对__定位。

向 `eyes1` 图片的 CSS 添加以下 3 行代码：

```
position: absolute;
top: 200px;
left: 100px;
```

你应该看到机器人的眼睛向机器人的正确部位移动。

![screenshot](images/robot-eyes-position.png)

此 CSS 代码告诉浏览器图片显示在距网页的顶部／左侧多远的地方。

![screenshot](images/robot-eyes-position2.png)

你可以使用 `bottom` ​而非 `top` 来告诉浏览器将图片显示在距画面底部多远的地方，以及使用 `right` 而非 `left`。

