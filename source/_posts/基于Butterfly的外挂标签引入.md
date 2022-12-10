---
title: 基于Butterfly的外挂标签引入
date: 2022-11-27 15:22:30
updated: 2022-11-27 15:22:30
tags: 写作
categories: 写作
keywords: 写作
description: 文章必要开头
top_img: https://s1.vika.cn/space/2022/11/16/35827391c4b24ab0a838fb6a94f9e02f
cover: https://s1.vika.cn/space/2022/11/16/35827391c4b24ab0a838fb6a94f9e02f
---
## 标签外挂
{% note simple %}
默认 提示块标签
{% endnote %}

{% note default simple %}
default 提示块标签
{% endnote %}

{% note primary simple %}
primary 提示块标签
{% endnote %}

{% note success simple %}
success 提示块标签
{% endnote %}

{% note info simple %}
info 提示块标签
{% endnote %}

{% note warning simple %}
warning 提示块标签
{% endnote %}

{% note danger simple %}
danger 提示块标签
{% endnote %}

```markdown
{% note simple %}
默认 提示块标签
{% endnote %}

{% note default simple %}
default 提示块标签
{% endnote %}

{% note primary simple %}
primary 提示块标签
{% endnote %}

{% note success simple %}
success 提示块标签
{% endnote %}

{% note info simple %}
info 提示块标签
{% endnote %}

{% note warning simple %}
warning 提示块标签
{% endnote %}

{% note danger simple %}
danger 提示块标签
{% endnote %}
```

## 隐藏代码

{% hideToggle display,bg,color %}
content
{% endhideToggle %}

display可替换为想表达的内容

```
{% hideToggle display,bg,color %}
content
{% endhideToggle %}
```

## 流程标签

使用mermaid标签可以绘制Flowchart（流程图）、Sequence diagram（时序图 ）、Class Diagram（类别图）、State Diagram（状态图）、Gantt（甘特图）和Pie Chart（圆形图），具体可以查看mermaid文档


```
{% mermaid %}
内容
{% endmermaid %}
```

Flowchart流程图

{% mermaid %}
graph TD;
A-->B;
A-->C;
B-->D;
C-->D;
{% endmermaid %}

```
{% mermaid %}
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
{% endmermaid %}
```

Setting the direction of the diagram （流程图）

{% mermaid %}
stateDiagram
direction LR
[*] --> A
A --> B
B --> C
state B {
direction LR
a --> b
}
B --> D
{% endmermaid %}

```
{% mermaid %}
stateDiagram
direction LR
[*] --> A
A --> B
B --> C
state B {
direction LR
a --> b
}
B --> D
{% endmermaid %}
```

Pie Chart（圆形图）

{% mermaid %}
pie
title Key elements in Product X
"Calcium" : 42.96
"Potassium" : 50.05
"Magnesium" : 10.01
"Iron" :  5
{% endmermaid %}

```
{% mermaid %}
pie
title Key elements in Product X
"Calcium" : 42.96
"Potassium" : 50.05
"Magnesium" : 10.01
"Iron" :  5
{% endmermaid %}
```

## 分类标签

{% tabs test1 %}
<!-- tab -->
**This is Tab 1.**
<!-- endtab -->

<!-- tab -->
**This is Tab 2.**
<!-- endtab -->

<!-- tab -->
**This is Tab 3.**
<!-- endtab -->
{% endtabs %}

```
{% tabs test1 %}
<!-- tab -->
**This is Tab 1.**
<!-- endtab -->

<!-- tab -->
**This is Tab 2.**
<!-- endtab -->

<!-- tab -->
**This is Tab 3.**
<!-- endtab -->
{% endtabs %}
```

{% tabs test4 %}
<!-- tab 第一个Tab -->
**tab名字为第一个Tab**
<!-- endtab -->

<!-- tab @fab fa-apple-pay -->
**只有图标 没有Tab名字**
<!-- endtab -->

<!-- tab 炸弹@fas fa-bomb -->
**名字+icon**
<!-- endtab -->
{% endtabs %}

```
{% tabs test4 %}
<!-- tab 第一个Tab -->
**tab名字为第一个Tab**
<!-- endtab -->

<!-- tab @fab fa-apple-pay -->
**只有图标 没有Tab名字**
<!-- endtab -->

<!-- tab 炸弹@fas fa-bomb -->
**名字+icon**
<!-- endtab -->
{% endtabs %}
```
## 字体高亮

