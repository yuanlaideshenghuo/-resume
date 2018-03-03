
>- ##新建一个项目的教程和克隆已有项目来操作



###新建一个项目的教程和克隆已有项目来操作
   打开自己的github→点开New repository
![](http://upload-images.jianshu.io/upload_images/10835683-331663ce502d5480.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


填写好  文件名称  描述   勾选publi（公共库，所有人都能看见里面的内容），prlivate是要续费才能使用的私有库，勾选Initialize this repository with a README（初次使用建议勾选，会用反之），ok之后Create repository
![](http://upload-images.jianshu.io/upload_images/10835683-5de3140f19a7c088.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

点开Clone or dowmload,切换到shh协议地址，OK之后，复制地址
![](http://upload-images.jianshu.io/upload_images/10835683-f3a6c2396334fadc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
打开终端输入：**git clone git@github.com:yuanlaideshenghuo/yuan.git**(这个就是刚刚复制的地址）
 - git clone(意思就是克隆）![](http://upload-images.jianshu.io/upload_images/10835683-d2504ffca5cb567f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)![](http://upload-images.jianshu.io/upload_images/10835683-e50a6100b89e62c7.png?imageMogr2/auto-![fdg.png](http://upload-images.jianshu.io/upload_images/10835683-c8ffdd4bfa2f953f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
orient/strip%7CimageView2/2/w/1240)

点开**头像**找到**Settings** 点开![](http://upload-images.jianshu.io/upload_images/10835683-78af68a65daab3c4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

进入**generating SSH keys**了解创建shh步骤


![](http://upload-images.jianshu.io/upload_images/10835683-82b32060ba3bb36a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

进入**Generating a new SSH key and adding it to the ssh-agent**了解步骤
![](http://upload-images.jianshu.io/upload_images/10835683-d56f290a6f8d2d02.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
步骤图
![](http://upload-images.jianshu.io/upload_images/10835683-ba6d67394314d914.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

在终端输入**ssh-keygen -t rsa -b 4096 -C "yuanlaideshenghuo.com"**（注意-C是**大写  -C**）

![9.png](http://upload-images.jianshu.io/upload_images/10835683-06fcf3a200491d2a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![10.png](http://upload-images.jianshu.io/upload_images/10835683-3c445ae50b2ac577.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
进去  **.ssh**目录下打开   **cat id_rsa.pub**把里面的串码复制下来
![](http://upload-images.jianshu.io/upload_images/10835683-f79c0120360025a8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
再回到这个界面打开New SSH key
![](http://upload-images.jianshu.io/upload_images/10835683-1c9ad2d809685696.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
这里注意是**ssh-rsa**开头（开头不要留**空格**），自己的**邮箱**结尾，OK之后**Add ssH key**

![](http://upload-images.jianshu.io/upload_images/10835683-67bc9d139878c3e4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这里还要你在输入一次**密码**确认
![](http://upload-images.jianshu.io/upload_images/10835683-bdcbb41168179b1c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
先点开这个猫，之后找到原来的文件点开
![](http://upload-images.jianshu.io/upload_images/10835683-2862e9d3b50b314b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

复制地址（记得是**ssh协议地址**噢）
![](http://upload-images.jianshu.io/upload_images/10835683-607a7bf9ec553a75.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
然后在终端输入**git lone     git@github.com:yuanlaideshenghuo/yuan.git** 回车，到这里Are you sure you want to continue connecting (yes/no)? （意思是你确定要继续连接吗）  输入**yes**回车，到这里我们就有了操作权限了。

![](http://upload-images.jianshu.io/upload_images/10835683-fbf11ef80d4d68d5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

**README.md**这个文件就是我们刚刚默认的文件
![](http://upload-images.jianshu.io/upload_images/10835683-95c0822cdde4dea0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
这个文件可以打开编辑新增文件也可修改，**vim   yuanlai.html**

![](http://upload-images.jianshu.io/upload_images/10835683-8c8fa89d7c1205c3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

推送：**1.git add . 2.git commit -am"add"  3.git push origin master**
![](http://upload-images.jianshu.io/upload_images/10835683-66d9a3a97fcca7fc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

OK之后回到自己的github刷新就可以看到刚刚创建的html了。
![](http://upload-images.jianshu.io/upload_images/10835683-c5b3e7f0feff57e8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

> - 如果想把自己的代码放进自己的仓库通过html给别人演示→点开settings→找到GitHub Pages(把你当前这个项目变成一个线上预览的页面）→点开None换成master branch→自己刷新之后在滑动鼠标回到GitHub Pages这里的网站就是了


##添加文件并提交
>#### 当我们初次使用Git的时候,我们需要设置姓名和邮箱。
>git config --global user.emali “邮箱”（如：yuan@blog.com）
  git config --global user.name“你的姓名”
>####创建文件
> touch  b.md(b就是文件名称）
> echo(这个命令是直接在b.md添加东西的）如：echo “hello” > b.md
>git status
>git push（把本地仓库推送到远程仓库的命令），**如果失败就使用 git push origin master推送，使用一次后面就用 git push就可以了**

![](http://upload-images.jianshu.io/upload_images/10835683-46496e5337cefecc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


##修改删除文件
>git pull （把远程仓库的变动更新到本地仓库）
>vim b.md{}进入编辑器修改文件命令（b.md是文件名称和后缀）}
> git add .  （是放入暂存区命令）
>git commit -a (**注意：如果提交大量字符串，提交命令不用加 m**
>**此时会进入vim界面，按下 i 进入编辑状态，进行编辑**
>**编辑完成后按下 esc 进入命令状态，输入 ：wq 保存退出  vim**)
>git push 

>**删除文件命令（后缀md的）**
  1.rm -rf（可以不输） b.md 
         2. git add . 
3.git commit -am "delete b"   
b就是文件名



#复杂使用
>-  **本地创建一个git项目推送到远程空仓库**
mkdir newProject
cd new Project
把一个文件夹初始化成一个本地 git 仓库
注意 仓库和文件夹的区别在于ck下有一个隐藏的   .git 文件，里面有一些信息
对于一个仓库，删除 .git文件夹，就变成一个普通文件夹了
git init
touch index.html
ceho "hello" > inder.html
git add .
git commit -am "init"


- **详细步骤**

     创建一个新的文件，但是这里没有勾选  **Initialize this repository with a README**（回看看过来之前创建是勾选的）


![](http://upload-images.jianshu.io/upload_images/10835683-99fe1a6de3b424f5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 打开终端
mkdir blogtest1   (创建一个文件夹）
cd blogtest1     （进入这个文件夹）
toush README.md      （然后创建这个文件）
git status  
git init    把本地的空文件夹变为仓库（ 注意： 空文件夹才去执行这个命令，不然克隆的项目全被覆盖）。没有仓库才去执行这命令
git status    
git add .   
git commit -am "init" 
git push
git remote add origin git@github.com:yuanlaideshenghuo/blogtest1.git   （这个命令的意思是说给我这个远程仓库（也就是邮箱）起一个名字叫  origin）
git push origin master    推送到远程地址（所以origin就是代表上面的邮箱）

下面演示
![](http://upload-images.jianshu.io/upload_images/10835683-ded8bdfa9d5db478.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](http://upload-images.jianshu.io/upload_images/10835683-0c1535ec06ee6d23.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
然后刷新就见到文件了
![](http://upload-images.jianshu.io/upload_images/10835683-4060182e99b4a2d5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
>-  **本地创建一个git项目推送到远程空仓库**
> **git remote -v**   (查看本地库里记录的远程库地址)
**git push -f origin master**   （慎用，这样会强制推送，会覆盖别人的代码）
**git remote add abc git@xxx.git** (在是在添加一个远程库的标签命令）(abc就像origin一样是代替邮箱的名称）
 **git push abc master**(这是推送命令)
**git remote remove abc**(删除命令）
**git remote set-url origin git@qaz.com/a.git**   (修改origin标签对应的地址）
**git remote rename abc coding**(把abc标签改名为coding）
#分支操作
**git branch -a**    (查看所有分支） 
**git branch dev** (创建本地库dev 分支）→dev称“开发分支”
**git checkout dev** （切换到dev 分支）
**touch b.md** (b.md就是创建你需要的文件）
**git add .**
**git commit -am “add b.md”**
**git push origin dev** (推送到origin地址的dev分支上）
- **觉得分支没有问题就可以合并到主支上了**
git checkout master (切换到主支上）
git merge dev(合并）
↓
git push origin master(推送到远程仓库）
##冲突
>当自己和别人改同意文件的同一个地方，在执行 git pull 时更新本地合并是会出现冲突
1.修改冲突文件
2.重新提交



 
