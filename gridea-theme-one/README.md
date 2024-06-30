# Gridea-theme-One-Pro

一款简洁专注于写作的 Gridea 博客主题，示例网站：<https://daoxi365.gituhb.io>。

修改自[Gridea-theme-one]([kytrun - Codeberg.org](https://codeberg.org/kytrun/gridea-theme-one))。

## `Gridea-theme-One` 的特点

- 基于 Zero 适配手机页面，精简依赖，添加更多自定义功能
- 增加 [搜索功能](https://github.com/kytrun/gridea-search)

## `Gridea-theme-Pro` 的特点和改动

|      局限性      |                           具体内容                           |
| :--------------: | :----------------------------------------------------------: |
|       全局       |                 修复 `font-awesome` 适配问题                 |
|   `index.ejs`    |       第一次进入网站时右上角弹窗（基于 cookies 实现）        |
|       全局       |                      引入 $\LaTeX$ 支持                      |
|    `post.ejs`    |                         添加代码高亮                         |
|       全局       | 引入 `Google Fonts`（引入的是某种宋体和 Ubuntu 西文字体）；  |
|   `header.ejs`   |         丰富 `headers` 的链接（当然需要您自行调节）          |
| `post-list.ejs`  |                         添加封面支持                         |
| `pagination.ejs` |                     修改切换上下页的文字                     |
|    `post.ejs`    |          文章图片居中显示；图片圆角化；图片点击放大          |
|       全局       |                       添加鼠标点击特效                       |
|    `post.ejs`    |          添加监听器，使跳出页面时标题和图标发生改变          |
|       全局       |                        引入不蒜子统计                        |
|       全局       | 通过 `colorfulbg_bright.min.js` 实现渐变背景色（详见 [ColorfulBG](https://github.com/pandaoxi/colorfulbg)） |
|    `post.ejs`    |            自定义表情、`placeholder`、提示文字等             |
|   `main.less`    |                        少量的样式修改                        |
|    `404.html`    |             崭新的 404 页面（建议自行修改一下）              |

## 安装方法

- 克隆项目到本地；
- 复制此目录到 `Gridea` 主题文件夹 `themes` 中；
- 重启 Gridea 客户端；
- 在主题中选择 `One Pro` 主题，点击保存；
- 预览查看效果；

## 注意事项

-   不建议在 Gridea 软件内进行自定义设置；
-   务必检查仓库内所有文件，把有关原来「daoxi365」的内容替换为您的博客；
-   建议修改网站描述（Gridea 左侧栏 → 主题 → 基础配置 → 网站描述）：

```html
<p><b>温和中坚持，宁静中创新。</b></p><br>
<p>本站总访问次数：<b id="busuanzi_value_site_pv">0</b>次</p>
<p>本站总访客数：<b id="busuanzi_value_site_uv">0</b>人</p>
<script async src="//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script><br>
<p>Copyright 2022-<span id="currentYear"></span> by <b>PanDaoxi</b>.</p><p>All rights reserved.</p>
<script>
document.addEventListener('DOMContentLoaded', () => {
var date = new Date();
document.getElementById("currentYear").innerHTML = date.getFullYear();
});
</script>
```

这是我主题设置的内容，仅供参考。
