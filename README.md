# 将本地代码上传到github
git命令行以及仓库的使用
## 创建SSH KEY
先看下C盘的user文件下有没有.ssh目录，如果没有，就输入命令进行创建：
<pre>
$ ssh-keygen -t rsa -C "youremail@example.com"
</pre>
![image](https://github.com/Sumahan/learning-git/blob/master/ssh.jpg)

在user目录下找到id_rsa.pub,复制里边的内容：

![image](https://github.com/Sumahan/learning-git/blob/master/key.jpg)

打开github，进入setting页面，找到ssh：

![image](https://github.com/Sumahan/learning-git/blob/master/add_key.jpg)
最后点击add key

## 将本地项目和github的仓库进行关联
1.首先用git init命令把要上传的文件夹变成git可管理的仓库
2.git add .  将该目录下的所有文件夹都添加到仓库
3.git status   查看要添加的文件
4.git commit -m  把项目提交到仓库
5.在github上新建一个仓库
6.创建好之后，复制仓库地址，在git中输入
<pre>
$ git remote add origin git@github.com:Sumahan/base-vue.git
</pre>
这样就把本地代码和github仓库关联好了
7.将代码push到仓库
<pre>
$ git push origin master
</pre>

以上步骤就完成了本地项目添加到github仓库的过程。

