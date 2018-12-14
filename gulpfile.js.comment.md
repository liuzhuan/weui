## yargs ^1.3.3

[yargs](https://github.com/yargs/yargs) 是一个命令行解析库。定义了如下三个选项：

1. `-w`, `--watch` 实时监听
2. `-s`, `--server` 开启服务器
3. `-p`, `--port` 端口号

## 任务

1. `build:style`，将 `weui.less` 编译压缩后，输出到 `dist/`
2. `build:example:assets` 将图片和脚本资源拷贝到 `dist/`
3. `build:example:style` 将样例的样式编译压缩后，输出到 `dist/`
4. `build:example:html` 将多个 HTML 片段合并，然后输出到 `dist/`
5. `build:example` 上面三个任务的大联合
6. `release` 综合 `build:style` 和 `build:example`
7. `watch` 监听本地文件
8. `server` 开启本地服务器
9. `default` 默认任务

## gulp-sourcemaps

[gulp-sourcemaps](https://www.npmjs.com/package/gulp-sourcemaps) 用来注入代码映射，以 `init()` 开始，`write()` 结束，默认是內联注入。

## gulp-less ^3.0.2

[gulp-less](https://www.npmjs.com/package/gulp-less)，用来编译 less 文件。

## gulp-postcss ^6.0.1

[gulp-postcss](https://www.npmjs.com/package/gulp-postcss)，用来增加浏览器前缀和删除注释。使用了 [`autoprefixer`](https://www.npmjs.com/package/autoprefixer) 和 [`postcss-discard-comments`](https://www.npmjs.com/package/postcss-discard-comments) 两个插件。

## gulp-header ^1.7.1

[gulp-header](https://www.npmjs.com/package/gulp-header) 用来插入头部版权信息。

## browser-sync ^2.9.11

[browser-sync](https://github.com/BrowserSync/browser-sync/tree/v2.9.11) 用来自动刷新页面。[Browsersync options](https://browsersync.io/docs/options) 列出了目前可用选项。

## gulp-cssnano ^2.0.0

[gulp-cssnano](https://www.npmjs.com/package/gulp-cssnano) 用来压缩 CSS 文件。通过将 [autoprefixer](https://cssnano.co/optimisations/autoprefixer) 和 [zindex](https://cssnano.co/optimisations/zindex) 设定为 `false`，减少不必要的不兼容风险。

## gulp-rename ^1.2.2

[gulp-rename](https://www.npmjs.com/package/gulp-rename) 用来重命名文件，给文件名中增加 `.min` 后缀。

## gulp-tap ^0.1.3

[gulp-tap](https://github.com/geejs/gulp-tap)，用于修改文件内容。在这里，将 `<link rel="import" href="xxx">` 替换为相应 html 文件的文本内容，并且包含在 `<script type="text/html" id="tpl_xxx"></script>` 之中。