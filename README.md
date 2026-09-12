# zloct 的博客

基于 [Hexo](https://hexo.io/) + [Butterfly](https://github.com/jerryc127/hexo-theme-butterfly) 主题，托管在 GitHub Pages。

线上地址：**https://zloct.github.io**

## 写新文章

```bash
hexo new post "文章标题"   # 会在 source/_posts/ 下生成 Markdown 文件
```

编辑完成后推送，GitHub Actions 会自动构建并发布（约 1~2 分钟生效）：

```bash
git add -A && git commit -m "post: 文章标题" && git push
```

## 本地预览

```bash
npm install --legacy-peer-deps   # 首次克隆后执行一次
npx hexo server                  # 打开 http://localhost:4000
```

## 常用操作

- `npx hexo clean`：清理构建缓存，页面显示异常时先执行这个再重新生成
- 主题美化：在根目录新建 `_config.butterfly.yml` 覆盖主题默认配置，参考 [Butterfly 文档](https://butterfly.js.org/)
- 站点信息（标题、头像、菜单等）在 `_config.yml` 的 Site 部分
