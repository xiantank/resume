# Resume
## 關於我
* 以Node.js 搭配MongoDB開發為主的後端工程師
* 聯絡信箱: xiantank@gmail.com

## 技能
* Node.js, C, Golang
* MongoDB, MySQL, Redis
* Git, Docker, Shell Script, JWT, OAuth2, RESTful API, AWS

## 經歷

**利頡資訊，軟體工程師 — 2018/03-2019/12**
1. 參與客服系統建置: 後台管理系統使用Express.js及mongoose、客服及使用者端聊天室使用 Socket.io, 負責第三方使用者資料導入、檔案上傳(aws s3), 客服及管理者端登入系統, 及其他API撰寫
2. 網頁版群組聊天室建置: 包含聊天室、黑名單禁言、關鍵字遮蔽、未讀數量通知
3. 協助改善部署: 透過Jenkins執行shell script, 進行下載倚賴, 前端檔案bundle及執行測試, 靜態檔案及artifact上傳至s3, 於部署時選擇所需的版本部署到server(aws ec2)上
4. 參與code review
5. 與PM討論功能並分派工作給底下新人, 並指導他們如期完成工作
6. 積極參與讀書會的分享, 曾分享過es6, clean code, session/JWT/Oauth2, RESTful API, 資料庫索引, docker/docker compose基礎操作

**台雲資訊，軟體工程師(兼職) — 2016/01-2016/11**
開發Chrome extension並以Node.js為後端

## 學歷
**國立中正大學**
資訊工程系 - 碩士  2014/09 ~ 2016/08
資訊工程系 - 學士  2010/09 ~ 2014/07

## 作品

### [訂閱通知](https://github.com/xiantank/node-watcher)
管理爬蟲並通知的系統, 提供使用者設定爬取網頁並設定比對條件, 比對成功就送出通知。

管理者可對使用者進行CRUD操作, 一般使用者可對爬蟲(網址加選擇器)進行新增、讀取、刪除、修改爬取時間, 並設定im通知。

實作上分web, cronjob, crawler, notification 四個運行。

使用者可透過RESTful API進行設定並存入MySQL server, 使用者登入機制採用session, 可透過環境變數決定本地或redis存取。

cronjob定時拉取需要進行的爬取動作, 並透過Message Queue進行抓取任務派送。

crawler訂閱message queue執行抓取網頁並透過css selector去比對, 符合比對條件時透過Message Queue進行通知任務派送。

notification訂閱message queue並將結果透過指定好的通知方式進行通知(目前僅實做telegram通知)



### [美食地圖](https://github.com/xiantank/food-map)

使用Node.js (Express.js)作為後端，並以MongoDB作為資料庫(使用Mongoose作為ODM)，串接Line login作為登入，以imgur API作為圖片儲存空間

提供使用者可以在
1. 網頁中搜尋並新增收藏地點、評論
2. 透過Line chat bot搜尋餐廳，並新增評論及相片

### [書籤快截](https://github.com/xiantank/bookmarksBackup)

使用Chrome extension api 搭配Google drive api
能將使用者所有的bookmarks備份成mhtml格式
並依照書籤結構存入Google drive中

### [csie.io DDNS](https://github.com/xiantank/csieioDDNS)
(csie.io only)
* Chrome app
* 為csie.io的DDNS服務寫的DDNS
* 定時確認IP，有變動就更新


