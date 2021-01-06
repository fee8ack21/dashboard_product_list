# Dashboard Product List
---
* 語言：PHP
* 資料庫：MySQL
* 連線方式：mysqli
* 筆數、分頁選擇：表單傳送到目前頁，PHP 設定是否 $_GET 的狀況 
* 新增：表單傳送到另一隻負責處理的檔案，把 $_POST 的資訊抓下來後 INSERT INTO 到資料表
* 查詢：表單傳送到目前頁，利用SELECT * FROM … WHERE … AND … LIKE $_GET的東西達到效果
* 修改：表單傳送到另一隻負責處理的檔案，利用 SELECT * FROM ... WHERE ... 的方式抓到該商品資訊，再把 $_POST 的資訊 UPDATE 上去
* 刪除：表單傳送到另一隻負責處理的檔案，不會真的把商品資訊刪掉，僅變更某欄位資訊，使其不符合 SELECT 條件
