![screenshot.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-hello/master/screenshot.jpg)

# 简介

「你好呀」(Hello)是一个定位简洁的 Bitcron 主题。没有分类和标签页面，初始网站地图如下所示：

```
|-- 首页 / (+最新文章 +分类目录)
	|-- 归档 /archive (所有文章)
	|-- 订阅 /feed
	|-- 404 /404 (找不到该页面)
```

# 设置

- **标题**：Dashboard → Site：大标题对应 Title；小标题对应 Sub Title
- **菜单**：Dashboard → Navigation
- **关于页面**：新建文件名为 `about.md`，放在根目录下
- **各种头像**：Dashboard → Images：favicon 对应 Site Favicon [.ico]；网站头像对应 Site Avatar；评论者头像对应 Visitor Avatar……等等
- **最新文章数**：index.jade 第29行 `posts.get_recent(10)`
- **归档页面显示文章数**：archive.jade 第12行 `limit=30`
- **各分类页面显示文章数**：category.jade 第7行 `+posts.set_min_per_page(30)`
- **搜索页面显示文章数**：result.jade 第12行 `limit=30`
- **point colour**：style.scss 第2行 `$pcolour: #ff0000;`

其他跟主题无关但我常用到的配置（以下内容全部在 Dashboard 中设置）。

- **Common**
	- **Show TOC**：是否显示 TOC (Table of content)。如果文章有多级标题，可以自动生成目录。
	- **Hide Post Prefix URL**：是否隐藏 post 前缀。选 yes 则 `domain.com/title`;选 no 则 `domain.com/post/title`。
- **Render**
	- **Force SSL**：是否强制 SSL。
	- **Hide Comments**： 是否隐藏评论。
- **Advanced**
	- **Admin Name**：管理者名字。如果网站名称和管理者名字不同，填写此项有助于在 RSS 订阅器中有较好的呈现。比如 Feedly 中会显示 `网站名 / by 管理者名 / 时间`。
	- **Anti Theft Chain**：是否防盗链。
