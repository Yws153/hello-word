# ModuleConcatenationPlugin

官方的说明是：https://cloud.tencent.com/developer/section/1477569
过去 webpack 打包时的一个取舍是将 bundle 中各个模块单独打包成闭包。
这些打包函数使你的 JavaScript 在浏览器中处理的更慢。
相比之下，一些工具像 Closure Compiler 和 RollupJS 可以提升(hoist)或者预编译所有模块到一个闭包中，提升你的代码在浏览器中的执行速度。
这个插件会在 webpack 中实现以上的预编译功能。
```
new webpack.optimize.ModuleConcatenationPlugin()
```
