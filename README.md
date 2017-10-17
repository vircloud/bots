# bots
Nginx 屏蔽垃圾網頁蜘蛛配置文件



服務器資源有限，受不了垃圾蜘蛛一天到晚的爬取，爬取也就算了，還拿去當做自己盈利點，果斷屏蔽！



本配置文件適合 nginx，apache 可以自己對照著修改，機器人不斷更新中，大家可以根據自己的需要添加或刪除。



用法：



① 下載配置文件，放到適當的位置，比如：




cd /usr/local/nginx/conf/vhost/ && wget https://





② 修改站點配置文件，在適當的位置引入配置，比如：



server


{



  ......
  
  
  
    include access-lese.conf;
    
    
    
  ......
  
  
  
}



③ 重啟 nginx 服務：




service nginx reload

