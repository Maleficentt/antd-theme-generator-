# antd-theme-generator 源码解读

`antd-theme-generator`只是针对于颜色的定制，对于其他属性例如字体大小，边框，边距等样式不提供定制

这里只针对`generateTheme`方法和其涉及到的方法进行讲解，其他的方法不予以讲解。官方文档有使用这个方法的例子，请参考：[https://github.com/mzohaibqc/antd-theme-generator](https://github.com/mzohaibqc/antd-theme-generator "antd-theme-generator")

## 参数
### options
* `antDir`: antd包目录，（`path.join(__dirname, './node_modules/antd')`）
* `antdStylesDir`: 可选，antd包目录，（`path.join(__dirname, './node_modules/antd/lib')`）
* `stylesDir`: 自己写的样式目录（后文统称自定义样式），（`path.join(__dirname, './src/styles')`）
* `mainLessFile`: 自定义样式入口文件，（`path.join(__dirname, './src/styles/index.less')`）
* `varFile`: 自定义样式入口文件，（`path.join(__dirname, './src/styles/index.less')`）
* `outputFilePath`: 输出less文件路径，（`path.join(__dirname, './src/styles/index.less')`）
