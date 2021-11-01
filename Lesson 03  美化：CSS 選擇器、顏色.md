<h2 align="center">Lesson 03: 美化：CSS 選擇器、顏色</h2>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 06</title>
</head>

<!--套用於整個區塊-->
<body style="background-color: blue">
    <!--包覆於 style="值" 之內，內部則以冒號、分號為格式-->
    <p style="font-size: 40px; color: yellow">我是段落 1</p>
    
    <!--font-family 定義字形，仍可定義區塊背景色-->
    <h2 style="background-color: #FF0000">我是標題 2</h2>　
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 07</title>
    <style>
        /* 於 style 定義: 內部樣式表 */
        p {font-family: 標楷體; color: purple}
        h2 {background-color: pink; text-align: center}
    </style>
</head>

<!--直接定義：內聯樣式，亦可以 rgb(0, 0, 255) 表之-->
<body style="background-color: #0000FF">　
    <p>我是段落 1</p>
    <h2>我是標題 2</h2>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 08</title>
    <style>
        body {background-color: rgb(192, 192, 192)}
        /* 類別選擇器: 不具唯一性 */
        .style {font-size: 15px; text-align: center}
        /* 類別選擇器可加上標籤額外指定 */
        p.style {color: green}
        
        /* ID 選擇器: 具有唯一性 */
        #another {background-color: green}
    </style>
</head>

<body>
    <!--受到 body, .style 和 p.style 影響-->
    <p class="style">我是段落 1</p>
    
    <!--受到 body, .style 影響-->
    <h1 class="style">我是標題 1</h1>
    
    <!--定義條件衝突時，以後者為準-->
    <h2 id="another">我是標題 2</h2>
</body>
</html>
```
