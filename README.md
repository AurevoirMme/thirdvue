# second-vue

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# 添加element components

npm i element-ui -S

# 安装组件后报错
问题已解决 步骤为：
1.cnpm install style-loader -D
2.cnpm install css-loader -D
3.cnpm install file-loader –D
4.安装cnpm install element-ui -S

5.在main.js中引入：

import ElementUI from ‘element-ui‘
import ‘element-ui/lib/theme-chalk/index.css‘
Vue.use(ElementUI)




# css中关联的字体没有被引用过来，缺少了引用字体的loader，加了楼上的webpack配置后，也许你还得装一个url-loader包

# wepack.config.js添加以下代码，重启

{
   test: /\.(eot|svg|ttf|woff|woff2)(\?\S*)?$/,
   loader: 'file-loader'
}


# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
