---  
layout: post   
title: "sublime text的使用"  
date: 2017-08-02 19:58:01  
categories: Sublime text  
excerpt: Sublime text 的使用    
---  

# 菜单项的说明  

* ## 文件   
  具有打开文件（crtl+o）和新建文件(ctrl+n)的功能  

* ## 编辑  
  行列：首行缩进（ctrl+]）和取消缩进(ctrl+[)的功能  
  注释：开启注释（ctrl+/）和取消注释（ctrl+/）的功能  
  文本：插入至行前（ctrl+shift+enter）和插入至行后（ctrl+enter）的功能
  标签：关闭标签(alt+.)

* ## 选择
  展开选定的词（ctrl+d）

* ## 查找
  查找（ctrl+f）和替换(ctrl+h)  

* ## 转到
  转到任何（ctrl+p）

* ## 工具  
  命令面板（ctrl+shift+p）  

* ## 首选项（可自行定制插件、显示）
  浏览插件
  设置-默认
  设置-用户
  主题方案-color scheme
  插件设置
  插件控制

# 转到任何（Go to anything）

提供一个快速定位的功能

快捷键ctrl+p打开后，1. 输入文件名模糊查询，在下拉列表中选择，页面对应显示被选择的文件；   
                    2. 输入路径模糊查询    
                    3. html文件中输入#标记名，可跳转到对应标记      
                    4. css文件中输入@符号，下拉列表中提示所有的选择器，选择后，跳转到被选择的选择器   

# 多行游标  
同时修改多行和添加多行  

同时修改多行(Eg: 可通过shift + ctrl + d来复制)：
    1. 选择一个单词或者符号，按下ctrl+d后会自动选中下一个同样的单词，再次按下ctrl+d后，会选中第三个同样的单词，此时这3行都有光标停留，可对其同时做修改，如果想跳过第2个单词不修改，可通过ctrl+k,ctrl+d快捷键跳过第2个单词。      
    2. 选择一个单词或者符号，按下alt+F3,全选文本内所有的该单词进行修改    
    3. ctrl+a全选后，按下ctrl+shift+l 来制造多行光标后，进行修改    
    4. shift + 鼠标右键拖动（尝试后，没有效果）    

 同时添加多行   
    1、根据上面的方法，选中多行后按下ctrl+enter（插入至行前则按ctrl+shift+enter），增加需添加的内容即可。

 退出多行游标：Esc     

 # 命令面板   
 Eg:  
     1. 设置语法 set syntax: html/markdow/css/javascript等均可选   
     2. 有时候忘记了关闭minimap的快捷键，可通过ctrl+shift+p打开命令面板，输入minimap,即可打开或关闭minimap     
     3. 打开markdown preview,在浏览器中查看markdown文件： 打开命令面板，输入mp，即可打开browser。   

 # 综合练习  

 1. html中关闭标签  
    方法一： alt+.  
    方法二：编辑->标签->关闭当前标签   
    方法三：利用Emmet插件： 输入！号(英文输入法下，最好已选择语法为html)，按下ctrl+e,即自动出现了html主标签   

 2. 同时产生10行li   
    方法一： 输入ul>.item$*10,按下ctrl+e,即产生如下效果:     
    
        <!DOCTYPE html>  
        <html lang="en">  
        <head>  
            <meta charset="UTF-8">  
            <title>hello,emmet</title>  
        </head>  
        <body>  
        <ul>  
            <li class="item1"></li>  
            <li class="item2"></li>  
            <li class="item3"></li>  
            <li class="item4"></li>  
            <li class="item5"></li>  
            <li class="item6"></li>  
            <li class="item7"></li>  
            <li class="item8"></li>  
            <li class="item9"></li>  
            <li class="item10"></li>  
        </ul>  
        </body>  
        </html>   

解释：.item为类名，$为序号，10行






