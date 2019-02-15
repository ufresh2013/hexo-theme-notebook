# hexo-theme-notebook

A pure theme put your articles in order.

[Demo](https://ufresh2013.github.io/)


### 安装
```
git clone https://github.com/ufresh2013/hexo-theme-notebook.git
npm install
```
修改根目录下的`_config.yml`内的`theme`值为`hexo-theme-notebook`
<br/>


### 文章声明
文章列表根据category分类，**每篇文章都要加上`category`**，且只写一个值
```markdown
  ---
  title: ES6参考手册
  date: 2016-12-23 16:08:28
  category:
  - 前端
  ---
```
<br/>

### 搜索
#### 1. 安装插件
在根目录下安装
```
npm install hexo-generator-tag --save-dev
npm install hexo-generator-search --save-dev
```

#### 2. 添加页面
手动在/source下创建目录和index.md文件
```
├── source
|      └── _posts
|      └── about
|            └── index.md
|      └── search
|            └── index.md
|      └── favicon.ico
```

/source/about/index.md
```
---
title: Search
layout: page
type: search
---
```

#### 3. 生成搜索文件
```
hexo g
```
<br/>




