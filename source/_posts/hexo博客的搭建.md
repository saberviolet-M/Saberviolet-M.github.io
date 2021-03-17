---
title: 'hexo博客的搭建整理总结'
date: 2020-09-11 19:19:47
tags: 整理总结
---

## 本次博客搭建教程来源如下:

{% asset_img 视频参考.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/视频参考.jpg) -->

[手把手教你从0开始搭建自己的个人博客 |无坑版视频教程| hexo](https://www.bilibili.com/video/BV1Yb411a7ty?t=1677)
<!--more-->
### 第一步
- 安装node.js+git
    + hexo就是基于node的静态博客

{% asset_img node.js.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/node.js.jpg) -->

就百度就行，安装基本下一步……

- windows下的话就win+R进入cmd

{% asset_img 开启终端.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/开启终端.jpg) -->

### 第二步
- 安装hexo
    + npm可能安装比较慢所以用npm安装cnpm然后再安装hexo

{% asset_img cnpm安装.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/cnpm安装.jpg) -->
如下：
```
$ npm install -g cnpm --registry=https://registry.npm.taobao.org
```
{% asset_img cli安装.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/hexo-cli安装.jpg) -->

### 第三步
- 建立一个文件夹存放所有的博客文件，错了就删了重来就行

初始化博客

{% asset_img 初始化博客.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/初始化博客.jpg) -->

看到如下就是初始化完成哒

{% asset_img 初始化博客完成.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/初始化博客完成.jpg) -->

可在本地端口打开

{% asset_img 可在本地端口打开.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/可在本地端口打开.jpg) -->

复制网址到在浏览器就能在本地预览了


一些基础命令

{% asset_img 基础命令.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/基础命令.jpg) -->

这是框架自动生成的博客就叫helloworld

hexo new "My New Post"——生成新的文章页

hexo s(server)——本地启动，简写s就行

hexo g(generate)——重新生成，基本就是修改之后hexo 
clean 然后重新生成

hexo d(deploy)——部署到远端

### 第四步
- 通过Github把博客部署到远端
    + 要用远端部署需要先下载一个git部署插件

{% asset_img 安装git部署插件.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/安装git部署插件.jpg) -->

如下：
```
$ cnpm install --save hexo-deployer-git
```
- 登录github建立新的仓库
    + 注意就仓库和ID要一致 .gihub.io

{% asset_img github构建仓库基础命名必须一致.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/github构建仓库基础命名必须一致.jpg) -->

- 然后就需要设置啦
    +找到如下文件，文件里找到最后面

{% asset_img 更改配置.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/更改配置.jpg) -->
{% asset_img 更改配置信息.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/更改配置信息.jpg) -->
type: git

rerp(就是远程仓库哒): bulabula……

branch(分支): master

ps:分支好像默认就是master，还有记得冒号后面跟空格

然后就可以hexo d往远端推了

{% asset_img 此时git仓库里就有很多东西了.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/此时git仓库里就有很多东西了.jpg) -->

### 关于换主题那些事情
- 找到想要的主题下载下来就好啦 git clone
    + 之后找到配置文件更改主题就好啦

{% asset_img 更改配置.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/更改配置.jpg) -->

默认就是搭建的时候自动下载的主题哒

{% asset_img 换成想要的主题.jpg This is an test image %}
<!-- ![](/source/_posts/hexo博客的搭建/换成想要的主题.jpg) -->

landscape删掉换成新主题就好啦

然后就能生成本地预览查看是否设置哒

然后hexo d就能推到远端啦

---

结尾の言葉:

还在摸索中，前端也是，博客也是，要坚持下去啊