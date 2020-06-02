# xmgmail

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```


笔记：     ①②③④⑤⑥⑦⑧⑨⑩
一、划分目录结构。
二、配置vue.config.js。
三、创建底部tabar栏。
    将封装好的tarbar引入到项目中：
      1、将相应的文件放入相应的目录中
      2、在App.vue中注册组件（分三步：import，components，<main-tab-bar></main-tab-bar>）
      3、配置路由：
        ①、未安装进行路由安装：（npm install vue-router --save）
        ②、在main.js中引入router：（import router from './router'）
        ③、在路由中配置index.js
四、修改底部tabar颜色，默认为红色。
    <tab-bar-item link="/home">
    <!-- <tab-bar-item path="/home" activeColor="green"> 修改底部tabar颜色，默认为红色-->
五、修改logo.png(即：favicon.ico):
    1、将原有的图片替换掉.
    2、在index.html中修改将 favicon.ico 改为 logo.png
六、首页布局。
    1、顶部“购物街”封装成通用组件，使用具名插槽。
      分成三部分left、center、right，各部分进行使用时对应名字使用即可。通用样式可以在封装好的通用组件中进行样式编写，不同样式在各自文件中进行编写。
    2、请求网络数据。
      ①、未安装axios进行安装：npm install axios --save
      ②、封装network中axios.js  （程序开发顺序：①、先进行网络数据请求，②、创建对应标签及元素、③、将请求的数据进行展示）

