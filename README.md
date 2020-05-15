# 基本语法

## 1. 标题

两种标记：底线（ - / =）和 #。  

- **底线仅支持二级标题**
- = 表示一级标题
- \- 表示二级标题    

* **#支持六级标题**
* \# 的个数表示等级
* 建议在\# 加一个空格

*建议使用#，前后空一行，不要有多余的空格。*

## 2. 粗体和斜体

- 斜体由一个* / _ 包裹
- 粗体由一个* / _ 包裹

*建议使用\*，不要用空格*

## 3. 段落与换行

不同的段落之间使用空行来标记。  
段内换行需要在上一行末尾插入至少两个空格并回车。

## 4. 列表

有序列表：数字符号+英文句号+空格+列表内容标记；  
无序列表：\*/+/- +空格+列表内容标记。

*列表可以互相嵌套，建议使用-来标记。*

## 5. 分割线

分割线由3个以上的\*/-/_来标记。

*可以在标记符中间加上空格。*

## 6. 图片

> 插入图片语法为：\!\[图片替换文字](图片地址)

- 图片替代文字在图片无法正常显示时才有用；
- 图片地址可以是本地路径也可以是网络图片地址；

## 7. 链接

### a. 文字链接

> 语法：\[链接文字](链接地址)

 支持Markdown语法的编辑器是[Tpyora](https://typora.io/)

### b. 引用链接

引用链接把链接地址作为“变量”先在Markdown文件的尾页定义好，然后在正文中进行引用。其语法如下：  

> **正文中，链接标记可理解为“变量”**  
> \[链接文字] [链接标记]  
> **尾页中**  
> \[链接标记]: 链接地址 

我们经常用到的网站有[Google][google]、[GitHub][GitHub]和[Stack Overflow][Stack Overflow]

- 链接标记不区分大小写
- 网址要以http/https开头，否则会被识别为本地地址

[Google]:https://www.google.com/
[GitHub]:https://www.github.com/
[Stack Overflow]:https://www.overflow.com/

### c. 网址链接

网址或邮箱地址使用<>包裹会被自动识别为超链接

> \<URL 或邮箱地址>

我的邮箱是<zhiwenyang@outlook.com>  
网址是<https://suiyidade.github.io/docsify/#/>

*自动链接要以http/https开头*

## 8. 行内代码与代码块

### a. 行内代码

行内代码块使用“ ` ”包裹

> \`代码块`

使用`cd ..`命令切换到上一级目录

### b. 代码块

代码块以Tab键或4个空格开头

​    #include <stdio.h>  
​    int main(int argv, char argc[])  
​    {  
​        printf(“Hello World!\n”);  
​    }

*此效果不够美观，许多扩展语法（如GFM）提供了围栏代码块，并且支持语法高亮。*

### c. 围栏代码块

可显示声明语言，可以显示语法高亮

> \```python
>
> import keyword
>
> for i in keyword.kwlist:
>
> ​    print(i)
>
> print(‘Hello Python’)
>
> \```  
>
> ```python  
> import keyword  
> for i in keyword.kwlist  
> print(i)  
> print('Hello Python')  
> ```
```c
#include <stdio.h>  
int main(int argv, char argc[])  
{  
	printf(“Hello World!\n”);  
	return 0;
}
```

## 9. 引用

引用由`> + 引用内容`来标记

`> 引用内容`

*引用可以嵌套，建议 > 后有一个空格*

## 10. 转义

在被渲染的符号前添加`\`即可取消相关符号的渲染，可被渲染的符号如下：

```ruby
\  反斜线
`  反引号
*  星号
_  下划线
{} 花括号
[] 方括号
() 括号
#  井号
+  加号
-  减号
.  英文句号
！ 感叹号
```









