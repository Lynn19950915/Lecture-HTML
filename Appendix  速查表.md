<h2 align="center">Appendix: 速查表</h2>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>1. CSS 與元素層級</title>
    <style type="text/css">
        h4 {color: blue}
    </style>
</head>

<body>
    <h4>區塊層級</h4>
    <p>div, p, h2 ...</p><hr>
    <h4>內聯層級</h4>
    <p>img, a, span ...</p>
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>2. 列表與表格</title>
</head>

<body>
    <ul>無序列表
        <li>1st</li>
        <li>2nd</li>
    </ul>
    <ol>有序列表
        <li>3rd</li>
        <li>4th</li>
    </ol>

    <table border=1>
        <tr>
            <th>表頭1</th>
            <th>表頭2</th>
        </tr>
        <tr>
            <td>內容1</td>
            <td>內容2</td>
        </tr>
    </table>
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>3. 表單</title>
</head>

<body>
    <form>
        username: <input type="text" size=20 maxlength=10><br>
        password: <input type="password" maxlength=8><br>
        多選題: <input type="checkbox" checked="checked"><br>
        單選題: <input type="radio" checked="checked"><hr>
        <select>
            <option selected>A</option>
            <option>B</option>
        </select><br>
        <textarea cols=40></textarea><hr>

        <input type="submit" value="送出">
        <input type="reset" value="清除">
    </form>
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>4. 鏈接總複習</title>
</head>

<body>
    <a href="aaa">文字超連結</a><br>
    <a href="bbb"><img src="xxx" height=40 width=40></a><hr>

    <a href="#ccc">查找文檔中 id=ccc 之部分</a>
    <h3 id="ccc">這段不是超連結</h3>
    <a href="mailto: ddd">傳送電子郵件</a>
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>5. 文本格式化</title>
</head>

<body>
    <b><i>粗體+斜體之文字</i></b>
    <pre><bdo dir="rtl">依照格式輸
    出</bdo></pre>
    <sub><small>下標+縮小</small></sub>或
    <sup><big>上標+放<del>小</del>大</big></sup>
</body>
</html>
```
