---
title: hexo创建文件自动打开
date: 2023-02-04 20:40:53
tags: 黑科技
categories: 科技分享给
---



## 如何在hexo创建新post文档之后自动打开

```
hexo n "The title of your blog"
```

这个指令可以快速创建

### 实现创建后自动打开

1. 新建`scripts`目录（hexo根目录）

2. 创建`auto_open.js`文件,如下

   ```
   
   var spawn = require('child_process').exec;
   hexo.on('new', function(data){
     spawn('start  "C:\Program Files\Typora\Typora.exe" ' + data.path);
   });
   ```

   

路径设置为你的软件路径即可
