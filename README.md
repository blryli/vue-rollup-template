# vue-rollup-component-template

下载即可开始组件开发

> webpack3+babek6版本，如果需要webpck4+babel7版本请 clone webpck4-babel7分支

- [文档](https://juejin.im/post/5d255c566fb9a07eac05fbd8)

- [展示](https://blryli.github.io/vue-rollup-component-template/)

## 组件开发

#### 运行

根目录下

```js
npm i
npm run dev
npm run build
npm run build:es
npm run build:browser
npm run build:umd
```

> dev运行的是 rollup watch，监听src文件夹的变化，实时打包插件

#### 开发

只需要关注src目录，.babelrc文件设置了src目录为root

src目录下的模块引入，不需要'../../'

```js
import Component from 'components/component'
import util from 'utils/util'
import mixins from 'mixins/mixin'
...
```

#### 打包

dist 输出文件

- vue-rollup-component-template.css
- vue-rollup-component-template.esm.js
- vue-rollup-component-template.min.js
- vue-rollup-component-template.umd.js

## docs

#### 运行

> docs目录下

```js
npm i
npm run dev
npm run build
```
> 入口文件是组件打包后的js，运行时自动监听入口文件的变化，实时响应

## why

这样开发组件的好处是，组件开发与测试解耦，专注组件开发，开发完成快速发布
