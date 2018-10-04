# Assignment #1 0920
如果你會寫第一題或第二題的話，那你就把這題用ipynb所另存成的.html檔給交上來就好。就不用做第三題。如果你第一、二題都做不出來的話，那就請完成第三題的練習。
1. 請把下列表格中的資料用dicationary與list表示後，指給（Assign）給一個變數。

id|area|district|price
---|---|---|---
a13248|18.5|信義區|17890000
a13249|21.3|信義區|20000000
a13250|32.1|信義區|36820000

2. 請用for-loop產生費氏數列的前50項並進行加總。

3. 請上Datacamp完成[Intro to Python for Data Science](https://www.datacamp.com/courses/intro-to-python-for-data-science)的練習。並用螢幕截圖擷取完成該單元的畫面（會獲得一個簡單的證書）成為.png或.jpg檔，上傳該圖檔即可。

# Assignment #2 0927
1. 自政府開放資料下載一個json檔，分別將其轉為層套的list或dictionary。針對該資料集：
    1. 說明你下載了哪個資料集的檔案，列出該資料集的名稱與超鏈結。
    2. 用程式列印出，該資料集包含幾筆資料。
    3. 用程式列印出，該資料集的主要資料表有哪些「變項」。這邊所指的「變項」為統計的「變項」。例如ubike的資料就有中文站名、英文站名等等。列印出的形式不拘。
    4. 嘗試用上週與本週所教的「計數counting」運算，統計其中一個變數。
2. 讀取json檔案的方法
```
with open("data/your_file.json", "r", encoding="UTF-8") as f:
    jdata = json.load(f)
print(type(jdata))
```
# Assignment #3 1004
1. 自政府開放資料下載一個CSV檔，分別將其轉為二層的list。針對該資料集：
    1. 說明你下載了哪個資料集的檔案，列出該資料集的名稱與超鏈結。
    2. 用程式列印出，該資料集包含幾筆資料、變項的數量有幾個？
    3. 用程式列印出，該資料集的主要資料表有哪些「變項」。這邊所指的「變項」為統計的「變項」。
    4. 嘗試用上週與本週所教的「計數counting」運算，加總或者計算其中一個變數的出現次數。（你可能需要自己記住你要抓的變項index）。假設我已經把資料轉為a list of list，並指給一個變數`all_list`，那我的程式碼可能會長的像這樣：
```
for row in all_list:
    if row[3] not in temp_dict:
        temp_dict[row[3]]  = 1
    else:
        temp_dict[row[3]] += 1
```
2. (option)將ubike data讀取後，轉為兩層的list所表示的格式，第0個list為欄位名稱。
3. (option)上網查詢要如何將這兩個list存為`.csv`檔。
