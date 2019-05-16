# Nginx 屏蔽垃圾網頁蜘蛛配置文件



服務器資源有限，受不了垃圾蜘蛛一天到晚的爬取，爬取也就算了，還拿去當做自己盈利點，果斷屏蔽！

本配置文件適合 nginx，apache 可以自己對照著修改，機器人不斷更新中，大家可以根據自己的需要添加或刪除。


用法：

① 下載配置文件，放到適當的位置，比如：


cd /usr/local/nginx/conf/vhost/ && wget https://raw.githubusercontent.com/vircloud/bots/master/deny-bots.conf



② 修改站點配置文件，在適當的位置引入配置，比如：


server


{


  ......
  
   
    include deny-bots.conf;
    
    
  ......
  
  
}



③ 重啟 nginx 服務：


service nginx reload


444 狀態碼說明：直接由服務器中斷連接，不會向客戶端再返回任何消息，此為 nginx 獨有。


更多方法参见：[网站如何屏蔽垃圾蜘蛛爬取？](https://vircloud.net/operations/site-deny-bot.html)


