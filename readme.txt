http://blog.jobbole.com/78960/


1.创建一个仓库文件夹，进入到该目录；
2.git init ：将该目录变为git可管理的仓库；
3.git add 文件名:将该文件加入到暂存区中；
4.git commit -m "更新提示":提交到仓库；
5.每次更新后使用3、4步提交到仓库；
6.git diff 文件名:查看文件的更改内容和仓库中的差异；
7.git status：查看git状态；
8.git log：显示文件变更日志；
9.git reset -hard HEAD^:回退到上个版本；
10.git reflog:查看版本变更日志，即时之前退出了命令行，可能显示日志
11.git reset -hard 6fcfc89 :回退到指定版本（和10配合使用） 


建立SSH Key
12.ssh-keygen -t rsa -C "1554988625@qq.com":会在用户目录先新建一个.ssh的文件夹
，用于保存公钥和私钥



远程仓库
13.登录到github,打开"setting",单击"Add SSH Key",填上任意title,在Key中粘贴公钥即
id_rsa.pub中的内容。
14.新建一个远程仓库


提交到远程仓库
15.git remote add origin https://github.com/jiansun719/test.git
16.git push origin master: push到远程仓库


Clone
17.git clone https://github.com/jiansun719/test
