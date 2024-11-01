# StarUML
# 南華大學-軟體工程 期中報告
<h3>11124101 林宥慈 11124102 林宥君<h3>
<h1>軟體工程 : 實驗四、UML動態建模之順序圖分析與設計</h1>

<h2>
一、實驗題目：UML動態建模之順序圖分析與設計

二、實驗目的：通過'網路教學系統'UML建模過程掌握順序圖的分析與設計方法。

三、實驗任務

網路教學系統」的功能需求主要包括以下幾個面向：
• 學生可以登入網站瀏覽資訊、尋找資訊和下載文件。
• 教師可以登入網站輸入課程簡介、上傳課件檔案、發布訊息、修改和更新訊息。
• 系統管理員可以對頁面維護以及批准使用者的註冊申請。

四、實驗步驟

分析實驗任務內容，完成各功能順序圖分析，並利用UML完成順序圖的建模，主要包括實驗二得到的各個用例擴展而成的功能順序圖。

五、實驗過程
</h2>
1.對於學生對象

![螢幕擷取畫面1](https://github.com/user-attachments/assets/0dedf2a3-8527-4800-952a-61d96da0607a)


分析：學生先要登入網站，輸入正確的資訊驗證成功，才能web介面，例如他要瀏覽訊息，先請求web取得訊息，web接著發送訊息給system，system再發送訊息給database，database根據指令找到對應的訊息，逐步回傳訊息，最後回傳給學生。

2.對於教師對象

![螢幕擷取畫面2](https://github.com/user-attachments/assets/a5b709c7-b338-4aa0-858f-66fb01d45cb5)


分析：教師要先登入網站，等待驗證成功之後，進入web介面，然後發布訊息給web，web再傳到system，system儲存到database,成功之後，database返回保存成功訊息給system，system返回上傳成功訊息 給web，web再回發布訊息成功給教師。

3.對於系統管理人員
![螢幕擷取畫面 3](https://github.com/user-attachments/assets/6198f35b-dae9-458c-b483-fdb2f58364b0)

分析：系統管理員，直接從後台登陸系統，等待身份驗證成功之後，他可以對資料庫修改和維護，修改成功之後，資料庫給系統返回更新成功訊息，系統給管理員返回修改成功訊息。

六、參考資料

https://blog.csdn.net/guleilei0/article/details/124869573?spm=1001.2014.3001.5502
