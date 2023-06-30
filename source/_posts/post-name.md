---
​---
title: Hello World
date: 2013/7/13 20:46:25
typora-root-url:post-name
​---
---

## 使用 Markdown 嵌入图片

[hexo-renderer-marked](https://github.com/hexojs/hexo-renderer-marked) 3.1.0 引入了一个新的选项，其允许你无需使用 `asset_img` 标签插件就可以在 markdown 中嵌入图片

如需启用：

```
_config.ymlpost_asset_folder: true
marked:
  prependRoot: true
  postAsset: true
```

启用后，资源图片将会被自动解析为其对应文章的路径。
例如： `image.jpg` 位置为 `/2020/01/02/foo/image.jpg` ，这表示它是 `/2020/01/02/foo/` 文章的一张资源图片， `![](image.jpg)` 将会被解析为 `<img src ="/2020/01/02/foo/image.jpg">` 。

```text
typora-root-url:
```

```
---
title: Hello World
date: 2013/7/13 20:46:25
---
```

![image-20230630201850715](/image-20230630201850715.png)
