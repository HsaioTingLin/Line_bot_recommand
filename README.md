# Line_bot_recommand
根據不同event事件刻出來的食譜推薦機器人
# recommand_linebot
準備環境  
1.下載 git: `https://git-scm.com/`    
2.下載 ngrok `https://ngrok.com/download`    
3.Line Developes    
`https://developers.line.biz/console/channel/1654940932/messaging-api`  
建立好 providers 參考: TOP/tutorial/eb103-test/Messaging API  
`在 messaging-api 下/ 回應設定 /加入好友的歡迎訊息、自動回應訊息[停用]/ Webhook [啟用]`  

* step 1
在 line bot 資料夾下開啟 cmd
1. 參考 github
`git clone https://github.com/BingHongLi/line_chat_bot_tutorial.git`  

2. 登入 jupyter notebook
----

* Step 2 開啟第二個 cmd
在 line bot 資料夾下 cmd
ngrok http 5000 -region ap
要複製加密網址到 Webhook URL (確認連線有無成功)  
`https://5c6210c60747.ap.ngrok.io -> http://localhost:5000`

Step 3 jupyter notebook 操作
參考 github: line_chat_bot_tutorial/material/line_secret_key:
```js
{
  "channel_access_token":"your channel_access_token ",
  "secret_key":"secret_key",
  "self_user_id":"self_user_id",
  "rich_menu_id":"放入生成自定義菜單的id",  #放入richmenu
  "server_url":"Forwarding"   
}
```
