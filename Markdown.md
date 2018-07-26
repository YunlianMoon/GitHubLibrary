# Markdown

Markdown: An github edit language.  
Common grammer. 

兼容HTML!  

## Title
标题使用不同数量的"#"来标识是什么层级, 可以对应于HTML里面的H1-H6.  
注意#和文字之间有空格.  
example:  
# Yunlian
## Yunlian
### Yunlian
#### Yunlian
##### Yunlian
###### Yunlian

## Newline
在需要换行的地方输入至少两个空格, 然后回车即可. 
还可以直接用html标签\<br /\><br />

### Backslash
可以利用反斜杠来插入一些在语法中有其它意义的符号.  
example:  
想要用\*加在文字旁边来做出强调效果(但不转换成em标签), 可以在\*的前面加上反斜杠\\.  
语法: `\*文字\*`.    
效果: \*文字\*  
warning:  
Markdown支持这些符号前面加上反斜杠来帮助插入普通的符号: \\(反斜杠), \`(反引号), \*(星号), \_(下划线), \{}(花括号), \[](方括号), \()(括弧), \#(井字号), \+(加号), \-(减号), \.(英文句点), \!(惊叹号).

## Link
文章中加入一个链接, 可以通过下面的方式添加:  
\[链接文字](链接地址)  
注意\[]和()要紧挨着.  
example:  
语法: `[Markdown](http://www.markdown.cn/)`  
效果: [Markdown](http://www.markdown.cn/)  
  
简单的链接: <>  
example:  
语法: `baidu: <https://www.baidu.com/>`  
效果: baidu: <https://www.baidu.com/>

## Picture
语法:  !\[Alt text](/path/to/img.jpg) 或 !\[Alt text](/path/to/img.jpg "optional title")  
一个惊叹号!  
接着一个方括号, 里面放上图片的替代文字;  
接着一个普通括号, 里面放上图片的网址.  
注意!, \[]和()要紧挨着.  
建议的做法是将readme.md里面要展示的图片放到仓库里面, 再调用图片链接, 当然直接调用网络上已经有的图片地址也是没有问题的.  
双引号表示鼠标移到该图片将显示的文字.  
example:  
语法: `![a-little-cat](https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg "A Little Cat")`  
![a-little-cat](https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg "A Little Cat")  

点击图片进入某个网页  
example: 点击github的icorn然后再进入`www.github.com`  
语法:  
`[![github-icon](https://avatars1.githubusercontent.com/u/9919?v=4)](http://www.github.com/)`  
效果:  
[![github-icon](https://avatars1.githubusercontent.com/u/9919?v=4)](http://www.github.com/)  
  
指定图片宽高  
Markdown没有指定图片的宽高的语法, 可以使用普通的<img>标签, 利用它的width和height属性来定制宽高.  
example:  
语法:  
`<img src="https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg" width="150" height="100" />`  
效果:  
<img src="https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg" width="150" height="100" />  
  
指定图片对齐方式  
example:  
语法:  
`<p align="center">`  
`<img src="https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg" width="150" height="100" />`  
`<img src="https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg" width="150" height="100" />`  
`</p>`  
效果:  
<p align="center">
<img src="https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg" width="150" height="100" />
<img src="https://github.com/YunlianMoon/GitHubLibrary/blob/master/Images/Markdown-Img/A-little-cat.jpg" width="150" height="100" />
</p>

## Emphasize
可以使用下面的方式给文本添加强调的效果:  
斜体: \*文字\* 或 \_文字\_;  
粗体: \*\*文字\*\* 或 \_\_文字\_\_;  
粗斜体: \*\*\*文字\*\*\* 或 \_\_\_文字\_\_\_;  
删除线: \~\~文字\~\~;  
注意\*, \_, \~与文字要紧挨着.  
example:  
*斜体* 或者 _斜体_  
**粗体** 或者 __粗体__  
***粗斜体*** 或者 ___粗斜体___  
~~删除线~~  

## ListTag
内容需要进行标记, 可以使用下面的方式:  
ordered list are created using 1. + space;  
unordered list are created using * + space or using - + space.  
example:  
- unordered list item
- unordered list item
- unordered list item  
  
任务列表(非标准Markdown语法):  
\- + space + \[x] 或 \- + space +\[ ], \[x]会在方框中画个√;  
example:  
- [x] 任务列表1
- [ ] 任务列表2
- [ ] 任务列表3  

## SplitLine
想用分割线对内容进行分割, 可以在单独一行里输入3个或以上的短横线(-)、星号(\*)或者下划线(\_)实现. 短横线和星号之间可以输入任意空格. 以下每一行都产生一条水平分割线.  
example:  
语法: `***` 或 `---` 或 `___`  
效果:  
***
---
___

## Code
在文章中添加代码,有三种方式.  
第一种方式是使用反引号\`(Esc键下面的按钮)将代码包裹起来;
语法: \`code\`;  
example:  
语法: \`this is a code by backtick\`  
效果: `this is a code by backtick`  
第二种方式则是使用制表符或者至少4个空格进行缩进的行;
example:  
    Indent each line by at least 1 tab, or 4 spaces.  
    var github = exactlyTheWebIWant;  
第三种方式是使用三个反引号\`\`\`(非标准Markdown语法), 三个反引号后面加入引用代码的语言类型;  
语法:  
\`\`\` language  
code  
\`\`\`  
example: language为c++  
语法:  
\`\`\` c++  
int a = 1;  
int b = 2;  
int c = a+b;  
\`\`\`  
效果:  
``` c++
int a = 1;
int b = 2;
int c = a+b;
```

## Quote
在文章中引用了资料, 可以通过一个右尖括号">"来表示这是一段引用内容. 可以在开头加一个, 也可以在每一行的前面都加一个. 还可以在引用里面嵌套其他的引用, 如二级引用加两个右尖括号">>", 以此类推.  
> Right angle brackets &gt; are used for block quotes.  
>> this is the second quote.  

## Table
同时按住shift和\键可调出表格中的|;  
用:表示对齐方式, -(默认左对齐), :-(左对齐), -:(右对齐), :-:(居中);  
-表示列的宽度权重;  
注意表格前必须有空行! 两|之间可以有空格.  
example:  
语法:  
'|Item|Price|Number|  
|--------|-----:|:----:|  
|computer|\$1600|5|  
|cellphone|\$12|12|  
|pen|\$1|234|'  
效果:  

|Item|Price|Number|  
|--------|-----:|:----:|  
|computer|\$1600|5|  
|cellphone|\$12|12|  
|pen|\$1|234|

## Textbox
注意文本框前必须要有空行!  
  
单行文本框  
语法: 在文字前面输入4个空格或者按两个Tab键;  

    这是一个单行的文本框,只要两个Tab再输入文字即可. We can never know what to want, because, living only one life, we can neither compare it with our previous lives nor perfect it in our lives to come.  
  
多行文本框  
语法: 每行文字前面都要有4个空格, 每行结尾处用两个空格换行.  

    这是一个有多行的文本框  
    你可以写入代码等,每行文字只要输入两个Tab再输入文字即可  
    Life sometimes seems too hard and difficult to understand but no matter what obstacles are standing in your way right now you have the power to overcome them. Sometimes your strength lies in stubbornness and determination but even more often it is hidden in your ability to go around obstacles and learn from the previous mistakes. Be strong as a fire that crushes everything in its way and like water that finds a way around any obstacle with gentle determination and a peaceful flow.  

## Expression
非标准的Markdown语法;  
example:  
语法: `表情一：:+1:, 表情二：:o:, 表情三: :smile:`  
效果: 表情一：:+1:, 表情二：:o:, 表情三: :smile:  
you can find all expressions at [表情大全](https://www.webpagefx.com/tools/emoji-cheat-sheet/). if the web page is slow, you can visit [here](https://github.com/YunlianMoon/GitHubLibrary/blob/master/MarkdownExpression.md).  
