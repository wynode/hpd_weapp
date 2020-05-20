# wynode-wx

> A Mpvue project

## Build Setup

使用mpvue+vant+scss进行开发，进入目录cnpm install + npm dev即可。

不能使用微信开发者工具预览是因为/static/images/文件过大，代码已经使用网络源代替，请自行更换。请不要过度依赖本网络源（随时可能会没钱续费）。

``` bash
# 安装依赖
yarn

# 开发时构建
npm dev

# 打包构建
npm build

# 指定平台的开发时构建(微信、百度、头条、支付宝)
npm dev:wx
npm dev:swan
npm dev:tt
npm dev:my

# 指定平台的打包构建
npm build:wx
npm build:swan
npm build:tt
npm build:my

# 生成 bundle 分析报告
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
