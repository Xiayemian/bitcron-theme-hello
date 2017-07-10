date: 2017-06-14 10:52 
title: 模板测试文本 Markdown
url: sample-content-markdown
tags: theme, work

**注意**：以下内容可能在 GitHub 和 Bitcron 中呈现不同的形式。最终效果以 Bitcron 为准。

---

换主题的时候常看到模板测试文本，于是拷贝了一份放在博客里，为了方便查看调试效果。这个测试文本由 html 写成，虽然内容涵盖广，但因为都是英文而且有些冗杂，我便打算用 Markdown 写一个**更适合我自己**的精简版。

## 这是二级标题

二级标题通常用于文章内部的结构梳理，除此之外还有三级至六级标题[^1]。而一级标题一般情况下会是文章标题，所以文章内部最好不要使用一级标题，以防与文章标题重叠，产生不美观的结构。

### 这是三级标题

二级标题所描述的内容中，若还需要细分，可以使用三级标题，甚至四级标题。

#### 这是四级标题

一般来说我只使用二级和三级标题，能用到四级标题的情况非常少，更别说五级和六级标题了。如果开启了 TOC 功能，这些级别的标题就会自动生成目录，显示在页面的某处，方便读者快速掌握文章脉络和跳步阅读。

## 图片

如果说博客中最常见的是文字（段落），那么第二重要的应该要数图片了。成语里有个词叫做“图文并茂”，看来非常有必要测试一下图片的显示样式了。

### 通常写法

```
![这是 alt](/test-photo.jpg '这是可写可不写的 title')
```

![这是 alt](/test-photo.jpg '这是可写可不写的 title')

### figure 写法

```html
<figure>
	<img src="/test-photo.jpg" alt="这是 alt" />
	<figcaption>这是可写可不写的 figcaption</figcaption>
</figure>
```

<figure>
	<img src="/test-photo.jpg" alt="这是 alt" />
	<figcaption>这是可写可不写的 figcaption</figcaption>
</figure>

来看看 w3schools 是如何定义 `figure` 和 `figcaption` 的。

> The &lt;figure&gt; tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.
> The &lt;figcaption&gt; tag defines a caption for a &lt;figure&gt; element.
> [-- *w3school*]]

由于 figure 写法在 css 上更有发挥空间，加上 `figcaption` 的助攻，让图片显示更加友好，所以再很早之前我就全部统一为这种写法[^2]。

## 表格

```table
标题一 | 标题二 | 标题三
1.1 | 1.2 | 1.3
2.1 | 2.2
3.1 | | 3.3
```

更多 Bitcron 中的表格技巧请查看[「关于 Bitcron 表格的各种」](http://blog.shuiba.co/about-bitcron-table)。

## 列表

这是一个无序列表

- 项目
- 项目
- 项目

---

这是一个有序列表

1. 项目一
2. 项目二
3. 项目三

---

这是一个 to-do list

- [x] 已完成
- [ ] 未完成
- [ ] 未完成

所有我想要测试的效果都包含在上文中了，其中包括了 header/link/img/footnotes/hr/code/pre code/blockquote/bold/italic/table/list/toc。


[^1]: 五级标题和六级标题并不常用。
[^2]: 由于 `title=""` 可写可不写，所以在有 `figcaption` 的情况下完全被我省略了。如果写了 `title=""`，默认样式是鼠标悬停图片时看到的说明。