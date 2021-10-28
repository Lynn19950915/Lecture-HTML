<h2 align="center">Lesson 01: HTML 101 (簡介、元素、屬性)</h2>

```
<!--聲明為 HTML 文檔-->
<!DOCTYPE html>
<html>
<head>
    <!--使用中文編碼-->
    <meta content="text/html; charset=utf-8">
    <title>Sample 01</title>
</head>

<body>
    Hello world!
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <!--文檔標題會顯示在網頁的分列-->
    <title>Sample 02</title>　
</head>

<body>
    <!--開頭與閉合標籤通常成對出現-->
    <h1>我是標題 1</h1>　
    <h3>我是標題 3</h3>
    <h5>我是標題 5</h5>
    
    <!--段落字體大小落在標題3, 4之間-->
    <p>這是一個段落</p>　
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 03</title>
</head>

<!--body標籤內包含許多標籤：巢狀-->
<body>
    <!--文字內容為<p>所包覆，整組內容又為<body>包覆-->
    <p>我是段落 1</p>
    <!--開頭標籤可夾帶屬性資訊-->
    <p style="font-size: 20px">我是段落 2</p>　
    <hr>
    <a href="https://www.facebook.com">我是一個臉書超連結</a>
</body>
</html>
```
