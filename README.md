# Web-Utilities
Link： https://suoweihu.github.io/WebUtilities/

----
- 参考了[《使用Github做一个完全免费的个人网站》](https://zhuanlan.zhihu.com/p/91652100)搭建
- 参考了少数派的CSS文件作为样式
----

<!-- 
# 使用Github做一个完全免费的个人网站(步骤很细)

https://zhuanlan.zhihu.com/p/91652100

[Source](https://zhuanlan.zhihu.com/p/91652100 "Permalink to 📡使用Github做一个完全免费的个人网站(步骤很细)")

**首先，我霸都傲天申明绝对是完全免费，不会在文章中推销什么云服务器，虚拟主机等。而且操作步骤上手简单，即使非IT人员也很容易实现。**

> 局限：只能是静态网站的个人网站
> 面向读者：所有人包括非IT人员

首先如果你无法理解“静态网站”的话，那么相信我，静态网站就可以满足你大部分个人网站的需求。其次这篇文章更多的是面向非IT人员，因为我写这篇文章的原因是我的一个同学的故事：

> 我同学小A是律师，他想把自己处理过的一些案件记录在自己的个人博客中，他已经注册了公众号。但是他始终觉得有个网站或者个人博客会显得专业一些，而且还可以展示自己的个人履历，把这个网站链接放在公众号里面会显得跟专业一些。“好吧，我明白了~”

而且学会自己搭建一个静态网站是一个很酷的事情，你可以做一些很漂亮的宣传页，或者表达自我主张的个人博客，或者在我以前的文章里面给别人做一个网页版生日祝福or纪念日等等。

所以开始吧~

## **前言**

首先我们要用到的工具是著名的开源社区Github，我们做的静态网站最终要托管在上面，这个功能叫做“Github Pages”，是一项免费的静态文件部署服务。

虽然Github是国外的网站，但是在国内可以访问并且速度还不错！

> 有人担心，如果以后Github被墙了怎么办？
> 放心，即使被墙了，你学会如下的操作依然可以在类似的国内平台，例如码云等

## **1.申请Github账号**

（如果有账号请直接登录然后跳转到教程下一步）

访问[Github](https://link.zhihu.com/?target=http%253A//github.com/)，点击SIGN UP按钮。（Sign in是登录的意思，应该都很好理解）还有Github是全英文的，没有中文的哦亲，但这不影响我们使用的。

![](https://pic2.zhimg.com/80/v2-8ea3f6182c6b5a788defb6866d02bda5_hd.jpg)

注册很简单，只需要**用户名，密码，邮箱**即可，不需要手机号。（对了，用户名用一个酷一点或者有意义一点的，因为它会出现在你的网址中）

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m5ed11j30ep0iz74r.jpg)注册填写Github用户名密码邮箱

接着，Github会问你是否需要付费使用。这里选择不用，因为Github提供的免费服务已经能满足大部分人包括开发者的需要了。付费服务主要是面向团队以及企业。

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m3htnjj30gv0d4aad.jpg)

后面还会有一些步骤，大概意思就是问你想用Github做什么，你对Git的熟练程度，（感觉像是moba游戏新手调研都会这么做）因为Github网站迭代的原因可能会稍有不同。比如笔者这里试的时候是这样子的。

![](https://pic2.zhimg.com/80/v2-32525025334550b7bfd94ed1dfa72321_hd.jpg)![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m08ljgj30eb0dzjrt.jpg)![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3lzvfnnj30f907jwek.jpg)

然后Github会给你注册的邮箱发送一个确认链接，**请点击链接确认**，不激活的话是无法正常使用Github的服务的。这个是Github的反爬虫系统。（题外话：Github的反爬虫系统很强很强！）

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m1lzy9j30k001wdfq.jpg)

如果收件箱没有看到，那么不用想了，一定在垃圾箱里面！

到这里我们的注册就完成了。

## **2.创建一个仓库**

接下来我们要创建一个仓库，仓库就是保存代码的地方，也就是保存网站的地方。这里我们做一个最简单的网站：个人简历。

1，首先点击“Your repositories”，查看个人全部仓库，第一次肯定是空空如也啊。

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m2hsqjj307206wmx3.jpg)

2，接着我们新建一个仓库

![](https://pic1.zhimg.com/80/v2-328dfe93e5934c79ad8adcc6592a3644_hd.jpg)

3，这一步很重要，仓库的名字不可以随便写，必须是 **\<我的名字\>.github.io**

比如我注册的名字是 zhihu1，所以这里我创建的仓库的名字必须是 ： [http://zhihu1.github.io](https://link.zhihu.com/?target=http%253A//zhihu1.github.io)

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m4xboxj30k00d9mxu.jpg)

4，接着下一步页面会比较复杂，你会看到一大堆看不懂的东西，其实那些事git操作提示。如果你熟练git的话就知道了。不过我们不管这些，我们只需要创建一个新的文件就行啦！

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m4g9ylj30k009f0t8.jpg)

5，新文件的名字不可以乱写哦，**必须是 index.html，**这里大家都一样都写这个。（题外话：静态http文件托管服务的默认访问文件就是index.html）

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m22dpcj30k00cw74q.jpg)

