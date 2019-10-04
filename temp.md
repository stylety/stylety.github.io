### Temp TEXT here
***
复制一下代码到记事本中并另保存为autoTelnet.bat，之后双击运行就实现自动登录到telnet服务器了，服务器IP自己修改

```
@echo off
echo set sh=WScript.CreateObject("WScript.Shell") >telnet_tmp.vbs
echo sh.SendKeys "open 192.168.210.91" >>telnet_tmp.vbs
echo WScript.Sleep 1000 >>telnet_tmp.vbs
echo sh.SendKeys "{ENTER}" >>telnet_tmp.vbs
echo WScript.Sleep 10000 >>telnet_tmp.vbs
echo sh.SendKeys "y{ENTER}" >>telnet_tmp.vbs
echo WScript.Sleep 5000 >>telnet_tmp.vbs
echo sh.SendKeys "administrator{ENTER}">>telnet_tmp.vbs
echo WScript.Sleep 3000 >>telnet_tmp.vbs
echo sh.SendKeys "password{ENTER}">>telnet_tmp.vbs
echo WScript.Sleep 3000 >>telnet_tmp.vbs
start telnet
cscript //nologo telnet_tmp.vbs
del telnet_tmp.vbs
``` 
***
#### 无版权图片下载
[https://pixabay.com/zh](https://pixabay.com/zh)
<br>
[https://www.freeimages.com/](https://www.freeimages.com/)
<br>
[https://www.ssyer.com/](https://www.ssyer.com/)
<br>
***
### [Github中能用的表情符号](https://www.webfx.com/tools/emoji-cheat-sheet/)
>例如： :coffee: :pizza:
:smile:
