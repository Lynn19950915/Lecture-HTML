<h2 align="center">Lesson 06: 元素 (2)：表單、鏈接</h2>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 18</title>
</head>

<body>
    <!--本身並非元素，但可定義整張表單範圍-->
    <form>
        <!--input 標籤為內聯層級-->
        Studentid: <input type="text"><br>
        <!--size 定義框格長度，與輸入上限無關-->
        Password: <input type="password" size=10><br>

        <!--可利用段落進行區塊分隔-->
        <p>單選題：
            <br><input type="radio">A <input type="radio">B <input type="radio">C<br>
        </p>
        <p>多選題：
            <br><input type="checkbox">A <input type="checkbox">B <input type="checkbox">C<br>
        </p>

        <!--按鈕上顯示提交、清除，執行 submit, reset 之功能-->
        <p>
            <input type="submit" value="提交">
            <input type="reset" value="清除">
        </p>
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
    <title>Sample 19</title>
</head>

<body>
    <!--fieldset 類似樣式版框，以 legend 定義標題-->
    <fieldset>
        <legend>回饋單</legend>

        <h4>最喜歡的曲目、原因</h4>
        <select>
            <!--option 為下拉選單，以 optgroup 為選單子分類-->
            <optgroup label="上半場">
                <!--selected 定義於 option 中，表示預設選項-->
                <option selected>Song A1</option>
                <option>Song A2</option>
            </optgroup>　
            <optgroup label="下半場">
                <option>Song B1</option>
                <option>Song B2</option>
            </optgroup>
        </select>
        <!--以段落適度分隔，設定輸入文框 textarea-->
        <p><textarea cols=50></textarea></p>

        <h4>總體評價</h4>
        <!--parseInt 轉換 value 為數字，若要輸出需定義 I/O 物件名稱 (id, name 均可)-->
        <form oninput="o.value=parseInt(i.value)">
            <!--range 表示可拉選軸，可定義 min, max 範圍 (與標籤外數字無關)-->
            0<input type="range" name="i">100
            <output name="o"></output>
        </form>
    </fieldset>	
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 20</title>
</head>

<body>
    <a href="aaa">點擊這行進入連結</a><br>
    <!--點擊這張圖進入連結，可設定 border, width, height-->
    <a href="bbb"><img src="xxx"></a><br>
    <!--可於新分頁開啟 (同預設)-->
    <a href="ccc" target="_blank">點擊這行進入連結</a><br>

    <!--由此分頁尋找匹配 id，不限於 <a> 標籤-->
    <a href="#ddd">點擊這行查找資料</a><br>
    <!--被查找的目標：href="此網頁#ddd"-->
    <h2 id="ddd">被查找的內容</h2>
</body>
</html>
```
<br/>

```
<!DOCTYPE html>
<html>
<head>
    <meta content="text/html; charset=utf-8">
    <title>Sample 21</title>
</head>

<body>
    <!--cc 表示副本、bcc是密件副本；subject 及 body 則為標題及內容。內容包含空白則使用 %20 取代-->
    <a href="mailto: aaa.com?cc=bbb.com&bcc=ccc.com&subject=ddd&body=eee">發送郵件</a>

    <!--post 為訪問頁面之方式，帶參數-->
    <form action="mailto: aaa.com" method="post" enctype="text/plain">
        StudentID: <br>
        <!--內文以 name=value 格式傳送輸入內容，value 預設空白而 name 屬性需載明-->
        <input type="text" name="ID"><br>　
        Comment: <br>
        <input type="text" name="comment"><br>
        
        <!--button 文字定義於標籤中內容，submit 鈕則設定於 value 屬性-->
        <input type="submit" value="提交">
    </form>
</body>
</html>
```