可以参考笔者的内容如下，改成你自己的介绍哦~

    <p>Hello 大家好</p>
    <p>我是霸都丶傲天，这是我的个人网站。 </p>
    <p>很高兴你来到这里, 你可以在以下的网站找到我</p>
    
    <ul>
      <li> <a href="https://www.zhihu.com/people/AJLoveChina">知乎</a> </li>
      <li> <a href="http://hejie.nigeerhuo.com">我的博客(已经不更细了,现在在知乎写文章)</a> </li>
    </ul>

## 3.查看网站的网址

到这里，我们一个最简单的个人网站的代码就完成了。接下来最重要的一步，我们需要知道网站的链接啊，只有这样，别人才能访问我们的网站呀。

1，点击settings

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m0mbpxj30k0048mx7.jpg)

2，然后往下翻找到 Github Pages， 看到绿色提示，后面的链接就是你的网站地址了，打开看看吧~

**Tip：很多老铁评论说这里看不到绿色框框，没有URL。**那是因为你的仓库名称与用户名不一致，不过不用担心，也是有办法的，看下面的第二张图片。

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3lzmqrnj30f907jwek.jpg)第一张图片![](https://pic1.zhimg.com/80/v2-5853ec09142aa91a84e941324a9d75b8_hd.jpg)第二张图片(这里我设置成小图防止误导正常老铁, 点击可以放大图)

3，点开网站看一下

![](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m13e3yj30b808idg6.jpg)

完成！

其实细心的同学会发现，其实我们的网站地址和我们写的仓库名称是一样的，是滴！而且非常有个性的是我们的名字还出现在网站地址中。

笔者的Github仓库&&网址：[Git仓库地址](https://link.zhihu.com/?target=https%253A//github.com/zhihu1/zhihu1.github.io) [http://zhihu1.github.io/](https://link.zhihu.com/?target=http%253A//zhihu1.github.io/) 

本来到这里这个教程已经结束了，但是我想有的同学肯定是不满意的。首先你的这个网站做的太简陋了吧，不是我想要的那种!

那好，其实学会这个教程就可以做下面两个非常炫酷的小站点了，一个是生日祝福，一个是爱情纪念日。都是很有意义、很温馨的题材哦：）

[霸都丶傲天：🎂改改数据,为心爱的人做一个超具创意的网页生日祝福吧~​zhuanlan.zhihu.com![图标](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m3y7vuj305003ca9v.jpg)](https://zhuanlan.zhihu.com/p/85899661)[霸都丶傲天：5分钟做一个免费的网页爱情树,快快学习发给自己的女朋友吧(微信QQ都可以查看哦)^\_^​zhuanlan.zhihu.com![图标](https://pic3.zhimg.com/v2-99a4258cb88d3fa71e472a50796f6cda_180x120.jpg)](https://zhuanlan.zhihu.com/p/72907840)[霸都丶傲天：告白气球？🌲圣诞节的创意网页小礼物不了解一下么？​zhuanlan.zhihu.com![图标](https://tva1.sinaimg.cn/large/006tNbRwly1gbb3m31hwzj305003cq2q.jpg)](https://zhuanlan.zhihu.com/p/99136480)

所以是这样子的，我没有演示复杂的网页是因为它需要写的代码太多了，许多第一次接触Github的老铁，或者以前从来没接触过HTML的人就会有点陌生。

是的，这里我们提到了HTML，它就是网页的描述语言，对HTML感兴趣我推荐这些最好的免费自学网站。

* [国内的w3school](https://link.zhihu.com/?target=https%253A//www.w3school.com.cn/html/index.asp) （国内的w3School这两年商业元素越来越浓厚了，不怎么推荐了）
* [国外的w3school](https://link.zhihu.com/?target=https%253A//www.w3schools.com/html/) 网络条件好，并且英语还不错的同学建议看国外的
* 但是业界**最专业**的的自学网站应该是这个 [https://developer.mozilla.org/en-US/docs/Web/HTML](https://link.zhihu.com/?target=https%253A//developer.mozilla.org/en-US/docs/Web/HTML) （Mozilla基金会出的mdn文档，绝对的大牛出品，质量把控）

后面一段时间，我还会出一些更高级的个人网站教程。所谓更高级不是说写一大堆代码，**而是如何使用业界非常流行的静态网站生成器来做个人网站。**静态网站生成器的英文说法叫做**“static-site-generator”。**我们只需要关注创作内容即可，这些工具可以帮助我们把网页做的非常绚丽，非常的awesome！

Github上面有专门的相关主题，并且非常火，这里我给个截图

![](https://pic4.zhimg.com/80/v2-7c1830fde392e02a98ea69847be34ffb_hd.jpg)Github上面有超过1500个静态网站生成工具

> 最后，这篇文章的初衷还是写给对编程知识不懂但是又感兴趣的老铁，以及刚上大学计算机系的后起新秀，做一个个人网站可以很大程度提高自己学习编程的动力，所以我觉得这是很有意义的一件事情。

感谢评论里的老铁各位的建议，有些老铁看了可能会疑惑，我来解答吧：

* wordpress确实是业界做**博客类**网站，或者也叫内容型网站的首选。它适合不会编程但是又想做出很绚丽博客的人，它有很多模板可以选择，每一个模板就是一种风格样式。它不在本次文章的推荐中是因为，使用wordpress需要购买主机或者wordpress专用虚拟主机，是需要付费的。
* @joey大佬提到了“用七牛，阿里之类的对象存储服务做免费的cdn静态网站”。**确实在目前来看它们是比Github Pages可能更优秀的选择。**但是它们有推销的嫌疑，所以我没有推荐这些，类似还有腾讯的COS对象存储，它们都有免费的额度，**大概是一个月免费15GB流量，最高免费10GB文件存储。**对于大部分人来说这些是足够的了。但是它的缺点也很明显，**未来可能需要付费以及需要自己购买域名**（当然你也可以使用它免费提供的域名，很长很难记！因为它看起来像这样子 Ukdalkdkl-china-shanghai-1。xxx。com ）

当然如果对上面感兴趣的老铁也可以在评论里面说，我也可以出类似的文章说一下怎么做的，用起来都很方便。

最后的最后，有什么问题直接评论即可，拜拜┏(＾0＾)┛，楼主镇楼。

![](data:image/svg+xml;utf8,%3Csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20width=%27200%27%20height=%27199%27%3E%3C/svg%3E) -->
