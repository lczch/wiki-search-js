# Wiki Search



## 用处
  本项目搭建了一个搜索的前端, 通过输入你先要在wikipedia上查找的keywords, 它可以帮你把相关的节点用图形化, 在图画中进行进一步的搜索.

## 特点
- 使用force graph的方式呈现节点, 你可以随意拖动节点, 并在节点上进行操作.

- 支持对于节点内容的简单预览.

- 会对用户的搜索进行智能的记录.

## 体验
http://195.245.239.29/index.html

## 安装
``` sh
npm install
```
启动:
``` sh
node main.js
```

## 基本操作
- 鼠标可以随意拖动节点;

- 鼠标悬浮在节点上的时候, 显示简略的说明;

- 双击节点, 将以此节点为关键词, 在wiki中进行搜索;

- Ctrl + 左键单击节点, 在新窗口打开节点的wiki页面.

## 更深入的功能
我认为用户输入的第一组keyword是比后续搜索的功能更重要的.
所以, 当用户输入关键词比如(A), 当他经过层层的点击, 找到最终想要的节点B后, 我会在将A和B之间的关系记录下来.

这样, 当下次用户又需要寻找B, 但他又想不起来B的关键词是什么的时候, 他再次输入A, B就会直接显示出来, 用醒目的红色.

这就是我添加的小功能的直觉性的描述.

具体使用此项功能:

1. 当你寻找到想要的节点时, 单击屏幕左上角的蓝色方块, 则此节点被记录;

2. 但你不想要显示当前节点和之前记录的节点的关系时, 点击黑色按钮, 和此节点相关的关系将被删除.

## TODO
- 现在访问wiki还有点慢.

- 为蓝色和黑色按钮加上文字说明. 

