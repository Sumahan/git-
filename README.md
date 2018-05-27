# 将本地代码上传到github
git命令行以及仓库的使用
## 创建SSH KEY
先看下C盘的user文件下有没有.ssh目录，如果没有，就输入命令进行创建：
<pre>
$ ssh-keygen -t rsa -C "youremail@example.com"
</pre>
![image](https://github.com/Sumahan/learning-git/blob/master/%E5%88%9B%E5%BB%BASSH-KEY.jpg)
在user目录下找到id_rsa.pub,复制里边的内容：
![image](https://github.com/Sumahan/learning-git/blob/master/key.jpg)

