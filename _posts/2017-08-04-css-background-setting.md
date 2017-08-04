---
layout: post
title:  "CSS中background的使用"
date:   2017-08-04 14:06:05
categories: Css  
excerpt: CSS中background的使用  
---  
#### 背景常用属性及其使用  
1. **background-img**:  *url()*;  
   设置背景图片的地址，默认背景图像从一个元素内边距的左上角开始。  
2. **background-repeat**:  *repeat/no-repeat/repeat-x/repeat-y/inherit*    
   设置背景图片平铺属性。   
   默认值为repeat:在水平和垂直方向进行平铺。    
3. **background-position**: 关键词/百分比/长度   
   设置背景图片放置的位置。  
   关键词：第一个值为垂直方向 *(top/center/bottom)*，第二个值为水平方向*(left/center/right)*，以图像的中心点作对比。  
   百分笔：第一个值为水平方向，第二个值为垂直方向（左上角为*0% 0%*，右下角为 *100% 100%*），以图像的中心点作对比。  
   长度：第一个值为水平方向，第二个值为垂直方向(左上角为0 0，单位是像素px或其他)，以图像的左上角的点作对比。  
   >
   如果仅定义了一个值，另一个值将是center或50%     
4. **background-color**: *颜色名称/十六进制的背景色/rgb()/transparent/inherit*    
   设置元素的背景颜色，为元素设置一种纯色。覆盖范围包括内容、内边距、边框。     
   十六进制的背景色和rgb代码背景色可通过查表取得。  
   transparent:如果你不希望某元素拥有背景色，又不希望用户对浏览器的颜色设置影响到你的设计，可设置transparent:默认，背景颜色为透明。  
5. **background-attachment**: *scroll/fixed/inherit*    
   设置背景图像是否固定或者随页面的其他部分滚动,默认scroll。  
6. **background-origin**: *padding-box/border-box/content-box* (CSS3)       
   规定background-position相对于什么来定位，默认padding-box.   
7. **background-clip**: *padding-box/border-box/content-box* (CSS3)  
   规定背景的绘制区域。  
8. **background-size**: *百分笔或像素*    
   规定背景图片的尺寸。  第一个值为水平方向，第二个值为垂直方向。

*事实上所有背景属性都不能继承，IE版本不支持inhert*



