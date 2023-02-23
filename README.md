# git

# 第一步：配置自己的git

PS C:\Users\Andy> git config --global [user.name](http://user.name/) "AndyZhou6688"
PS C:\Users\Andy> git config --global user.email "[andywy1229@gmail.com](mailto:andywy1229@gmail.com)"
PS C:\Users\Andy> git config --core.editor "code -w"

# 第二步：在本地创建一个文件夹

使用命令：mkdir learn-git，创建一个名为“learn-git”的文件夹

# 第三步：打开learn-git文件夹

使用命令：cd learn-git，打开“learn-git”文件夹

# 第四步：初始化learn-git文件夹

使用命令：git init, 初始化learn-git文件夹

# 第五步：查看learn-git文件夹

使用命令：ls，查看learn-git文件夹下面的内容，由于是刚创建，所以内容为空。

说明：使用git init命令初始化“learn-git”文件夹后，会生成一个后缀为.git的隐藏文件夹，使用一个特殊的命令：ls -force，可以看到这个被隐藏的文件夹

# 第六步：使用git status命令查看git状态

对新手来说，这个操作很重要，我们需要从git的视角观察文件夹里的变化情况

# 第七步：创建一个README.md的文件