# Z-Godzilla_ekp
### 哥斯拉webshell二次开发规避流量检测设备  
如果工具帮到了你，顺手点个 ⭐ 就是对项目最大的支持，感谢各位师傅！

二开详细教程在微信公众号：艾克sec  
截止2024.4.10 测了国内两安全厂商的态感，连接和执行命令无告警，目前效果未知  
最新版本增加了内存马注入，三种语言自定义免杀加密器，流量高度模拟混淆等功能，但目前由于特殊原因不能公开，推荐师傅们看公众号文章自行二开。  
#### 1.2更新
最近df将哥斯拉dll的特征加到amsi里了，很多师傅提到shell在却连接不上，更新一个版本，可绕过amsi正常连接  
建议配合命令执行bypass插件食用 ，不然执行命令会被检测w3wp进程然后查到文件给查杀  
https://github.com/ekkoo-z/Gsl_ekp_bypassPlugin  
<img width="2998" height="1324" alt="image" src="https://github.com/user-attachments/assets/5e47af92-2fe3-4b68-bcea-e1aff2f60d5a" />  
注：server2022版本及以上自带的所有插件都用不了 不是bug而是df杀软的问题  
由于自己已经不用哥斯拉了，这个问题懒的解决了，后续会开源一个新的webshell管理工具来解决这些问题  

#### 1.1更新
更新一下net的生成即免杀以及随机html
使用方法：  
生成webshell选择bypass1   
<img width="640" alt="图片" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/87b86418-ad9f-49f7-bc4c-00e8634654c4">  
即可免杀(vt 微步 阿里云 河马等均0报红)   
<img width="1444" alt="图片" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/6d4780ba-c322-4bd9-b303-f489e2441f17">  
<img width="697" alt="图片" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/e56e264d-a23c-4953-bcb4-123f54114bf8">
<img width="697" alt="图片" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/a732cd0e-f2b8-4973-9899-cd3ca1d49ac6"> 
<img width="705" alt="图片" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/1ac7d306-1da7-4d4b-ac44-3fc2f23c5ed8">  
<img width="1294" alt="图片" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/557f1c5f-f8f6-43eb-87ff-8ff174a54d35">  



#### 流量修改效果  
1.去除cookie后分号强特征  
2.去除响应包中md5前后16位匹配强特征  
3.去除ua头等等弱特征  
4.修改请求包和响应包伪装成正常流量  
phpxorbase64流量修改前  
<img width="948" alt="image" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/5b38b145-5bfd-4c17-a7fc-f48cc7de58d8">  
修改后  
<img width="634" alt="image" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/fa5e98ee-1989-4566-a2b9-4a623cb55305">   

#### 使用方法：  
直接生成webshell再用网上的工具或者自己的免杀方法进行免杀（后续可能会提供一键免杀的功能）  
<img width="539" alt="image" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/89f98872-ff73-482b-8f2f-efa7a08d95f0">  
连接时也选择对应的模式  
<img width="534" alt="image" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/1e4b9104-524f-4fde-9916-374f6e947f06">  
命令执行一切正常  
<img width="643" alt="image" src="https://github.com/kong030813/Z-Godzilla_ekp/assets/97926809/3f76318e-2e03-496f-bfbf-112080d47d11">  

注：使用二开版本生成的webshell，用普通版本的哥斯拉是连不上的（选项中需要选择二开版本模式进行连接）

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=ekkoo-z/Z-Godzilla_ekp&type=Date)](https://www.star-history.com/#ekkoo-z/Z-Godzilla_ekp&Date&Date)









