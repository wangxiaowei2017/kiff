# 什么是git？
* GIT 是一个分布式版本控制软件，最初由林纳斯·托瓦兹（Linus Torvalds）创作，于2005年以GPL发布。最初目的是为更好地管理Linux内核开发而设计。是目前世界上最先进的分布式版本控制系统.
# git安装
## ubuntu linux安装方法
```sh
$ sudo apt-get install git
```
##   mac ox安装方法
```sh
$ brew install git
```
# 创建git本地仓库
```sh
$ mkdir git
$ cd git
$ mkdir c
$ cd c
$ git init
```
# 增加文件
1.复制已有的文件到当前目录里：
```sh
$ cp ../../c/*.c .
```
2.创建一个新的文件。
```sh
$ touch hello.c
$ vim hello.c   //输出hello world字符串的C语言的程序（代码）
```
# 查看目录状态
查看当前目录下的文件在git仓库中的状态。
```sh
1.$ git status
```
# 跟踪文件
将当前目录下的所有文件， 进行跟踪。
```sh
1.$ git add .
```
# 配置个人用户信息
为提交增加个人用户信息。
```sh
1.$ git config --global user.name "wangxiaowei2017"
2.$ git config --global user.email "wang.xiao.wei@outlook.com"
3.$ git config --global core.editor vim
```
# 提交
向本地git仓库提交， 跟踪文件。
```sh
1.$ git commit
2.First commit
3.Init commit
```
# 查看提交信息
查看提交相关信息。
```sh
1.$ git log
第一行： commit ID
第二行： 提交作者名字和email.
第三行： 提交的时间
第四行： 提交信息标题
第五行： 提交信息具体内容
```
# git diff
1.查看修改源码。
```sh
1.$ git diff
```
   2.两个提交版本之间做比较
```sh
   1.$ git diff  commitID-1 commitID-2
3.理解Patch标记格式的含义。
```
 # 删除文件
 1.删除文件后， 恢复文件。
```sh
1.$ rm -rf hello.c
2.$ git status
3.$ git checkout hello.c
```
2.从版本库里删除文件。（真正删除文件）
```sh
1.$ git rm hello.c (or) rm hello.c
2.$ git status
3.$ git add .
4.$ git commit
```
# 版本之间切换  
根据commitID， 可以进行版本切换。
```sh
1.$ git reset --hard commitID
```
# 忽略文件
忽略不需要跟踪到git仓库里的文件。
```sh
1.$ touch .gitignore
2.$ vim .gitignore
3.-----
4.a.out
5.-----
6.$ git add .
7.$ git commit
```
# github
1.注册github帐号
    1.注册邮箱， 注意不要使用QQ.com
2.创建gitc仓库
3.从github将创建的gitc仓库， 克隆到本地。
```sh
1.$ git clone https://github.com/username/gitc.git
```
4.将本地仓库与github仓库进行同步， 将本地提交推送到服务器上。
```sh  
1.$ git push origin master
2.input username:
3.input password:
```
5.更新本地仓库， 与github仓库进行同步。将服务器提交拉取到本地。
```sh   
1.$ git pull
```    
# MarkDown语法     
    
    



















    
