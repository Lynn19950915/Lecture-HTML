<h2 align="center">Lesson 07: 其他功能 (文本格式化、腳本)</h2>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 22</title>
</head>

<body>
    <!--p 相對 div 具行距特色-->
    <p><i>這是一行<del>粗</del>斜體字</i></p>　
    <p><b>這是一行粗體字，可設定<sub>下標</sub>與<sup>上標</sup></b></p>
    <p><u>這是一行底線字，可以<big>放大</big>也能<small>縮小</small></u></p>
    
    <!--顛倒輸出以 bdo 定義，rtl 表由右至左-->
    <p><bdo dir="rtl">反過來</bdo></p>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 23</title>
</head>

<body>
    <pre>
    <!--q 形同加上引號之位置-->
    老師說: <q>有了 pre，空行就能遵照格式打印</q>　
    <!--未設定時會忽略空行，使跨行文字相黏-->
    像這樣。
    </pre>　
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 24</title>
</head>

<body>
    <script>
        <!--不支援標題、換行 pre，為 javascript 語言-->
        document.write("可寫入一段話<p>或段落</p>")
    </script>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 25</title>
</head>

<body>
    <p id="click">可寫入一段事件腳本</p>

    <!--事件觸發是作用在 function，可全寫在同一腳本-->
    <script>
        <!--針對 id=click 元素調整樣式-->
        function event1(){
            document.getElementById("click").style.color="#ff0000"
        }
        <!--針對 id=click 元素輸出 HTML (內容)-->
        function event2(){
            document.getElementById("click").innerHTML=("Magic")
        }
    </script>

    <!--不同於 input 按鈕，button 功能視事件自定義-->　
    <button type="button" onclick="event1()">幫我修改顏色</button>　
    <button type="button" onclick="event2()">幫我換一句話</button>
</body>
</html>
```
