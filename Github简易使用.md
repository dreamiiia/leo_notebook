# Github 使用

1. 初始化 `git init`, 这样就会生成一个`.git`文件,这个目录是Git来跟踪管理版本库的，没事千万不要手动修改这个目录里面的文件，不然改乱了，就把Git仓库给破坏了。
2. 第一步，用命令`git add <文件名>`告诉Git，把文件添加到仓库 （`git add .` 添加全部）
3. 第二步，用命令`git commit -m"你要说的话"`告诉Git，把文件提交到仓库
4. 关联你的仓库 `git remote add origin https://github.com/dreamiiia/crawlerstudy.git`

    如果出现错误：[git fatal: 远程 origin 已经存在](http://www.cnblogs.com/leinuo2016/p/6547818.html)
    将配置删除 `git remote rm origin` ，再重新关联就好
5. 上传本地代码 `git push -u origin master`