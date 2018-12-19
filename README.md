# Markdown-基本语法
## 目录
- **[分级标题](#1分级标题)**  
- **[斜体粗体](#2斜体粗体)**  
- **[超链接](#3超链接)**  
- **[区块引用](#4区块引用)**  

### 1.分级标题
两种形式：
+ 使用'-'和'='标记一级二级标题
  > 一级标题  
  > '======='  
  > 二级标题  
  > '-------'  

  效果：
  > 一级标题  
  > ========  
  > 二级标题  
  > --------  

+ 使用'#'，表示1-6级标题
  > \# 一级标题  
  > \## 二级标题  
  > \### 三级标题  
  > \#### 四级标题  
  > \##### 五级标题  
  > \###### 六级标题  

  效果：
  > # 一级标题
  > ## 二级标题
  > ### 三级标题
  > #### 四级标题
  > ##### 五级标题
  > ###### 六级标题

### 2.斜体粗体

> \*斜体\*，\_斜体\_  
> \*\*粗体\*\*，\_\_粗体\_\_  
> \*\*\*加粗斜线\*\*\*   
> \~\~删除线\~\~

效果：
> *斜体*，_斜体_  
> **粗体**，__粗体__  
> ***加粗斜线***  
> ~~删除线~~

### 3.超链接
Markdown 支持两种形式的链接语法： 行内式和参考式两种形式，行内式一般使用较多。  
+ 行内式  
  语法：[]里写链接文字，()里写链接地址, ()中的“”中可以为链接指定title属性，title属性可加可不加。title属性的效果是鼠标悬停在链接上会出现指定的 title文字。链接地址与链接标题前有一个空格。
  > 欢迎star\[Markdown-grammar\]\(https://github.com/Young0510/Markdown-grammar\)  
  > 欢迎star\[Markdown-grammar\]\(https://github.com/Young0510/Markdown-grammar "Markdown-grammar"\)  

  效果：
  > 欢迎star[Markdown-grammar](https://github.com/Young0510/Markdown-grammar)  
  > 欢迎star[Markdown-grammar](https://github.com/Young0510/Markdown-grammar "Markdown-grammar")  
+ 参考式  
  语法：参考式链接分为两部分，文中的写法 [链接文字][链接标记]，在文本的任意位置添加[链接标记]:链接地址 “链接标题”，链接地址与链接标题前有一个空格。  

  如果链接文字本身可以做为链接标记，你也可以写成[链接文字][] [链接文字]：链接地址的形式，见代码的最后一行。

  > 欢迎关注我的\[知乎\]\[1\]，\[掘金\]\[2\]，\[stackoverflow\]\[3\]，\[github\]\[\]  
  > \[1\]:https:://www.zhihu.com/people/zhang-liu-ping-55   
  > \[2\]:https:://juejin.im/user/5c1780926fb9a049ca37436c   
  > \[3\]:https:://stackoverflow.com/users/10556742/liuping-zhang   
  > \[github\]:https:://github.com/Young0510  

  效果：
  > 欢迎关注我的[知乎][1]，[掘金][2]，[stackoverflow][3]，[github][]  


  [1]:https:://www.zhihu.com/people/zhang-liu-ping-55  
  [2]:https:://juejin.im/user/5c1780926fb9a049ca37436c  
  [3]:https:://stackoverflow.com/users/10556742/liuping-zhang  
  [github]:https:://github.com/Young0510  

  **注意**：上述的`[1]:https://www.zhihu.com/people/zhang-liu-ping-55`不出现在区块中。  

+ 自动链接
  > \<http://baidu.com>  
  > \<zlpyde@163.com> 

  效果：
  > <http://baidu.com>  
  > <zlpyde@163.com> 
 
### 4.区块引用
语法：引用需要在被引用的文本前加上'>'符号  
>\> 这是一段引用

>\> 这是多行引用
>\> 引用文字1
>\> 引用文字2

效果：  
> 这是一段引用

> 这是多行引用
> 引用文字1
> 引用文字2

+ 引用的多层嵌套  
  语法：区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的'>'  
  > \>请问如何学习前端？
  > \>\>看书
  > \>\>\>看视频

  效果：  
  > 请问如何学习前端？
  >> 看书
  >>> 看视频

+ 引用其他要素  
  引用的区块内也可以使用其他Markdown语法，包括标题、列表、代码区块等  

  > \> 1.  这是第一行
  > \> 2.  这是第二行
  > \> 代码例子：
  > \>print("hello world!")

  效果：  
  > 1.  这是第一行
  > 2.  这是第二行
  > 代码例子：
  > print("hello world!")
  