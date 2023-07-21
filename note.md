### Vue3 notes

#### 源码
> https://unpkg.com/vue@3.3.4/dist/vue.global.js

#### 组成
- Vue对象
```javascript
  <script> 
    Vue.createApp({
        data() {
            return {
                x: "Mike" // 状态
            }
        }
    }).mount("#app")
  </script>
```
- HTML挂载到vue的锚点，#id
- Vue的语法， v-if, v-for, v-model...用于vue和DOM进行交互
- {{ }} 数据响应，数据绑定，vue来进行解析和渲染动态数据
- data, 处理data的方法
- Vue本质在High-Level操作DOM，大部分通过vue指令完成的

#### Vue指令
- vue不支持js语句，因为v-if提供了指令
- v-bind对于数据进行绑定，可以绑定属性，动态改变属性