# Markdown 基本语法


Markdown 是一种轻量级的「标记语言」，易读易写，简洁至上，被广泛使用。这篇文章提供了可以在 Hugo 的文章中使用的基本 Markdown 语法示例。

<!--more-->

{{< admonition >}}
这篇文章借鉴了一篇很棒的[来自 Grav 的文章](http://learn.getgrav.org/content/markdown).

如果你想了解 **Loveit** 主题的扩展 Markdown 语法, 请阅读[扩展 Markdown 语法页面](../theme-documentation-content#extended-markdown-syntax).
{{< /admonition >}}

## 一、标题

```markdown
# 一级标题 h1
## 二级标题 h2
### 三级标题 h3
#### 四级标题 h4
##### 五级标题 h5
###### 六级标题 h6
```

## 二、强调

```markdown
**加粗**
*斜体*
~~删除线~~
***斜体加粗***
~~**删除线加粗**~~
~~*斜体删除线*~~
~~***斜体删除线加粗***~~
```

**加粗**、*斜体*、~~删除线~~、***斜体加粗***、~~**删除线加粗**~~、~~*斜体删除线*~~、~~***斜体删除线加粗***~~

## 三、引用

```markdown
> 引用
>> 嵌套引用
```

> 引用
>> 嵌套引用

## 四、分割线

```markdown
---
***
```

---

***

## 五、图片

```markdown
![Backsided's World](https://backtraxe.github.io/apple-touch-icon.png "Backtraxe's World")
<img src="https://backtraxe.github.io/apple-touch-icon.png" alt="Backtraxe's World" width="30%" height="30%">
```

![Backsided's World](https://backtraxe.github.io/apple-touch-icon.png "Backtraxe's World")

<img src="https://backtraxe.github.io/apple-touch-icon.png" alt="Backtraxe's World" width="30%" height="30%">

## 六、超链接

```markdown
[Backsided's World](https://backtraxe.github.io/)
<https://backtraxe.github.io/>
这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）
[1]: http://www.google.com/
[runoob]: http://www.runoob.com/
```

[Backsided's World](https://backtraxe.github.io/)

<https://backtraxe.github.io/>

这个链接用 1 作为网址变量 [traXe][1]

这个链接用 runoob 作为网址变量 [traXe][traxe]

然后在文档的结尾为变量赋值（网址）

[1]: https://backtraxe.github.io/

[traxe]: https://backtraxe.github.io/

## 七、列表

### 无序列表

```markdown
- 北京
- 上海
- 广州
- 深圳
```

- 北京
- 上海
- 广州
- 深圳

### 有序列表

```markdown
1. 北京
1. 上海
1. 广州
1. 深圳
或者
1. 北京
2. 上海
3. 广州
4. 深圳
```

1. 北京
1. 上海
1. 广州
1. 深圳

### 列表嵌套

```markdown
- 北京
- 上海
- 广东
  1. 广州
  2. 深圳
```

- 北京
- 上海
- 广东
  1. 广州
  2. 深圳

## 八、表格

```markdown
姓名|分数|排名
--|:--:|--:
张三|100|1
李四|85|2
王五|60|3
```

姓名|分数|排名
--|:--:|--:
张三|100|1
李四|85|2
王五|60|3

> - `--`，`:--` : 左对齐
> - `:--:` : 居中
> - `--:` : 右对齐

## 九、代码

### 单行代码

```markdown
`print("Hello World!")`
```

`print("Hello World!")`

### 多行代码

```markdown
\```cpp
#include<iostream>
int main() {
    std::cout << "Hello World!" << std::endl;
    return 0;
}
\```
```

```cpp
#include<iostream>
int main() {
    std::cout << "Hello World!" << std::endl;
    return 0;
}
```

## 十、流程图

```markdown
\```flow
st=>start: 开始
op=>operation: My Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
\```
```

```flow
st=>start: 开始
op=>operation: My Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
```

## 十一、LaTeX公式

### 行内公式

```markdown
$ E=mc^2 $
```

$ E=mc^2 $

### 多行公式

```markdown
$$ \sum_{i=1}^n a_i=0 $$
$$ f(x_1,x_2,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$
```

$$ \sum_{i=1}^n a_i=0 $$

$$ f(x_1,x_2,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$




