---
layout: post
title: 文献检索的基本操作
description: 基本的问下检索操作
date: 2022-03-27 10:54:07
hero_image: https://images.unsplash.com/photo-1457369804613-52c61a468e7d?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1066&q=80
hero_height: is-large
hero_darken: true
image: https://images.unsplash.com/photo-1457369804613-52c61a468e7d?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1066&q=80
tags: resource academic
---

本文写于 2022 年 3 月，内容可能已经过时，请注意检查。

## 1. 有效的检索

1. 检索文献不建议漫无目的的用宽泛的词来进行检索（如：`神经网络`，`深度学习`等），否则很难定位到自己想要的东西。选好一个（组）检索词组，并添加领域限定，是进行有效检索的前提（如：`内窥镜图像 神经网络 算法`）；
2. 善用代表性文献进行检索，一般代表性文献都会引用或被其他文献引用，这会是非常高效的文献检索办法（查阅 Reference 和谷歌他引）；
3. 使用官方的渠道进行检索，如 [CNKI](https://www.cnki.net/), [图书馆外文检索工具（校内使用）](https://hfut.summon.serialssolutions.com/), [WebofScience](https://www.webofscience.com/wos/alldb/basic-search), [IEEEXplore](https://ieeexplore.ieee.org/Xplore/home.jsp), [sciencedirect](https://www.sciencedirect.com/)等。具体可参见我校图书馆已订阅的[电子资源列表](http://lib.hfut.edu.cn/list.php?fid=100)。对于学术类引擎，仅推荐[谷歌学术](https://ac.scmor.com/)，其他暂不推荐。对于如 paperwithcode 等聚合类的网站，可以作为参考，但强烈建议去原文的出版商处查找原始文章；
4. Arxiv, Biorxiv, chinaxiv 等预印本网站，现在也会有较多高质量论文，但在没有正式出版之前，质量难以明确，除非是非常有影响力的文章，否则不建议过多参考；
5. 妥善维护好自己的文献库，以 Zotero 为例，良好的分组和标签习惯是进行本地检索的前提（最新的 Zotero 6.0 已经支持内嵌 PDF 阅读器，支持标注与 PDF 的分离，非常推荐）。

## 2. 中文检索

中文的检索平台主要以知网（CNKI）、万方、维普等商业数据库公司为主，检索途径相对简单。

### CNKI

#### 基本检索

[知网](https://www.cnki.net/)应该是中文搜索的首选，一般教育机构的 IP 都可以正常访问。下图可以看到专利论文等信息都可以在网站上进行检索。

![知网的搜索框](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331160502.png)

我们以`深度学习` `图像分割`为检索词，就可以得到如下结果：
![简单的检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331160754.png)

并进一步对检索得到的内容进行筛选，例如检索学术期刊、学位论文、会议、专利、标准、成果等。
![筛选](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331160952.png)

而对于特定子项，以学术期刊为例，可以在左侧栏进一步筛选，例如发表时间，期刊来源，研究层次等。
![左侧栏](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331161043.png)

#### 高级检索

简单检索可用于找到特定的文献或者宽泛的检索，而对于检索要求更为复杂的情境下，更为实用的可能是知网的高级检索，高级检索可以对于主题、作者、文献来源等等类别进行检索，并且支持模糊匹配。这里可以理解为增强版的基本检索。

> 高级检索支持使用运算符*、+、-、''、""、()进行同一检索项内多个检索词的组合运算，检索框内输入的内容不得超过 120 个字符。输入运算符*(与)、+(或)、-(非)时，前后要空一个字节，优先级需用英文半角括号确定。若检索词本身含空格或\*、+、-、()、/、%、=等特殊符号，进行多词组合运算时，为避免歧义，须将检索词用英文半角单引号或英文半角双引号引起来。

![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331161946.png)
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331162252.png)

而如果我们想要更加复杂的检索过程，可以选择专业检索。

> 专业检索可检索字段包括：SU%=主题,TKA=篇关摘,TI=题名,KY=关键词,AB=摘要,FT=全文,AU=作者,FI=第一责任人,RP=通讯作者,AF=机构,JN=文献来源, RF=参考文献,YE=年,FU=基金,CLC=分类号,SN=ISSN,CN=统一刊号,IB=ISBN,CF=被引频次

例如我想检索管理学部推荐期刊关于`医疗`的相关文献，我就可以编写如下的表达式：

```
SU=(医疗) AND (LY=(管理科学学报) OR LY=(系统工程理论与实践) OR LY=(管理世界) OR LY=(数量经济技术经济研究) OR LY=(中国软科学) OR LY=(金融研究) OR LY=(中国管理科学) OR LY=(系统工程学报) OR LY=(会计研究) OR LY=(系统管理学报) OR LY=(管理评论) OR LY=(管理工程学报) OR LY=(南开管理评论) OR LY=(科研管理) OR LY=(情报学报) OR LY=(公共管理学报) OR LY=(管理科学) OR LY=(预测) OR LY=(运筹与管理) OR LY=(科学学研究) OR LY=(中国工业经济) OR LY=(农业经济问题) OR LY=(管理学报) OR LY=(工业工程与管理) OR LY=(系统工程) OR LY=(科学学与科学技术管理) OR LY=(研究与发展管理) OR LY=(中国人口、资源与环境) OR LY=(数理统计与管理) OR LY=(中国农村经济))
```

![专业检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331162952.png)
当然包括年份、排序等工作，都可以在搜索框中进行额外选择，更多信息可以访问[官方的文档](https://piccache.cnki.net/2022/kdn/index/helper/manual.html#frame2-1-5)。

### 万方数据

#### 基本检索

[万方数据](https://www.wanfangdata.com.cn/index.html?index=true)也是一个常用的平台，内容上与知网大同小异，也分基本检索、高级检索和专业检索，只是部分规则有所不同。其中基本检索部分在此不表，参考知网即可。
![万方](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331163715.png)

#### 高级检索

高级检索点击搜索框右侧即可进入，万方的高级检索与知网略有不同，但是也都是从标题、作者、发表时间等维度进行搜索的，这里需要注意的是，万方**并不支持运算符（\*/+/\^）的检索，请用大小写（and/or/not）代替，（\*/+/\^）将会被视为普通检索词。**

![万方高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331163824.png)
而如果进行更复杂的检索，则可以转到专业检索中，万方提供了更加便捷的可视化规则编写工具，点击即可生成对应的专业搜索结果。例如：`题名或关键词: (("协同过滤" and "推荐算法") or ("协同过滤" and "推荐系统" and "算法") or ("协同过滤算法"))`
![专业检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331164335.png)

### 维普期刊

[维普期刊](https://qikan.cqvip.com/)在部分高校可能比较冷门，但是它绝对可以称得上是中文检索领域的佼佼者。它同样支持基本检索、高级检索和专业检索。

#### 基本检索

![基本检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331164701.png)
由于维普仅收集了期刊文献，因此在检索时范围也更准确。
![维普](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331164755.png)

#### 高级检索

高级检索方面，维普的界面则更为直观，同样可以用逻辑语句，对文献特定的域进行搜索。
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331164958.png)
而对于表达式检索，也就是知网和万方的专业检索方面，维普的规则也是大同小异。

> 支持逻辑运算符 AND（逻辑“与”）、OR（逻辑“或”）、NOT（逻辑“非”）；可检索字段标识符 U=任意字段、M=题名或关键词、K=关键词、A=作者、C=分类号、S=机构、J=刊名、F=第一作者、T=题名、R=摘要；

例如：`(K=(深度学习 OR 神经网络) OR T=医学) AND R=影像 NOT K=视频`即检索了关键词包括深度学习或神经网络，或题目包括医学并且摘要中有影像但关键词没有视频的文献。当然你可以编辑更复杂的规则。

### 查收查引

中文文献搜索的另一个重要目标就是查收查引，一般来说，上述的搜索引擎都会在显著位置标识出来收录和引用的情况。
![一个收录标识范例](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331165611.png)

如果需要更加专业的检索，还是建议去我校的[图书馆申请文献检索报告](http://lib.hfut.edu.cn/bencandy.php?fid=145&id=83)，作为教育部下属的科技查新站，学校图书馆出具的检索报告是被广泛认可的。

### 中文专利检索

由于专利的时效性较强，专利检索则不能完全依赖上述平台。这里还是推荐前往[国家知识产权局](http://pss-system.cnipa.gov.cn/sipopublicsearch/portal/uiIndex-pubservice.shtml)进行搜索，这里检索国内外的专利文件，并进一步的对专利的元素进行筛选。
![](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/%E5%8A%A8%E7%94%BB.gif)

在注册登录后，还可以进一步解锁新页面，获得更为简单的支持全文模糊检索的工具，并进一步下载。
![](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331170555.png)

其实如果仅仅是下载权利要求书，则更加推荐[谷歌专利](https://patents.google.com/)，检索下载都更方便。

## 3. 英文检索

英文的文献库可以用浩如烟海来形容了，几乎每家出版社都会有一个自己的在线文献搜索引擎。因此，当明确了出版社的时候，还是推荐去他们的出版社搜索引擎进行搜索，下面简单介绍几个常用的搜索引擎。

### Web of science（SCIE）

WOS 可以说是学术界的\*\*了，大家常说的 SCI 就是来源于此。但是不可否认，强也是真的强。[新版的 WOS](https://www.webofscience.com/wos/alldb/basic-search)比原有的 WOS 搜索引擎要简约很多，但是要注意的是，如果是检索 SCI 文献，请选择`核心合集`
![核心合集选择](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331172403.png)
![检索SCI](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331173213.png)

#### 基本检索

基本检索是模糊匹配，支持按域进行检索
![基本检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331172842.png)
其次，可以对检索结果进行分析，这对于情报发现来说，比较有用
![情报分析](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331173026.png)
对于年份、期刊等条目的筛选，在此不表。

#### 高级检索

对于高级检索部分，WOS 支持下述字段和逻辑。
![支持字段](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331173307.png)
并且支持交互式录入
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220331173405.png)

### Nature

Nature 及其子刊可以在[Nature 主站](https://www.nature.com/)直接进行搜索，
![基本检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414150233.png)
或者点击 Advanced search 进入高级检索，这里可以进一步选择条目、作者、标题、时间、出版期刊、卷期号、页码等等。
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414150555.png)

### IEEEXplore

主页为[IEEEXplore](https://ieeexplore.ieee.org/Xplore/home.jsp)，在基本检索中，可以对 IEEE 上不同的类别进行筛选检索，以关键词模糊检索整个数据库。
![简单检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414150816.png)
抑或是选择高级检索，进行更为精准的检索，IEEE 同样提供了高级检索和专业检索，其中高级检索可以对文章的特定字段进行更为精确的检索，通过组合规则以实现对文章的定位。
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414150941.png)
专业检索则是可以进一步的编辑出表达式，这提供了更加灵活的规则组合，具体可以参考[Command search examples](https://ieeexplore.ieee.org/Xplorehelp/searching-ieee-xplore/search-examples#command-search-examples)
![专业检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414151210.png)

### ACM

主页为[Digital Library](https://dl.acm.org/)，同样可以进行简单的检索。
![简单检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414151604.png)
抑或是进行高级检索，同样可以选择字段、时间、出版期刊、卷期号等等。
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414151748.png)

### INFORMS

Informs 的主页可以在[PubsOnLine](https://pubsonline.informs.org/)看到，同样可以进行简单检索。
![简单检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414152319.png)
或者点击高级检索
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414152425.png)
在此不做赘述

### ScienceDirect

主页为[ScienceDirect](https://www.sciencedirect.com/)，可以进行简单的搜索，如关键词、作者、期刊名、卷期页码等
![简单搜索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414153032.png)
也可以进一步选择高级检索
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414153125.png)
具体的检索规则可以参考[此处](https://service.elsevier.com/app/answers/detail/a_id/25974/supporthub/sciencedirect/)。

### Taylor & Francis ST

全文托管于[Taylor & Francis Online](https://www.tandfonline.com/)，同样有简单检索
![简单检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414153330.png)
或是选择更为复杂的高级检索，具体规则可以参考右侧的说明。
![高级检索](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414153409.png)

### 英文专利检索

英文专利首选[谷歌专利](https://patents.google.com/)，可以直接进行题目、专利号等的检索
![谷歌专利](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414153534.png)
![规则约束](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414153634.png)

## 4. 维护自己的文献库

搜索文献实际上只是开始研究的第一步，需要注意把收集到的文章进行有效的管理归档，好记性不如烂笔头，整理好记下了才是真正有价值的，这里建议以文献管理工具的方式进行归档，例如 Zotero、Endnote 等等。

### Zotero

例如可以在 Zotero 中按文件或标签的维度对文献进行编辑。
![布局](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414170651.png)
进一步的可以在利用 Zotero 内建的编辑器进行 PDF 标注。
![标注](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414170756.png)
特别注意 Zotero6.0 及以上版本才支持，且 PDF 标注需要 Store Annotations in File
![](https://cdn.jsdelivr.net/gh/waynehfut/img@img/img/20220414170921.png)

## 5. 后记

文献检索说来简单，但是在整理完我常用的数据库后发现还是需要比较长的时间，才能真正的形成“高效”的检索方式。
