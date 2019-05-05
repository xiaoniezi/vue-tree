# tree

> element-ui tree secondary development

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8088
npm run serve

# build for production with minification
npm run build

```

## 简单说明
elementUI ^2.2.0可以使用scoped slot的方式自定义节点，所以有两种方式，但原理都是一样。

## 展示地址
[click here][1]

## 更新说明

### 2019/04/17 
- `NODE_ID_START` 代替 `maxexpandId`，不用从后台获取
- `NODE_KEY`代替全局`id`
- 删除节点采用组件自带方法`remove`
- 使用scss

### 2019/04/26
- 删除.babelrc文件
- 更新展示地址：请求地址错误问题

[1]: https://xiaoniezi.github.io/projects/VueTree
