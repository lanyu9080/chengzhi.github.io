# 我的博客 — 文件说明

## 📁 文件结构

```
我的博客/
├── blog.html       ← 博客主页面（不需要改）
├── articles.js     ← 所有文章数据（只需要改这个！）
└── README.md       ← 本说明文件
```

## ✍️ 如何新增文章

打开 `articles.js`，在最顶部的注释下面，数组最前面粘贴以下模板：

```javascript
{
  id: 6,                          // 每次 +1，不能重复
  cat: '随笔',                    // 分类：随笔 / 读书 / 摄影 / 思考
  date: '2025-06-01',             // 日期格式固定
  title: '这里写文章标题',
  excerpt: '这里写首页显示的摘要，60~100字左右。',
  tags: ['标签1', '标签2'],
  content: `
    <p>正文第一段。</p>
    <h2>小标题</h2>
    <p>正文第二段。</p>
    <blockquote>这里写引用的句子。</blockquote>
    <p>正文第三段。</p>
  `
},
```

## 🌐 如何打开博客

```bash
# 方式一：直接双击 blog.html（用浏览器打开）

# 方式二：终端打开
start D:\我的博客\blog.html

# 方式三：VS Code 编辑
code D:\我的博客
```

## ⚠️ 注意事项

- `blog.html` 和 `articles.js` 必须在同一个文件夹里
- 用浏览器直接打开 HTML 文件时，由于安全限制，部分浏览器可能不加载外部 JS
  → 推荐用 VS Code 安装 **Live Server** 插件来预览
  → 或者用 Chrome 并允许本地文件访问

