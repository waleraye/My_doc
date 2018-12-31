## win7系统封装静默激活



使用windows loader工具进行激活

静默激活参数：

`/silent /norestart`



使用封装工具调用windows loader添加静默激活参数进入桌面激活之后文件删不掉，发现使用bat命令可以实现

bat命令为：      



```batch

start /wait WindowsLoader/WindowsLoader.exe /silent /norestart        
// 运行WindowsLoader文件夹下的WindowsLoader.exe程序  

 
rd /s /q WindowsLoader                
// 删除WindowsLoader文件夹及文件夹下的所有文件


del %0                                              
// 删除bat文件自身


```



*新建文本文档然后复制粘贴修改后缀明 为“bat”*



可以手动双击bat文件进行激活也可以在封装工具中进行调用激活，激活过程中没有图形界面，完全隐藏的，适用于windows7旗舰版。



[激活程序文件下载](https://github.com/WalerGit/my_doc/releases/download/%E6%BF%80%E6%B4%BB%E5%B7%A5%E5%85%B7/win7.zip)