臣亮言：{% label 先帝 %}创业未半，而{% label 中道崩殂 blue %}。今天下三分，{% label 益州疲敝 pink %}，此诚{% label 危急存亡之秋 red %}也！然侍衞之臣，不懈于内；{% label 忠志之士 purple %}，忘身于外者，盖追先帝之殊遇，欲报之于陛下也。诚宜开张圣听，以光先帝遗德，恢弘志士之气；不宜妄自菲薄，引喻失义，以塞忠谏之路也。
宫中、府中，俱为一体；陟罚臧否，不宜异同。若有{% label 作奸 orange %}、{% label 犯科 green %}，及为忠善者，宜付有司，论其刑赏，以昭陛下平明之治；不宜偏私，使内外异法也。

```
臣亮言：{% label 先帝 %}创业未半，而{% label 中道崩殂 blue %}。今天下三分，{% label 益州疲敝 pink %}，此诚{% label 危急存亡之秋 red %}也！然侍衞之臣，不懈于内；{% label 忠志之士 purple %}，忘身于外者，盖追先帝之殊遇，欲报之于陛下也。诚宜开张圣听，以光先帝遗德，恢弘志士之气；不宜妄自菲薄，引喻失义，以塞忠谏之路也。
宫中、府中，俱为一体；陟罚臧否，不宜异同。若有{% label 作奸 orange %}、{% label 犯科 green %}，及为忠善者，宜付有司，论其刑赏，以昭陛下平明之治；不宜偏私，使内外异法也。
```

## 时间轴

{% timeline 2022,green %}
<!-- timeline 01-02 -->
这是测试页面
<!-- endtimeline -->
<!-- timeline 01-03 -->
这是测试页面
<!-- endtimeline -->
{% endtimeline %}

```
{% timeline 2022,green %}
<!-- timeline 01-02 -->
这是测试页面
<!-- endtimeline -->
<!-- timeline 01-03 -->
这是测试页面
<!-- endtimeline -->
{% endtimeline %}
```

## 友链类

{% flink %}
- class_name: 友情链接
  class_desc: 那些人，那些事
  link_list:
    - name: JerryC
      link: https://jerryc.me/
      avatar: https://jerryc.me/img/avatar.png
      descr: 今日事,今日毕
    - name: Hexo
      link: https://hexo.io/zh-tw/
      avatar: https://d33wubrfki0l68.cloudfront.net/6657ba50e702d84afb32fe846bed54fba1a77add/827ae/logo.svg
      descr: 快速、简单且强大的网志框架

- class_name: 网站
  class_desc: 值得推荐的网站
  link_list:
    - name: Youtube
      link: https://www.youtube.com/
      avatar: https://i.loli.net/2020/05/14/9ZkGg8v3azHJfM1.png
      descr: 视频网站
    - name: Weibo
      link: https://www.weibo.com/
      avatar: https://i.loli.net/2020/05/14/TLJBum386vcnI1P.png
      descr: 中国最大社交分享平台
    - name: Twitter
      link: https://twitter.com/
      avatar: https://i.loli.net/2020/05/14/5VyHPQqR6LWF39a.png
      descr: 社交分享平台
      {% endflink %}

```
{% flink %}
- class_name: 友情链接
  class_desc: 那些人，那些事
  link_list:
    - name: JerryC
      link: https://jerryc.me/
      avatar: https://jerryc.me/img/avatar.png
      descr: 今日事,今日毕
    - name: Hexo
      link: https://hexo.io/zh-tw/
      avatar: https://d33wubrfki0l68.cloudfront.net/6657ba50e702d84afb32fe846bed54fba1a77add/827ae/logo.svg
      descr: 快速、简单且强大的网志框架

- class_name: 网站
  class_desc: 值得推荐的网站
  link_list:
    - name: Youtube
      link: https://www.youtube.com/
      avatar: https://i.loli.net/2020/05/14/9ZkGg8v3azHJfM1.png
      descr: 视频网站
    - name: Weibo
      link: https://www.weibo.com/
      avatar: https://i.loli.net/2020/05/14/TLJBum386vcnI1P.png
      descr: 中国最大社交分享平台
    - name: Twitter
      link: https://twitter.com/
      avatar: https://i.loli.net/2020/05/14/5VyHPQqR6LWF39a.png
      descr: 社交分享平台
      {% endflink %}
```

## 不常见的代码框

{% codeblock [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcodeblock %}

```
{% codeblock [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcodeblock %}
```

{% code [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcode %}

```
{% code [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcode %}
```
