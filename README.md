# 使用prosess Monotor 观察 程序的文件操作
### 第一步
![first](/img/1..PNG)
1. 虚拟机中打开process monitor.

2. 运行cmd，输入如图所示的代码，tab键可以补全，输入dir检查是否成功。

 ![code](/img/2.PNG)

3. 再在cmd中输入homework.exe 运行程序。

### 第二步

1. 打开process monitor，打开filter
![filer](/img/4.jpg)

2. 添加几个过滤器选项
* process name is homework.exe include (监测它的活动)
* path begins with C:\Windows Exclude（排除它访问系统文件的活动）
* result is success include（排除失败的那些结果）

* 在软件界面中只选择 show me file system activity 
![h](/img/6.PNG)
* 继续设置过滤器    path  contains homework exclude（排除它访问自身文件的活动）
* path contains C:\Users\vegetable\AppData exclude（根据显示情况继续排除）
  
 最后肉眼就会得到如下结果
![h](img/7.PNG)
3. 点开在沿着路径找到他就可以看到jpg文件的目录了
   

##### 其实还有一种更为简便的过滤方法
* 直接设置过滤器：
* process name homework include
* path ends with jpg include 
 ![h](img/8.PNG)
 
就可直接看到结果了
![h](img/1573912210607.jpg)




