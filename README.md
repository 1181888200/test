#初始化本地git
git init 

#在本地文件夹下面创建一个文件README.md
#git add把文件添加进去，实际上就是把文件修改添加到暂存区
git add README.md

#git commit提交更改，实际上就是把暂存区的所有内容提交到当前分支
git commit -m "备注信息" 

#和github远程库关联起来，起个名lwl
git remote add lwl https://github.com/1181888200/test/git

#将master枝干上的所有东西推送到服务lwl目录下
git push -u lwl master

    #我在这个地方再次修改一下
#服务器文件被我修改了

#我是本地修改文件上传的

#我在本地又改了一次

git diff #查看冲突的文件
git status #查看文件状态
git pull lwl master #拉取远程库内容 前提是要先关联起来
