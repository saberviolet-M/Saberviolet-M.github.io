---
title: '超文本标记语言——HTML'
date: 2020-09-16 16:34:47
tags: 学习笔记
---
### html骨架 
!DOCTYPE html——文档类型[HTML 5]
html lang="en"——语言显示
meta charset="UTF-8"——编码规范[字符集]
### 标签语义化
<!--more-->
**排版标签**
1. 标题标签——h1~h6[双标签]
2. 段落标签——p[双标签]
3. 水平线标签——hr[单标签]
4. 换行标签——br[单标签]
5. div和span标签——div、span[双标签]

**文本格式化标签**
1. b、strong——加粗[双标签]
2. i、em——斜体[双标签]
3. s、del——删除线[双标签]
4. u、ins——下划线[双标签]
ps：后者语义强烈

**标签属性(图片标签)**
1. src——源(图像路径)
2. alt——替换文本
3. title——提示文本
4. width——宽度
5. height——高度(二者选一即可)
6. border——带边框

**连接标签**
1. href——链接地址
2. target——打开方式(_blank——开一个新标签页，默认覆盖自身页面)

**base标签**
base target="_blank"——所有连接都是新标签页打开[单标签]

**预格式化文本**
pre——标签里面怎么写怎么显示，基本不咋用[双标签]

**特殊字符**
1. [空格]——[&nbsp;]
2. [<]——[&lt;]
3. [>]——[&gt;]

**表格(table)**
1. table——双标签
2. tr——行[双标签]
3. td——行内数据(单元格)[双标签]
标签属性：border、width、height、align[水平对齐方式]、cellspacing(外边距单元格之间)、cellpadding(内边距，单元格内数据和单元格边的距离)
4. th——表头单元格[文字居中加粗][重点在，th是单元格不是行row]
5. caption——表格标题[双标签，置于table之内，tr、th之上]

**合并单元格**
1. rowspan——夸行[合并后删除多余单元格]
2. colspan——跨列[合并后删除多余单元格]

**表格结构划分**
1. thead——表格头部区域[必须有tr标签]
2. tbody——表格内容区域
3. tfoot——表格尾注部分

**列表标签**
1. 无序列表——ul>li[无序]
2. 有序列表——ol>li[有序]
3. 自定义列表——dl>dt(主题)>dd(根据主题的分支，解释说明)[有一个主题和他的分支]

**表单标签**
1. input——单标签[input type=" " value=" " name=" " id=" "]
属性: type value
> text——文本框
> password——密码框
> radio——单选按钮
> checkbox——复选按钮

value：显示表单内的内容(表单值)
name：表单的名字[单选按钮同名则只能选取一个]
checked="checked"——[属性][表示默认选中]

> button——普通按钮
> submit——提交按钮
> reset——重置按钮
> image——图像形式的提交按钮(此项要scr属性表示图片来源)
> file——文件域(上传头像类似这种表单)

2. label标签——扩大标签点击范围
用法：
> 1. 包含input表单
> 2. 通过for(="id")和id(input中id="")

3. textarea——文本域类似留言板[双标签]
   文本框是单一行，文本域能多行显示输入
4. select——下拉列表[内包含option标签，在双标签option内填写内容]

**表单域**
form action="url地址"[提交到哪里] method="提交方式"[怎么提交] name="表单姓名"[提交了啥]
> action——url地址
> method——get/post
> name——表单姓名

推荐网站：
[MDN](https://developer.mozilla.org/zh-CN/)
[w3school](https://www.w3school.com.cn/index.html)
