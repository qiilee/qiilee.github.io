---
layout: post
title: 如何搭建一个独立博客——简明 Github Pages与 jekyll 教程
date: 2014-05-10 13:31:54
categories: blog
tags: [Hexo,github,独立博客]
description: 这是一篇很详尽的独立博客搭建教程，里面介绍了域名注册、DNS设置、github 和 jekyll 设置等过程，这是我写得最长的一篇教程。我想将我搭建独立博客的过程在一篇文章中尽可能详细地写出来，希望能给后来者一个明确的指引，同时用这篇教程开篇，正式开始我的第八大洲之旅。
---

更新：


- 2015-11-10 01:07:55
- 2015-11-06 01:21:21


----


摘要：这是一篇很详尽的独立博客搭建教程，里面介绍了域名注册、DNS 设置、github 和 jekyll 设置等过程，这是我写得最长的一篇教程。我想将我搭建独立博客的过程在一篇文章中尽可能详细地写出来，希望能给后来者一个明确的指引，同时用这篇教程开篇，正式开始我的[第八大洲之旅](http://www.douban.com/note/523589521/)。

## 前言

作为一个技术小白，没有技术基础，看网上的教程也云里雾里，看程序员的教程相当不容易，稍微有些细节描述得不清楚自己就要绕弯路去找答案（善用搜索引擎），所以，在自己的博客搭建完成之后，我决定要将我搭建博客的过程全记录下来，以供后期和我一样的小白参考（是的，我坚信还有很多一样和我一样的人），我会尽可能详细的整理这个教程，其中的资料可能会摘录到其他人的教程，我会在后面列出了参考资料，感谢这些作者们。

为什么要开博客？可以看看我的这篇[《为什么你要写博客？》](http://zhuanlan.zhihu.com/cnfeat/19743861)

也可以看看这篇[《我的博客时代》](http://zhuanlan.zhihu.com/cnfeat/19743255)

以下以我的博客:www.cnfeat.com为例，教大家如何搭建一个独立博客。

##为什么要搭建一个独立博客?

独立的才是自己的。

##小白进入门槛

- 1、非常折腾，需要耐心；
- 2、也需要一定的学习能力和钻研精神；
- 3、懂一些网页基础知识，不懂也重要，参看第二和第三条；

##小白白请看

2014年5月15日更新：发现一个更简单的方法：[用静态页面生成静态博客](http://isnowfy.github.io/about-simple-cn.html) byisnowfy

按此教程操作即可。

##为什么选择GitHub Pages？

很多人用 wordpress，你为什么要用 github pages 来搭建？

- 1、github pages有300M免费空间，资料自己管理，保存可靠；
- 2、学着用 github，享受 github 的便利，上面有很多大牛，眼界会开阔很多；
- 3、顺便看看 github 工作原理，最好的团队协作流程；
- 4、github 是趋势；
- 5、你不觉得一个文科生用 github 很 geek 吗？瞬间跻身技术界；
- 6、就算 github 被墙了，还可以搬到国内的 gitcafe 中去。

![](http://cnfeat.qiniudn.com/bg2012082502.jpg)

##GitHub Pages是什么？

GitHub Pages 本用于介绍托管在 GitHub 的项目， 不过，由于他的空间免费稳定，用来做搭建一个博客再好不过了。

>github Pages可以被认为是用户编写的、托管在github上的静态网页。

![](http://cnfeat.qiniudn.com/1.png)

##购买域名

只推荐上 [godaddy](https://www.godaddy.com/) 购买，安全，而且可以使用支付宝。

教程（截止至2014年5月10日）如下

**1、查你想要的域名**；


![](http://cnfeat.qiniudn.com/2.png)


**2、查到适合的域名之后选择「continue to Cart」**；

![](http://7d9mjz.com1.z0.glb.clouddn.com/goodcnfeat-buy.jpg)

**3、godaddy附加收费服务，不要管，继续「continue to Cart」**；

![](http://cnfeat.qiniudn.com/4.png)

**4、确认购买** 修改购买年限，默认是两年，可以修改成 1/2/3/5/10 年，随自己喜欢。现在 godaddy 上 com 每年的默认费用是12.99美元，附加上ICANN的管理费用就是13.17美元。

![](http://cnfeat.qiniudn.com/5.png)


如果你不是土豪，可以上网搜 godaddy 的优惠码，一大堆，找一个填进这里，填完之后，一年的费用会变成8.99美元。

![](http://cnfeat.qiniudn.com/61.png)


**说明一下**：一般来讲，使用网上的优惠码第一年收费8.99美元，以后每年的收费是10.99美元，不过在网上可以搜到合适的优惠码，可以每年的收费都是8.99美元，记得多测试自行鉴别。

如图，我买了五年的费用就是45.85美元，随后点击「Proceed to Checkout」

![](http://cnfeat.qiniudn.com/6.png)


**5、结算。**登录或注册界面，填完必要的信息之后，选择用支付宝结算。

![](http://cnfeat.qiniudn.com/7.png)



如果以上的教程如果不够清晰，可以参照这一份[《2013年10月新版godaddy域名注册图文教程》](http://www.admin5.com/article/20131014/527495.shtml)。

**6、检查。**结算后，重新登录，去「My Account」，域名已经显示在你的账户了。

![](http://cnfeat.qiniudn.com/8.png)



**7、补充一些注意事项：**

- 输入优惠码没有优惠或者优惠幅度较低，请清除浏览器 cookies 再尝试；
- 如果没有支付宝支付选项，有可能是使用的优惠码不支持支付宝，请重新清除浏览器 cookies 再尝试；
- 注册时用户填写信息时一定要输入正确的邮箱名字，否则修改十分麻烦。
- 买完域名之后一定要记得去自己的邮箱查看激活邮件，否则域名激活不了。

##安装准备软件

依次下载安装。

- 1、[Node.js](http://nodejs.org/)
- 2、[Git](http://git-scm.com/)

## 怎么打开Git？


### Win 平台操作 

- 1、开始菜单Git Bash

![](http://cnfeat.qiniudn.com/9.jpg)

- 2、鼠标右键打开Git Bash

![](http://cnfeat.qiniudn.com/s10.jpg)

### Mac 平台操作

安装 git 之后可直接在 terminal 操作



##注册GitHub

访问：http://www.github.com/ 

注册你的username和邮箱，邮箱十分重要，GitHub上很多通知都是通过邮箱的。

注册过程比较简单，详细也可以看：

[一步步在GitHub上创建博客主页 全系列](http://pchou.info/web-build/2013/01/03/build-github-blog-page-01.html) by pchou（推荐）

## 配置和使用 Github

以下教程主要参考beiyuu的[《使用Github Pages建独立博客》](http://beiyuu.com/github-pages/)写成。

## 配置 SSH keys

我们如何让本地git项目与远程的github建立联系呢？用SSH keys。

### 检查 SSH keys的设置

首先我们需要检查你电脑上现有的ssh key：

    $ cd ~/.ssh 检查本机的ssh密钥

如果提示：No such file or directory 说明你是第一次使用git。

###生成新的SSH Key：

    $ ssh-keygen -t rsa -C "邮件地址@youremail.com"
    Generating public/private rsa key pair.
    Enter file in which to save the key (/Users/your_user_directory/.ssh/id_rsa):<回车就好>

注意1: 此处的邮箱地址，你可以输入自己的邮箱地址；注意2: 此处的「-C」的是大写的「C」

然后系统会要你输入密码：

    Enter passphrase (empty for no passphrase):<输入加密串>
    Enter same passphrase again:<再次输入加密串>

在回车中会提示你输入一个密码，这个密码会在你提交项目时使用，如果为空的话提交项目时则不用输入。这个设置是防止别人往你的项目里提交内容。

注意：输入密码的时候没有*字样的，你直接输入就可以了。

最后看到这样的界面，就成功设置ssh key了：

![](http://cnfeat.qiniudn.com/11.png)

###添加 SSH Key 到 GitHub

在本机设置SSH Key之后，需要添加到GitHub上，以完成SSH链接的设置。

- 1、打开本地C:\Documents and Settings\Administrator\.ssh\id_rsa.pub文件。此文件里面内容为刚才生成人密钥。如果看不到这个文件，你需要设置显示隐藏文件。准确的复制这个文件的内容，才能保证设置的成功。

- 2、登陆github系统。点击右上角的 Account Settings--->SSH Public keys ---> add another public keys

- 3、把你本地生成的密钥复制到里面（key文本框中）， 点击 add key 就ok了

![](http://cnfeat.qiniudn.com/s12.jpg)


###测试

可以输入下面的命令，看看设置是否成功，git@github.com的部分不要修改：

    $ ssh -T git@github.com

如果是下面的反馈：

    The authenticity of host 'github.com (207.97.227.239)' can't be established.
    RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
    Are you sure you want to continue connecting (yes/no)?

不要紧张，输入yes就好，然后会看到：

    Hi cnfeat! You've successfully authenticated, but GitHub does not provide shell access.

###设置用户信息

现在你已经可以通过 SSH 链接到 GitHub 了，还有一些个人信息需要完善的。

Git 会根据用户的名字和邮箱来记录提交。GitHub 也是用这些信息来做权限的处理，输入下面的代码进行个人信息的设置，把名称和邮箱替换成你自己的，名字必须是你的真名，而不是GitHub的昵称。

    $ git config --global user.name "cnfeat"//用户名
    $ git config --global user.email  "cnfeat@gmail.com"//填写自己的邮箱

### SSH Key 配置成功

本机已成功连接到 github。

若有问题，请重新设置。常见错误请参考：

[GitHub Help - Generating SSH Keys](http://help.github.com/articles/generating-ssh-keys)

[GitHub Help - Error Permission denied (publickey)](http://help.github.com/articles/error-permission-denied-publickey)



## 将独立域名与 GitHub Pages 的空间绑定


### DNS 设置

用 DNSpod，快，免费，稳定。

注册[DNSpod](www.dnspod.cn)，添加域名，如下图设置。

![](http://cnfeat.qiniudn.com/15.png)



其中A的两条记录指向的ip地址是github Pages的提供的ip

- 192.30.252.153
- 192.30.252.154

如博客不能登录，有可能是 github 更改了空间服务的 ip 地址，记得及时到在[GitHub Pages](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages)查看最新的ip即可

www 指定的记录是你在 github 注册的仓库。

### 去 Godaddy 修改 DNS 地址

更改 godaddy 的 Nameservers 为 DNSpod 的 NameServers。

![](http://cnfeat.qiniudn.com/16.png)

1、点击「My Account」，管理我的域名。

![](http://cnfeat.qiniudn.com/17.jpg)


2、点击域名。

![](http://cnfeat.qiniudn.com/18.jpg)



3、将 godaddy 的 Nameservers 更改成 f1g1ns1.dnspod.net 和 f1g1ns2.dnspod.net


![](http://cnfeat.qiniudn.com/19.jpg)

如有不详看可以看[DNSpod提供的官方帮助](https://support.dnspod.cn/Kb/showarticle/tsid/42/)

详细也可以看这里：[一步步在GitHub上创建博客主页(3)](http://pchou.info/web-build/2013/01/05/build-github-blog-page-03.html)

## 使用 GitHub Pages 建立博客

与 GitHub 建立好链接之后，就可以方便的使用它提供的Pages服务，GitHub Pages分两种，一种是你的GitHub用户名建立的username.github.io这样的用户&组织页（站），另一种是依附项目的pages。

想建立个人博客是用的第一种，形如cnfeat.github.io这样的可访问的站，每个用户名下面只能建立一个。



### Fork 已设置好的仓库

点击 [cnfeat/blog.io](https://github.com/cnfeat/blog.io/tree/master)

点击右上角的 Fork 

![](http://7d9mjz.com1.z0.glb.clouddn.com/fork-blog-io.jpg)

这样，你就得到我的博客仓库了。


你可以到

    https://github.com/你的用户名/blog.io

确认一下


将 blog.io 改成 你的 github 用户名.github.io

例如我的就改成 cnfeat.github.io

改好之后，可以发现，'你的 github 用户名.github.io' 已经可以访问了。


## 将独立域名与 GitHub Pages 的空间绑定

### GitHub Pages 的设置


去到你的 blog.io 仓库，点击 CNAME ,再点击右下角的 铅笔 编辑，将 cnfeat.com 改成你的域名


![](http://7d9mjz.com1.z0.glb.clouddn.com/edit-CNAME.jpg)

这样，你再去你绑定的域名看看，估计已经导向到 '你的用户名.github.io' 了。

## 搭建完成

至此，独立博客就算搭建完成，如需进步一完善请在参看以下文章或博客下留言。

## 如何更新博文


### 下载博客模板的 ZIP

去到你 frok 的仓库地址：https://github.com/你的用户名/你的用户名.github.io

点击右下角的 Download ZIP，你会得到一个名为「你的用户名.github.io-master.zip」的压缩包。

![](http://7d9mjz.com1.z0.glb.clouddn.com/github-zip-down.jpg)

解压到本地，将文件夹改名为'你的 github 用户名.github.io' 

### 安装 github desktop 

下载地址：[GitHub Desktop](https://desktop.github.com/)

### 打开你刚刚下载的文件夹



![](http://cnfeat.qiniudn.com/add-folder-to-github.jpg)

点击左上角的「+」号，选择 add，choose '你的 github 用户名.github.io' 文件夹。

如此，你的本地博客仓库就已经和 github 的仓库同步起来了。




2015-11-06 01:18:36


挖坑，待补增






##404页面

GitHub Pages有提供制作404页面的指引：[Custom 404 Pages](https://help.github.com/articles/custom-404-pages)。

直接在根目录下创建自己的404.html或者404.md就可以。但是自定义404页面仅对绑定顶级域名的项目才起作用，GitHub默认分配的二级域名是不起作用的，使用hexo server在本机调试也是不起作用的。

推荐使用[腾讯公益404](http://www.qq.com/404)。

##图床

推荐使用七牛（10G空间，免费）。

我是七牛的付费用户。



## 参考资料：

[1][一步步在GitHub上创建博客主页 全系列](http://pchou.info/web-build/2013/01/03/build-github-blog-page-01.html) by pchou（推荐）

[2]网站优化：[一步步在GitHub上创建博客主页(6)](http://pchou.info/web-build/2013/01/09/build-github-blog-page-06.html) by pchou （推荐）

[3][搭建一个免费的，无限流量的Blog----github Pages和Jekyll入门](http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html) by 阮一峰（推荐）

[4][hexo系列教程：（二）搭建hexo博客](http://zipperary.com/2013/05/28/hexo-guide-2/) by zippera（推荐）

[5][hexo系列教程：（三）hexo博客的配置、使用](http://zipperary.com/2013/05/29/hexo-guide-3/)by zippera（推荐）

[6][hexo系列教程：（四）hexo博客的优化技巧](http://zipperary.com/2013/05/30/hexo-guide-4/) by zippera（推荐）

[7][hexo你的博客](http://ibruce.info/2013/11/22/hexo-your-blog/) by ibruce（推荐） 

[8][Pacman主题介绍](http://yangjian.me/workspace/introducing-pacman-theme/) by yangjian（推荐）

[9][使用hexo搭建博客](http://yangjian.me/workspace/building-blog-with-hexo/) by yangjian（推荐）

[10][折腾了个Pacman主题](http://wuchong.me/blog/2014/01/24/change-to-pacman/) by wuchong（推荐）

[11]hexo官方写作教程[「Writing」](http://hexo.io/docs/writing.html)

[12]知乎上的教程：[如何搭建个人独立博客？](http://www.zhihu.com/question/20463581)

[13]在GitHub Pages设置独立域名的官方教程：[[Setting up a custom domain with GitHub Pages]](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages)

[14][使用Github Pages建独立博客](http://beiyuu.com/github-pages/) by beiyuu

[15][git/github初级运用自如](http://www.cnblogs.com/fnng/archive/2012/01/07/2315685.html) by 虫师

[16][hexo搭建静态博客以及优化](http://code.wileam.com/build-a-hexo-blog-and-optimize/) by Joanna Wu

[17][使用Hexo搭建个人博客](http://c4fun.cn/blog/2014/03/03/use-hexo-blog/) by c4fun

[18][Github Pages与Hexo建个人博客流程](http://kescoode.com/2013/11/17/github-page-and-hexo-guide/) by Kesco

[19][Git push时重复输入用户名密码的问题](http://zipperary.com/2013/05/26/ssh-errors-with-github/) by zippera

[20][hexo文件结构及网站优化](http://www.solarck.com/) by kevin chen


##相关链接

[1][GitHub Pages主页](https://pages.github.com/)

[2][godaddy域名商](http://www.godaddy.com/)

[3][DNSPOD](www.dnspod.cn)

[4][Hexo官方主页](http://hexo.io/)

[5][GotGitHub：GitHub介绍](http://www.worldhello.net/gotgithub/index.html)（推荐）

[5][图标制作网站：faviconer](http://www.faviconer.com/)

[6]本地测试页[localhost:4000](http://localhost:4000/)


##鸣谢

[wuchong](http://wuchong.me/)

[yangjian](http://yangjian.me)



##[关于我](http://cnfeat.com/about/)

这里有我的个人简介：[关于我](http://cnfeat.com/about/)

如果你想看到我最新的文章，可以关注我的微信公众号「cnfeat」。

![](http://cnfeat.qiniudn.com/1000.png)






