---
layout: post
title: 前端初长成--记在一年半工作之后的回顾与总结
author: beyondouyuan
date: 2017-08-04
categories: blog
tags: [Notes]
description: 杨家有女初长成，养在深闺人未识。天生丽质难自弃，一朝选在君王侧。回眸一笑百媚生，六宫粉黛无颜色。

---

### 写在前面 ###

忽见陌头杨柳色，悔教夫婿觅封侯。

第一次总是紧张而又刺激，纠结了好久，终于还是霸王硬上弓离开了上一家公司--生存还是毁灭？继续留在公司风平浪静的安慰自己慢慢学习还是毅然出去追寻大前端之梦？当然是选择原谅我要去征战星辰大海了！


#### 关于离职 Why ? ####

- 1.公司对于前端的工作需求与个人的工作诉求不相符
- 2.孤独


关于1，前东家公司做第三方支付，在职一年半的时间里，后端的主要业务在于api，对于前段的需求，几乎就是一个可以展示数据的界面，一年半的时间里大概有一年的时间是没有ui配合的工作，划船不用浆，全靠浪！

其次，前后端并不分离，几乎每个项目都是前端自己写好界面模板，然后丢给后端去套用，这种分工模式首先就已经不适合当前的趋势，甚至已经落后，前端只写界面，接口api全然不知，连api都没得（第二声）调用过，养老就美滋滋！

再者，几乎没有参与感，ui设计稿大部分时候是没有的，需求？也许在大部分的人看来前段只是做页面效果的，参与需求讨论？你也配姓赵！

不参与或者说甚至都不知道项目的需求，那么，甚至连最基本的应用场景都不知道，对于不同的应用场景，开发起来也是不同的好吗！

公司对于前端工作的需求太低，事情做得不多，适合养老，但对于征途是星辰大海的人来说，及其不利。打包好的React静态页面都不用，去修改重构的页面都是table布局，分离好的js、css文件最终也是内敛到页面，打包压缩也是徒劳。。。

关于2，近两年了，从大学毕业后自学前端一个月出来实习到现在，除了在社区，以及早期在qq群里有过与同行交流外，就像但申购从未见过女子一般的感觉，这是多么令人绝望啊！当遇到问题，掉进坑里，80%可以在社区可以到Google找到解决办法，剩下的20%，有点时候第二天睡醒起来就能豁然开朗，有的坑爬不出来，那就真的爬不出来了！当解决了一个问题也许已经花了很多时间，耽误进度也没人可问，有时快速的解决了一个难题，站起来兴奋的想跟人交流下心得，牛弹琴，当关注某个新问题或者热门问题，想交流一下，还是自己孤苦伶仃。


公司四个分部，上海没有前端，需要前端时我得去接，深圳没人我得去接，忙完回来广州之前的项目搁置等着我。。。

孤独可以让人学习更多知识，这句话大多数时候都是对的。担不是所有时候都对。

我给过他们机会了。

### 关于工作 What ?

惭愧的说，自学一个月前端便出来实习了，刚出来时，拿到第一份任务时气得我手发抖，我懂的HTML、CSS怎么好像都用不上？写哪里去？怎么写？copy下来的布局怎么千奇百怪？我去，这JS还能这么写？写那么多？不会啊！！！

搜索引擎是最好的老师！

左手设计稿，右手W3C文档，用脚敲键盘，HTML+CSS结构终于都float、position布局出来了。所见所得即所写，颇有成就感，这也是当初选择前端时的原因，用户看到的界面都是我写的！

第一份做出来，信心满满！感觉还不错，第二份设计稿，花花绿绿，错综复杂哦！我去，还要自适应，还要相应式，还要栅格化？这什么鬼？Google之！Boostrap！搞定，框架的甜头，快速的开发初步尝到！

第三份设计稿，我去！鼠标点击换图片，变颜色，图片还要自动滚动！这怎么做的！Google之！javascript!太复杂，javascript太难了，怎么破？Jquery！wow!

从此以后HTML+CSS用Boostrap布局，交互用Jquery代替原生javascript！还有什么搞不定的工作么！美滋滋中。。。

很长一段时间后。。。

移动端设计稿来了，适配，弹性布局，滑动。。。我去，还有这么多玩意，怎么适配？Boostrap和jquery都太过重了，Google之！flex-box布局，rem适配,flex-box兼容？CSS#动画兼容？PostCSS+gulp构建工具解放自己！

如此，一年过去了，有一天忽然想起来，难道布局自取依靠那么笨重的css框架吗？那么重型的js框架么，于是去编写自己通用的css逐渐，去用封装自己常用的js方法！一做起来吓一跳，封装出自己的第一个面向对象的分发，兴奋不急，然后发现自己的代码和别人的重视有差距，然后开始深入社区学习，井盖终于打开了！

想起来，真的是挺有意思的，说是工作，也可以是学习，感谢自己努力。


工作即修行。

### 关于学习

从始至终都是自己一个人摸索前进，痛苦并快乐吧。遇到一个又一个不会又难啃的问题，学到一个又一个知识的高兴，解决一个又一个自己遇到的问题的兴奋。


早前自己一直犯这样的错误：学习需要抽时间专心去学，学习的时候就该只学习，不该被打扰，导致早前除了周末学得比较多外，工作只是完全没意识到很多注释就是我自己的学习过程，那应该报道自己的博客来，那都是宝贵的经验和成长的烙印啊！

- 搜索引擎是最好的老师
- 人无所息 学无止境
- 学习不止眼前和工作，还有未来的星辰大海
- 工作中学习是最好的学习方法
- 学会使用搜索引擎，寻找资源的能力就是学习的能力
- 不会有武林高手带你飞，武功秘籍都是假的
- 别看！动手！

### 关于扎实基础与框架应用

最近知乎不太平，ng和vue撕逼好久了

其实对于前端来说，几乎所有的框架都是基于JS,JS才是王道！

坦白地将，直到最近把编程艺术和高级程序设计又重新过了一遍，以及重新整理了一遍之前对JS的原型、闭包、继承的知识后，才开始计划往后慢慢的集成Nodejs、React和Vue等框架到项目中去。重新过了一遍之前工作和学习的知识才发现，半年前跟风跟着做了一点的Vue，React，Node才发现，那是真是只求用上了就行了，一知半解甚至不求甚解的感觉，真是太着急太焦虑，当然，也不能说拒绝框架，实际工作项目中无论是基于需求还是开发效率，框架应用得好，合理，都是极其必要的。

### 关于计划

征程是星辰大海，扎实的基础，紧随时代步伐，司机也终于到了。

- 1.基于之前帮忙朋友的项目中使用了React，下一步将是先熟悉并在自己计划的项目以及空余的时间学习React，把React全家桶应用一遍
- 2.Vue和React有所区别但又相近，趁热打铁
- 使用Node做一个小型CMS系统，真正的学习Node，通往大前端之路


下一站，星辰大海！









































