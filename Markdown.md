# Markdown

Markdown: An github edit language.  
Common grammer. 

兼容HTML!    

## Title
标题使用不同数量的"#"来标识是什么层级,可以对应于HTML里面的H1-H6.  
注意#和文字之间有空格.  
example:  
# Yunlian
## Yunlian
### Yunlian
#### Yunlian
##### Yunlian
###### Yunlian

## Newline
在需要换行的地方输入至少两个空格,然后回车即可. 

### Backslash
可以利用反斜杠来插入一些在语法中有其它意义的符号.  
example:  
想要用\*加在文字旁边来做出强调效果(但不转换成em标签),可以在\*的前面加上反斜杠\\.  
语法: `\*文字\*`.    
效果: \*文字\*  
warning:  
Markdown支持这些符号前面加上反斜杠来帮助插入普通的符号: \\(反斜杠), \`(反引号), \*(星号), \_(下划线), \{}(花括号), \[](方括号), \()(括弧), \#(井字号), \+(加号), \-(减号), \.(英文句点), \!(惊叹号).

## Link
文章中加入一个链接,可以通过下面的方式添加:  
\[链接文字](链接地址)  
注意\[]和()要紧挨着.  
example:  
[Markdown](http://www.markdown.cn/)  
  
简单的链接: <>  
example:  
语法:`baidu: <https://www.baidu.com/>`  
baidu: <https://www.baidu.com/>

## Picture
语法:  !\[Alt text](/path/to/img.jpg)  
一个惊叹号!  
接着一个方括号,里面放上图片的替代文字;  
接着一个普通括号,里面放上图片的网址.  
注意!,\[]和()要紧挨着.  
建议的做法是将readme.md里面要展示的图片放到仓库里面,再调用图片链接,当然直接调用网络上已经有的图片地址也是没有问题的.  
example:  
![a-little-cat](https://github.com/YunlianMoon/Markdown/blob/master/Images/little-cat.jpg)   

## Emphasize
可以使用下面的方式给文本添加强调的效果:  
斜体: \*文字\* 或 \_文字\_;  
粗体: \*\*文字\*\* 或 \_\_文字\_\_;  
粗斜体: \*\*\*文字\*\*\* 或 \_\_\_文字\_\_\_;  
注意\*和\_与文字要紧挨着.  
example:  
*斜体* 或者 _斜体_  
**粗体** 或者 __粗体__  
***粗斜体*** 或者 ___粗斜体___  

## ListTag
内容需要进行标记，可以使用下面的方式:  
ordered list are created using 1. + space;  
unordered list are created using * + space or using - + space.  
example:  
- unordered list item
- unordered list item
- unordered list item

## SplitLine
想用分割线对内容进行分割,可以在单独一行里输入3个或以上的短横线(-)、星号(\*)或者下划线(\_)实现.短横线和星号之间可以输入任意空格.以下每一行都产生一条水平分割线.  
***
---
___

## Code
在文章中添加代码,有两种方式.  
第一种方式是使用反引号\`(Esc键下面的按钮)将代码包裹起来;  
example:  
`this is a code by backtick`  
第二种方式则是使用制表符或者至少4个空格进行缩进的行.  
    Indent each line by at least 1 tab, or 4 spaces.  
    var github = exactlyTheWebIWant;  

## Quote
在文章中引用了资料,可以通过一个右尖括号">"来表示这是一段引用内容.可以在开头加一个,也可以在每一行的前面都加一个.还可以在引用里面嵌套其他的引用,如二级引用加两个右尖括号">>",以此类推.  
> Right angle brackets &gt; are used for block quotes.  
>> this is the second quote.  

## Table


## Textbox
