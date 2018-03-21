---
title: 使用 Hexo + GitHub 搭建个人博客
date: 2018-03-21 10:57:23
tags:
---

### 以下是步骤

1、进入一个安全的目录，比如 cd ~/Desktop 或者 cd ~/Documents，别在根目录 / 瞎搞。以后所有的教程第一步都是「进入一个安全的目录，别在根目录瞎搞」，只有 ~ 里面的目录是你能碰的！
2、在 GitHub 上新建一个空 repo，repo 名称是「你的用户名.github.io」（请将你的用户名替换成真正的用户名）
3、npm install -g hexo-cli，安装 Hexo
4、hexo init myBlog
5、cd myBlog
6、npm i
7、hexo new 名称 ， 创建一篇博客
8、start _config.yml，编辑网站配置
&emsp;&emsp;i.把第 6 行的 title 改成你想要的名字
&emsp;&emsp;ii.把第 9 行的 author 改成你的大名
&emsp;&emsp;iii.把第 15 行的 url 改成https://你的github用户名.github.io/myBlog
&emsp;&emsp;iv.把第 16 行的 url 改成/你的github用户名.github.io/
&emsp;&emsp;v.把最后一行的 type 改成 type: git
&emsp;&emsp;vi.在最后一行后面新增一行，左边与 type 平齐，加上一行 repo: 仓库地址 （请将仓库地址改为「你的用户名.github.io」对应的仓库地址，仓库地址以 git@github.com: 开头你知道吧？不知道？不知道的话现在你知道了）例如：git@github.com:用户名/用户名.github.io.git
&emsp;&emsp;vii.第 4 步的 repo: 后面有个空格，不要眼瞎。
9、npm install hexo-deployer-git --save，安装 git 部署插件
10、hexo deploy
11、进入「你的用户名.github.io」对应的 repo，打开 GitHub Pages 功能，如果已经打开了，就直接点击预览链接
12、你现在应该看到了你的博客！

### 第二篇博客
1、hexo new 第二篇博客
2、复制显示的路径，使用 start 路径 来编辑它
3、hexo generate
4、hexo deploy
5、去看你的博客，应该能看到第二篇博客了
