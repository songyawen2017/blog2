---
layout: post
title:  "sublime中git的使用"
date:   2017-08-03 18:47:05
categories: Front-end
excerpt: sublime中git的使用
---
> sublime可以作为前端开发工具，和git集成后，可以同步代码（博客）到远程服务器。  
主要参考了简书中的这篇文章[sublime中git的使用](http://www.jianshu.com/p/c3fabbeebbeb)

##### 前提要求：

   * 本地Git客户端生成公私钥，将公钥放到远程服务器（github）上，将本地分支和github上的库地址关联
   * sublime中安装了git插件，git插件的用户配置中添加本地Git客户端的安装目录中git.exe的路径
   * 使用sublime中的命令模式，add、commit、push文件

**简单地原理就是：将本地Git和远程github库关联，将sublime和本地Git关联，则在sublime中可使用本地Git客户端push代码到远程github库**

##### 几个细节：
   1. Git客户端下载完成后，需要将git的bin/cmd目录设置到path环境变量中，例如E:/Git/cmd（PS：不加是否可行没有尝试）
   2. 本地Git客户端需要配置几个全局变量:user.name、user.email、push-default（执行push命令的策略，有4种选择）
   3. 在git bash中用$ ssh-keygen -t rsa命令生成公私钥，会提示需要输入保存公私钥的文件名和密码
   4. 生成的秘钥保存在git bash中提示的目录下，而是保存在了Git安装目录下，其中多了.pub后缀的为公钥
   5. 将公钥放到github,在github上建库后，用git remote add origin "github上库的地址" 命令实现本地和远程关联
   6. sublime中Git用户设置可通过菜单打开Git.sublime-settings文件，添加
   		{
	       "git_command":"E:/Git/cmd/git.exe"
        }
   7. 第一次可以在本地生成文件提交后，push到远程某库，此时远程不要有任何文件
