使用的打包工具是 `gulp 3.8.10+`，脚本命令如下：

```js
{
    scripts: {
        start: 'gulp -ws',
        test: 'gulp release'
    }
}
```

`-ws` 的含义在 `gulpfile.js` 中有说明：

```js
// -w: 实时监听
// -s: 启动服务器
```