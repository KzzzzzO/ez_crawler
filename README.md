# Easy Crawler
该Python脚本仅用于爬取页面文本信息，作为语言训练的数据集所使用。
本来是个人使用的，只用来爬贴吧，结果发现还能爬其他网页，于是干脆修改了一下。

# 简介
## Easy Crawler 简易网络爬虫 v0.1
基本上可以爬取大部分页面文本信息。

## 优点
1. 在爬取后可进行去重、删除带有关键字词的文本。
2. 爬取配置操作简易。
3. 可绕过（至少能绕过百度的）身份验证环节。

## 缺陷
1. 爬取的结果乱序。
2. 部分页面爬取的内容无法换行。
3. 一次仅能抓取一类标签的文本。

# 使用方法
## 0. 安装requirements内的所需库（如果需要的话）
## 1. 运行Crawler.py
## 2. 根据提示填入爬取的网址、页数
## 3. 为填入剩下内容，则需要在你想要爬取的网页上按下F12，这里以火狐浏览器为例：
### 3.1 使用“选取页面中的元素”工具，查看你想爬取内容的一部分的源码。
### 3.2 找到类似 div id = "A" class="B" 的内容，其中id、class是标签，"A""B"是标签的具体名
## 4. 根据剩下提示继续进行。
## 5. 在根目录下找到"Output_(X).txt"，即为输出文件。

# Q&A
## Q: 爬取后的输出为空文本。
## A: 可能被身份验证环节拦截了，可以在Chrom加载页面后的代码加入一个input()之类的，完成身份验证后重新运行。当然也有可能标签填写错误，导致找不到要爬取的内容。
## Q: 有的标签具体名的结尾加了空格，我也需要加上么？
## A: 我自己的试的时候是不用加的。
