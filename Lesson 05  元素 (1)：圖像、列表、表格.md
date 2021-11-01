<h2 align="center">Lesson 05: 元素 (1)：圖像、列表、表格</h2>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 13</title>
</head>

<body>
    <!--內聯層級不自動換行，需定義 br 或下個段落-->
    <img src="xxx">　

    <!--align 預設 bottom，垂直對齊會換行-->
    <p><img src="xxx" width="180" height="120" align="top">apple</p>
    <!--設定漂移位置 (文字仍為靠左)：等同 align="right" 水平對齊-->
    <p><img src="xxx" width="180" height="120" style="float: right">apple</p>

    <!--在圖片設定超連結 yyy 網址；img, a 均無結束標籤-->
    <p><a href="yyy"><img src="xxx"></p>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 14</title>
</head>

<body>
    <h3>這是兩個無序列表</h3>
    <ul>
        <li>我是第一項</li>
        <li>我是第二項</li>
    </ul>
    <!--預設為 disc，circle 為非實心圓-->
    <ul style="list-style-type: square">
        <li>我是第三項</li>
        <li>我是第四項</li>
    </ul>　

    <h3>這是兩個有序列表</h3>
    <!--標籤改用 ol-->
    <ol>
        <li>我是第五項</li>
        <li>我是第六項</li>
    </ol>
    <!--type: A/a, I/i，以 start="數字" 指定起始項標序-->
    <ol type=I start=7>
        <li>我是第七項</li>
        <li>我是第八項</li>
    </ol>　

    <h3>這是一個巢狀列表</h3>
    <ul>
        <li>我是第九項
            <!--巢狀包覆第一項內，需加寫 ul 標籤；預設為非實心圓-->
            <ul>
                <li>我是第一小項</li>
                <li>我是第二小項</li>
            </ul>
        </li>　
        <li>我是第十項</li>
    </ul>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 15</title>
</head>

<body>
    <!--預設 border=0 (無表格邊框)-->
    <table border=1>
    <!--可統一設定表頭、表身格式，於此例可略-->
    <thead>　
        <tr>
            <!--表頭欄位為 th 標籤，自動設定粗體置中-->
            <th>x<0</th>
            <th>x>0</th>
        </tr>
    </thead>
    
    <tbody>
        <tr>
            <td>我是第二象限 (-,+)</td>
            <td>我是第一象限 (+,+)</td>
        </tr>
        <tr>
            <td>我是第三象限 (-,-)</td>
            <td>我是第四象限 (+,-)</td>
        </tr>
    </tbody>
    </table>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 16</title>
</head>

<body>
    <!--單元格邊距對內 (文字)；單元格間距對外 (表格)-->
    <table border=1 cellpadding=15 cellspacing=5>
        <!--無法對齊，可用 caption (預設置中) style="margin-bottom" 取代-->
        <h3>垂直表頭寫法</h3>　
        <tr>
            <th>y>0</th>
            <td>我是第二象限 (-,+)</td>
            <td>我是第一象限 (+,+)</td>
        </tr>
        <tr>
            <th>y<0</th>
            <td>我是第三象限 (-,-)</td>
            <td>我是第四象限 (+,-)</td>
        </tr>
    </table>
</body>
</html>
```
<br/>

```html
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 17</title>
</head>

<body>
    <!--定義：所有元素置中對齊-->
    <table border=1 cellpadding=8 style="text-align: center">　
        <tr>
            <th/>
            <th colspan=2>x 軸</th>
        </tr>
        <tr>
            <th rowspan=2>y 軸</th>
            <td> II </td>
            <td> I </td>
        </tr>
        <tr>
            <!--首欄為 rowspan 範圍，直接輸入另兩欄即可-->
            <td> III </td>
            <td> IV </td>
        </tr>　
    </table>
</body>
</html>
```
