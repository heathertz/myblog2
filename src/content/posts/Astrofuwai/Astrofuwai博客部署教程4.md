---
title: Astro/test3
published: 2025-08-23
description: 新博自己的博客
tags: [博客教程]
category: 教程
draft: false 
pinned: true
---

# Astro/test3

## 前言

新博客站点部署也有2周多时间了，新站的访问量不是很多，但是我发现有人是用我的[fuwai_zyplj](https://github.com/ZyPLJ/fuwai_zyplj)仓库去修改配置然后再部署自己的博客，因为我个人喜欢对博客乱改，所以我这边出一个教程，来讲讲如何部署和我一样的博客。

<font color='red'>本篇文章重点讲解博客配置！！！</font>

为了方便大家使用我的仓库，我特意将原本的仓库改为私有，新建了一个公共的仓库，包括不限于没有我的文章、其他第三方配置。

我的博客只是在原作者[fuwari](https://github.com/saicaca/fuwari)仓库的基础上增加了：

1. 音乐播放器
2. 文章置顶固定（原作者仓库PR中的）
3. 评论系统
4. 友链页面
5. 首图支持视频

如果对于上述功能不感兴趣的可以直接`clone`原作者的仓库。

## 页面基础配置

大部分页面配置都在`src/config.ts`文件中完成,大部分配置都有注释。重点讲解我添加的配置。

### banner图换成视频

将`type`设置为`video`，然后将`src`指向视频`MP4`格式的视频文件，注意视频文件放在 `public/videos/` 目录下。

```ts
banner: {
    enable: true,
    src: "assets/images/banner.jpg", // Relative to the /src directory. Relative to the /public directory if it starts with '/'
    // 如果要使用MP4视频，可以这样配置：
    // src: "/videos/banner-video.mp4", // 视频文件放在 public/videos/ 目录下
    // type: "video", // 设置为视频类型
    position: "center", // Equivalent to object-position, only supports 'top', 'center', 'bottom'. 'center' by default
    type: "image", // Support 'image' or 'video' format
    credit: {
        enable: false, // Display the credit text of the banner image
        text: "", // Credit text to be displayed
        url: "", // (Optional) URL link to the original artwork or artist's page
    },
},
```

### Microsoft Clarity 分析

`Microsoft Clarity`是微软提供的用于网站流量分析的工具，如果用不上改成false即可，如果想用就需要去官网注册个账号：<https://clarity.microsoft.com/>

```ts
clarity: {
    enable: false, // 是否启用 Microsoft Clarity 分析
    projectId: "", // Clarity 项目 ID
},
```
