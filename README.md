# HowtoLearnHyperMesh
HyperMesh和OptiStruct学习经验

首先放一个 Altair China 的官方百度云盘：https://pan.baidu.com/s/1c7SLg6#list/path=%2F&parentPath=%2F

以下，HyperMesh 简称 hm，OptiStruct 简称 OS。

## 1. 帮助文档 Tutorials

- 首先学习[HyperWorks帮助文件使用方法简介_V2.pdf](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E5%85%B6%E4%BB%96%E8%B5%84%E6%96%99&parentPath=%2F)。
- 入门直接看Tutorial部分，里边全是实例，跟着操作就行。不要畏惧英文，Tutorials 的英文都很简单。
- 害怕英文的，可以从[这里](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E5%85%AC%E5%BC%80%E5%9F%B9%E8%AE%AD%E8%B5%84%E6%96%99%2F2017%E5%B9%B4%2FHyperMesh%E8%BD%AF%E4%BB%B6%E5%AD%A6%E4%B9%A0%E5%8F%8A%E5%9F%B9%E8%AE%AD%E8%B5%84%E6%96%99%2FHyperMesh_tutorials_hw13.0&parentPath=%2F)下载 hm 的中文讲解视频，从[这里](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E5%85%AC%E5%BC%80%E5%9F%B9%E8%AE%AD%E8%B5%84%E6%96%99%2F2017%E5%B9%B4%2FOptiStruct%E8%BD%AF%E4%BB%B6%E5%AD%A6%E4%B9%A0%E5%8F%8A%E5%9F%B9%E8%AE%AD%E8%B5%84%E6%96%99&parentPath=%2F)下载 OS 的中文视频。
- 帮助文档结构很清晰，选择自己需要的章节学习即可。
- HyperMesh 的帮助文档，有个`Solver Interfaces`。这是 hm 与其他求解器的接口。实际上，hm 中，选择不同的求解器，`Analysis`面板差别最大，也是用处最多。可以认为这个`Solver Interfaces`是对不同求解器下 `Analysis`面板的讲解。使用 LS-Dyna 的用户可以看下。
- 出错信息，out文件，从头至尾翻译一遍

## 2. 百度云盘 网络研讨会

Altair China 的百度云真是个百宝箱，尤其是网络研讨会资料，有不少工程级别的实用视频。

对于新手，个人推荐以下资料

- 其他资料  → 实用教程 → [有限元仿真实践原理](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E5%85%B6%E4%BB%96%E8%B5%84%E6%96%99%2F%E5%AE%9E%E7%94%A8%E6%95%99%E7%A8%8B&parentPath=%2F)   既有理论，又有实践。既有鱼，又有渔。

  以下均为`网络研讨会`文件夹下的资料，排序不分先后

- 2013 [hypermesh 六面体及复制壳结构网格划分解决方案](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2013%2F20130228_HyperMesh%E5%85%AD%E9%9D%A2%E4%BD%93%E5%8F%8A%E5%A4%8D%E6%9D%82%E5%A3%B3%E7%BB%93%E6%9E%84%E7%BD%91%E6%A0%BC%E5%88%92%E5%88%86%E8%A7%A3%E5%86%B3%E6%96%B9%E6%A1%88&parentPath=%2F) 

- 2014 [《OptiStruct&HyperStudy理论基础与工程应用》讲解](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2014&parentPath=%2F) 

- 2014 [改变你的设计流程_Optistruct优化案例培训](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2014%2F20140910_%E6%94%B9%E5%8F%98%E4%BD%A0%E7%9A%84%E8%AE%BE%E8%AE%A1%E6%B5%81%E7%A8%8B_Optistruct%E4%BC%98%E5%8C%96%E6%A1%88%E4%BE%8B%E5%9F%B9%E8%AE%AD&parentPath=%2F) 

- 2017 [HyperMesh高效前处理技术在方程式赛车设计中的应用](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2017%2F20170306_HyperMesh%E9%AB%98%E6%95%88%E5%89%8D%E5%A4%84%E7%90%86%E6%8A%80%E6%9C%AF%E5%9C%A8%E6%96%B9%E7%A8%8B%E5%BC%8F%E8%B5%9B%E8%BD%A6%E8%AE%BE%E8%AE%A1%E4%B8%AD%E7%9A%84%E5%BA%94%E7%94%A8&parentPath=%2F) 

- 2014 [HyperMesh HyperView应用提示和技巧](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2014%2F20140627_HyperMesh_%20HyperView%E5%BA%94%E7%94%A8%E6%8F%90%E7%A4%BA%E5%92%8C%E6%8A%80%E5%B7%A72&parentPath=%2F) 

- 2014 [《HyperMesh_HyperView应用技巧与高级实例》讲解](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2014%2F20140310_%E3%80%8AHyperMesh_HyperView%E5%BA%94%E7%94%A8%E6%8A%80%E5%B7%A7%E4%B8%8E%E9%AB%98%E7%BA%A7%E5%AE%9E%E4%BE%8B%E3%80%8B%E8%AE%B2%E8%A7%A3&parentPath=%2F) 

- 2015 [Optistruct优化案例培训](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2015%2F20151118_Altair%202016%20%E4%BC%98%E5%8C%96%E8%AE%BE%E8%AE%A1%E5%A4%A7%E8%B5%9B-Optistruct%E4%BC%98%E5%8C%96%E6%A1%88%E4%BE%8B%E5%9F%B9%E8%AE%AD%E7%AC%AC%E4%B8%80%E6%9C%9F&parentPath=%2F) 

- 2015 [CAE有限元网格竞赛赛前培训](https://pan.baidu.com/s/1c7SLg6#list/path=%2F%E6%BE%B3%E6%B1%B0%E5%B0%94%E4%BC%81%E4%B8%9A%E7%BD%91%E7%9B%98%2F%E7%BD%91%E7%BB%9C%E7%A0%94%E8%AE%A8%E4%BC%9A%E8%B5%84%E6%96%99%2F2015%2F20150613_Altair%202015%20CAE%E6%9C%89%E9%99%90%E5%85%83%E7%BD%91%E6%A0%BC%E7%AB%9E%E8%B5%9B%E8%B5%9B%E5%89%8D%E5%9F%B9%E8%AE%AD(%E4%B8%80)&parentPath=%2F) 

## 3. 进阶

- 主要是帮助文档的关键字手册，没什么好说的。
- 网络研讨会，很多工程经验值得学习
- [Altair forum 论坛](http://forum.altairhyperworks.com/) ：Altair官方论坛，有Altair的工程师及网友解答问题。大多数普遍性问题都可以搜索到，非常实用，进阶必备。

