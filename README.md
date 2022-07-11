# swc-transform-import 插件

效果同 [babel-plugin-transform-imports](https://www.npmjs.com/package/babel-plugin-transform-imports)

代码抽取自 [EMP Compile SWC](https://github.com/efoxTeam/emp/tree/next/packages/compile-swc)

## 安装
```sh
npm i swc-transform-import -D
# or
pnpm add swc-transform-import -D
```

## 配置

> .swcrc
```js
'plugin': m => new PluginTransformImport({
        antd: {
            transform: 'antd/es/${member}',
            style: true,
        },
    }).visitProgram(m);
},
```
