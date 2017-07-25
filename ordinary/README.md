![screenshot.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-ordinary/master/screenshot.jpg)

「庸」(Ordinary)是一个平淡无奇的 Bitcron 主题，基本实现了所有功能。

## 特点

- 网站标题采用中国风的「王汉宗超明体」（仅作用于繁体字）；
- 支持 `分类` 和 `标签`；
- 归档页面包括 `归档` 和 `分类&标签` 目录；
- 支持网站颜色自定义（具体操作在后文说明）；
- 自适应页面，手机浏览体验佳；
- 可显示社交账号
- 优化了评论框
- 只有六个文件

## 安装设置

[下载](https://github.com/shuibaco/bitcron-theme-ordinary) template 文件夹，放入网站根目录下。

- **标题**：Dashboard → Site → Title / Sub Title
- **每页显示文章数**：Dashboard → Common → Posts Per Page
- **社交账号**：Dashboard → Common → Social ID
- **嵌套评论**：Dashboard → Render → Comments Type: Tree
- **菜单**：Dashboard → Navigation
- **网站相关图片**：Dashboard → Images
- **归档页面显示文章数**：archive.jade 第九行 `limit=30`
- **网站颜色自定义**：style.scss 第一行开始的 `Customize field`。
    + `$mcolor`：main color 主要颜色
    + `$pcolor`：point color 链接等
    + `$bgcolor`：background color 背景颜色
    + `$scolor`：second color 次于主要颜色的第二多被使用的颜色
    + `$tcolor`：text color 文字颜色

## 配色方案

### 奶昔 Yellow（默认）

```
$mcolor: #eee;
$pcolor: #ffbb00;
$bgcolor: #fffaf2;
$scolor: #bbb;
$tcolor: #888;
```

![yellow.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-ordinary/master/colours/yellow.jpg)

### 单色 Mono

```
$mcolor: #e1e8ef;
$pcolor: #3f4851;
$bgcolor: #fafafa;
$scolor: #aab7c4;
$tcolor: #8592a0;
```

![mono.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-ordinary/master/colours/mono.jpg)

### 夏日 Summer

```
$mcolor: #cae5c5;
$pcolor: #ff8b94;
$bgcolor: #fff7f2;
$scolor: #b7a9a3;
$tcolor: #7c6e66;
```

![summer.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-ordinary/master/colours/summer.jpg)

### 入夜 Night

```
$mcolor: #2d3547;
$pcolor: #c5c7d6;
$bgcolor: #030c21;
$scolor: #515466;
$tcolor: #7b7d91;
```

![night.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-ordinary/master/colours/night.jpg)

### 纯净 Pure

```
$mcolor: #f4f4f4;
$pcolor: #e2e2e2;
$bgcolor: #fdfdfd;
$scolor: #bcbbb8;
$tcolor: #a5a4a2;
```

![pure.jpg](https://raw.githubusercontent.com/shuibaco/bitcron-theme-ordinary/master/colours/pure.jpg)

## 支付宝赞助

![alipay.jpg](https://raw.githubusercontent.com/shuibaco/donate/master/alipay.jpg)