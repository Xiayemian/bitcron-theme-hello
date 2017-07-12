![screenshot.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-hello/master/screenshot.jpg)

# 简介

「你好呀」(Hello)是一个定位简洁的 Bitcron 主题。没有分类和标签页面，初始网站地图如下所示。配色方面用的是最简单的黑白灰，point colour 是红色。评论部分也做了相应调整，欢迎测试。

```
|-- 首页 / (+最新文章 +分类目录)
	|-- 归档 /archive (所有文章)
	|-- 订阅 /feed
	|-- 404 /404 (找不到该页面)
```

# 安装配置

从[码仓](https://github.com/shuibaco/bitcron-theme-hello)下载 template 文件夹，解压后放入根目录中。正确形式应为 `根目录/template/index.jade`。

## 基本

- **标题**：Dashboard → Site。大标题对应 Title；小标题对应 Sub Title。
- **菜单**：Dashboard → Navigation。
- **关于页面**：新建文件名为 `about.md`，放在根目录下。
- **网站 logo**：Dashboard → Images。favicon 对应 Site Favicon [.ico]；网站头像对应 Site Avatar。
- **评论区头像**：Dashboard → Images。网站管理员头像对应 Admin Avatar；评论者头像对应 Visitor Avatar。另外关于在其他 Bitcron 网站中留言时显示的头像，需要在 bitcron.com → Account → Setup 中设置。
- **评论区使用 Gravatar 头像**：Dashboard → Render → Use Gravatar for Visitors: Yes。
- **评论邮件通知**：bitcron.com → Bicron Mail，新建邮箱后关联相应网站。

## 进阶

- **最新文章数**：index.jade 第29行 `posts.get_recent(10)`
- **归档页面显示文章数**：archive.jade 第12行 `limit=30`
- **各分类页面显示文章数**：category.jade 第7行 `+posts.set_min_per_page(30)`
- **搜索页面显示文章数**：result.jade 第12行 `limit=30`
- **point colour**：style.scss 第2行 `$pcolour: #ff0000;`
- **图片样式**：使用以下代码插入图片则拥有100%宽度。更多请参考[「模板测试文本 Markdown」](/sample-content-markdown)。

```html
<figure>
	<img src="图片地址" alt="对应文字说明" />
	<figcaption>描述</figcaption>
</figure>
```

## 推荐

- **显示文章目录**：Dashboard → Common → Show TOC: Yes。如果文章有多级标题，可以自动生成目录。
- **优化文章 URL**：Dashboard → Common → Hide Post Prefix URL。选 Yes 则 `domain.com/title`;选 No 则 `domain.com/post/title`。
- **开启 SSL**：Dashboard → Render → Force SSL: Yes。
- **评论嵌套**：Dashboard → Render → Comments Type: Tree。
- **设置管理者名字**：Dashboard → Advanced → Admin Name。如果网站名称和管理者名字不同，填写此项有助于在 RSS 订阅器中有较好的呈现。比如 Feedly 中会显示 `网站名 / by 管理者名 / 时间`。
- **图片防盗链**：Dashboard → Advanced → Anti Hotlinking: Yes。

# 更新日志

2017-06-09 发布主题
2017-06-11 首页增加自定义链接模块。示例：友情链接
2017-07-10 修改角标样式；修改“返回页首”按钮样式；修改评论框样式
2017-07-12 修改评论嵌套样式
