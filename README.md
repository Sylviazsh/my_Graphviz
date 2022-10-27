# my_Graphviz

- [官方文档: Graphviz.org](http://www.graphviz.org/)
- [CSDN: graphviz的基本语法及使用](https://blog.csdn.net/mouday/article/details/80902992)
- [CSDN: graphviz](https://blog.csdn.net/claroja/article/details/82586670)
- 安装: ```sudo apt-get install graphviz```
- 画图: ```dot test.dot -Tpng -o test.png``` 
- vscode安装Graphviz(dot)插件后，Ctrl+Shift+v 开启预览
   - 通过预览界面可以导出svg（Scalable Vector Graphics，基于XML的可缩放矢量图形）

## 语法
```
// 无向图
graph graphname {
     a -- b -- c;
     b -- d;
 }

// 有向图
digraph graphname {
     a -> b -> c;
     b -> d;
 }
```
- 如果subgraph的名字以cluster_开头，所有属于这个子图的节点会用一个矩形和其他节点分开