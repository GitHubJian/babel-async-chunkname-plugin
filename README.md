# babel-async-chunkname-plugin

检测 `import()` 异步引入的 vue 模块是否存在 webpackChunkName 标记

## 安装

```sh
npm i babel-async-chunkname-plugin -D
```

## 使用

```js
// .babel.config.js
module.exports = {
    plugins: [
        [
            require.resolve('babel-async-chunkname-plugin'),
            {
                // component: () => import(p)
                replace: function (p) {
                    return p;
                },
            },
        ],
    ],
};
```
