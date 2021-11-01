# Vite+vue3+element-plus的demo项目

Vite官网：[https://cn.vitejs.dev/guide/#scaffolding-your-first-vite-project](https://cn.vitejs.dev/guide/#scaffolding-your-first-vite-project)

Element-Plus官网：[https://element-plus.gitee.io/en-US/guide/quickstart.html](https://element-plus.gitee.io/en-US/guide/quickstart.html)
### 1.安装element-plus
```javascript
npm install element-plus --save
```
### 2.安装按需自动导入element-plus依赖的插件
```javascrip
npm install unplugin-vue-components
```
### 3.配置vite.config.js文件
```javascrip
// vite.config.ts
import Components from 'unplugin-vue-components/vite'
import { ElementPlusResolver } from 'unplugin-vue-components/resolvers'

export default {
  plugins: [
    // ...
    Components({
      resolvers: [ElementPlusResolver()],
    }),
  ],
}
```
