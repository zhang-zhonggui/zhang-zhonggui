---
title: 工作bug
date: 2023-05-29 23:31:09
tags: work
---

# 工作bug

<!--more-->

今天前后端传参数的时候一直报错。

```java
“Content type ‘application/json；charset=UTF-8‘ not supported”
```

1. 我猜到是参数类型有问题，但应为这个实体类嵌套的参数太多，真的找不到，一个下午差不多都在找那的参数出现了问题，最后实在找不到，只能，参数一个一个的注释掉，然后一点点添加，就这样，我终于发现问题了。但具体还是不知道那个参数有问题，又经行无休止的查询，

2. 最后让我熬到了下班还是没找到到，最后没办法回家，在家中讲报错的内容在网上发了一遍又一便最后发送有一个帖子上写着

   ```text
   日期属性为错误格式（Data），经改正为（Date），后测试传输顺利。同样问题可仔细检查自己的实体类属性值是否错误，比如“Date类型的实体类属性中,Date必须是Java.util.Date，不可以为Java.sql.Date”。
   ```

   让我觉得是不是我也出了这样的问题。

3. 果然，我就是这个错误。哎大意了，一个小错误差不多浪费我半天时间以后还是得更加的细心啊
