<h2 align="center">Lesson 04: 架構：區塊、標題段落、布局</h2>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 09</title>
</head>

<body>
    <h2>我是標題 2</h2>
    <!--x 號標題對應到 (7-x) 號字體-->
    <font size="5">我是 5 號字體</font>
    <!--觀察兩條 hr，標題會自帶行距而文字不會-->
    <hr/>
    <h5>我是標題 5</h5>
    <hr/>

    <!--標題會自動換行，文字不會-->
    <font size="2">我是 2 號字體</font>
    <br>
    <!--size 為一種標籤屬性，其他格式則須寫入 style-->
    <font style="font-family: 標楷體">我是 2 號字體</font>
    <br>　
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 10</title>
    <style>
        /* .two 不受到影響 */
        .one {background-color: rgb(100, 255, 0)}　
    </style>
</head>

<body>
    <!--div 為一個大區塊，可協助統一格式-->
    <div class="one">
        <!--div, h3, p 都是塊狀層級，自帶行距-->
        <h3>我是標題 3</h3>
        <p>我是段落 1</p>
    </div>
    
    <div class="two">
        <p>我是段落 2</p>
    </div>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 11</title>
    <style>
        /* 標籤選擇器 */
        span {font-size: 40px}
    </style>
</head>

<body>
    <h3>我是標題 3</h3>
    
    <!--運用 br 可於段落內自動換行，與 span 均為內聯層級-->
    <p>我是段落 1
        <br>我是第二行
    </p>
    <!--運用 span 可於段落內不換行定義格式-->
    <p>我是段落 2
        <span>我還是第一行</span>
    </p>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 12</title>
</head>

<body>
    <!--以一個大區塊包含其他 div，可定義範圍-->
    <div style="width: 600px">
        <div style="background-color: rgb(0, 0, 255)">
        <!--h2 自帶行距但背景色只套用文字，需設定 margin-bottom-->
        <h2 style="text-align: center; margin-bottom: 0px">這是一個主標題</h2></div>　

        <div style="background-color: rgb(0, 255, 0); height: 300px; width: 160px; float: left">
            <p>功能選單按鈕</p>
            <!--段落彼此亦帶行距，其內則用 br 分行-->
            <p>功能 1
                <br>功能 2
                <br>功能 3
            </p>
        </div>　
        <!--float 設定對齊浮標向左，防止區塊未填滿便自動換行-->
        <div style="background-color: yellow; height: 300px; width: 440px; float: left">
            <font size="6">主頁內容</font>
        </div>

        <div style="background-color: #000000; color: white; text-align: center">
            <!--亦可改為font style="text-align: center"-->
            版權所有，翻印必究
        </div>
    </div>
</body>
</html>
```
