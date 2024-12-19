---
title: Markdown的用法
date: 2024-12-19 15:31:22
tags:
---
在 Hexo 中，使用 Markdown 语法来编写博客文章。这些语法非常简洁，适合用来快速排版和组织内容。以下是常用的 Markdown 语法，帮助你更好地创建图文并茂的博客文章。
1. 标题
Markdown 使用 # 来表示标题的层级，最多可以使用六级标题。
markdown
￼
复制代码
# 这是一级标题

## 这是二级标题

### 这是三级标题

#### 这是四级标题

##### 这是五级标题

###### 这是六级标题

2. 段落和换行
段落通过空行分隔，不同的段落之间要留有空行。
换行：在行尾添加两个空格，然后按回车。
markdown
￼
复制代码
这是第一行。  
这是第二行。  

3. 加粗、斜体和删除线
• 加粗：使用 ** 或 __ 包裹文字。
• 斜体：使用 * 或 _ 包裹文字。
• 删除线：使用 ~~ 包裹文字。
markdown
￼
复制代码
**加粗的文字**

*斜体的文字*
~~删除线的文字~~

4. 列表
• 无序列表：使用 - 或 * 来创建无序列表。
• 有序列表：使用数字和点来创建有序列表。
markdown
￼
复制代码
- 项目1

- 项目2

  - 子项目1

  - 子项目2


1. 第一项

2. 第二项

   1. 子项

   2. 子项

5. 链接
• 普通链接：[链接文字](链接地址)
• 图像链接：![图片描述](图片地址)
markdown
￼
复制代码
[点击这里访问我的博客](https://myblog.com)
![
图片描述](https://example.com/image.jpg)

6. 插入图片
图片的插入和链接很类似，只是前面加上 !。
• 本地图片： 如果图片存放在 Hexo 项目中的 source/images/ 文件夹下，可以这样插入：
markdown
￼
复制代码
![图片描述](/images/your-image.jpg)

• 网络图片： 插入网络上的图片：
markdown
￼
复制代码
![图片描述](https://example.com/image.jpg)

7. 代码块
• 单行代码：使用反引号 ` 包裹代码。
markdown
￼
复制代码
这是 `代码`。

• 多行代码：使用三个反引号 
￼
包裹代码块，可以指定语言以启用语法高亮。
markdown
￼
复制代码
```python
def hello_world():
    print("Hello, World!")

￼
复制代码
￼
8. 引用
引用使用 > 来标记。可以用于引用他人说的话或者加上一些特殊说明。
markdown
￼
复制代码
> 这是一个引用文本。

9. 表格
表格使用 | 分隔列，用 - 来分隔表头和内容。
markdown
￼
复制代码
| 表头1 | 表头2 |
|-------|-------|
| 内容1 | 内容2 |
| 内容3 | 内容4 |

10. 分割线
分割线使用三个或更多的 - 或 *。
markdown
￼
复制代码
---

11. 代码高亮和语法高亮
Hexo 默认支持通过 highlight.js 或 prismjs 来对代码进行高亮显示。
markdown
￼
复制代码
```javascript
console.log('Hello, World!');

arduino
￼
复制代码

### 
12. **嵌入视频**
可以通过嵌入 YouTube、Vimeo 或其他支持嵌入的媒体来插入视频。一般使用 HTML 标签来实现：

```markdown
<iframe width=
"560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>

13. Hexo 特定语法
• <!-- more -->：用来在文章中插入“更多”分隔符，帮助在首页或列表页显示文章的摘要。
markdown
￼
复制代码
这是文章的开头部分。
<!-- more -->
这是文章的剩余部分。

14. 自定义CSS
你可以通过 style 标签在博客中插入自定义的 CSS 样式。将以下代码添加到文章中，即可自定义样式：
markdown
￼
复制代码
<style>
  .custom-class {

    color: red;
    font-size: 20px;
  }
</style>


<div class="custom-class">这是自定义样式的文字</div>

总结
通过掌握这些基本的 Markdown 语法，你就可以在 Hexo 中创建更丰富的文章内容，插入图片、视频和代码，还能进行简单的排版和格式化。只需将这些语法应用到你的 Markdown 文件中，Hexo 会根据这些规则生成你想要的网页内容。
你可以在 Hexo 项目中的 source/_posts/ 文件夹里创建 Markdown 文件，并按照上述方法添加内容，然后使用 hexo generate 或 hexo deploy 来生成并发布文章。