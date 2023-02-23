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
使用命令code README.md创建一个文件夹，命名为“README.md”, 按回车，启动Vs Code，在Vs Code界面下输入内容，然后保存，关闭Vs Code

# 第八步：把经过编辑的README.md提交到git管辖

使用命令：git commit，把刚刚我们编辑过的README.md文件提交给git管辖，命令行界面会弹出关于本次提交的说明信息

说明：提交之后，可以再用git status命令查看git的状态，观察前后的变化

# 第九步：登录自己的github账户，创建一个命名为“learn-git”的仓库

创建仓库时，为这个仓库取个名字就行，github远程仓库名称可以和本地仓库名称一致，也可以不一致，对于初学者来说，建议让本地文件夹名称和github远程仓库名称保持一致，这样方便我们学习。

为仓库完成命名后，当前页面的其他选项保持默认状态，点击最下方的“创建”按钮，然后弹出一个页面，从上到下有三个选项，分别是：

**…or create a new repository on the command line（**使用命令行创建一个新的仓库**）**

```jsx
echo "# leran-git" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/AndyZhou6688/leran-git.git
git push -u origin main
```

**…or push an existing repository from the command line（把现存的本地仓库push到github）**

```jsx
git remote add origin https://github.com/AndyZhou6688/leran-git.git
git branch -M main
git push -u origin main
```

**…or import code from another repository（从其他仓库import代码）**

You can initialize this repository with code from a Subversion, Mercurial, or TFS project.

# 第十步：把本地仓库push到github

```jsx
git remote add origin https://github.com/AndyZhou6688/leran-git.git
git branch -M main
git push -u origin main
```

在当前工作目录下（刚刚创建的README.md文件所在的目录），这点很重要，千万不要弄错。

“git remote add origin https://github.com/AndyZhou6688/leran-git.git”这句话的意思是：让我们本地创建的仓库把我们在github上创建的那个公共仓库关联起来。

“git push -u origin main” 这句话的意思是把本地仓库（文件夹）push（推）上github远程仓库

# 第十一步：输入自己github仓库的账号和密码

# 第十二步：刷新自己github上的“learn-git”仓库