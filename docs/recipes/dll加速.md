# dll 加速

## usage

```
yarn install @qnpm/poi-preset-dll --dev
```

```javascript
var options =  {
  require('@qnpm/poi-preset-dll')({
    dllVendor: [
      'vue',
      'vue-router',
      'vue-stash',
      'axios',
      'bluebird',
      '@qnpm/iview'
    ]
  })
}
```

```
# 生产环境dll编译
NODE_ENV=production poi dll
# 开发环境dll编译
NODE_ENV=development poi dll
```

## 参考文档

参考 [https://webpack.js.org/plugins/dll-plugin/](https://webpack.js.org/plugins/dll-plugin/)