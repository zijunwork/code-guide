#### 01、命名规范

1. vue文件，如果有多个单词，全部采用pascal命名法。e.g.: `MyComponent.vue`, `BaseButton.vue`

2. 基础组件文件。也就是样式类的，无逻辑，或无状态的组件。全部以一个特定的前缀开头。e.g.：`Base`, `App`, `V`, `C `

3. 单例组件文件。无数据交互的，每个页面只可能使用一次的，单例组件不接受任何 `prop`。组件名必须以 `The` 前缀命名。e.g.: `TheHeading.vue`, `TheSidebar.vue` 

4. 紧密耦合组件文件。子组件命名必须以父组件名作为前缀命名。e.g.: `TodoList.vue`, `TodoListItem.vue`, `TodoListItemButton.vue`

5. 公共组件与页面组件 `class` 名必须加以区分。e.g.: `<div class="view-login"></div>`, `<div class="component-btn"></div>`

6. `props` 、 `data` 中变量名，全部采用驼峰命名法。e.g.: `tableData`, `titleText`

7. `computed` 、`methods`、`watch` 中的方法名，全部采用驼峰命名法。e.g.: `getTableList(){}`

8. 函数名全部采用驼峰命名法，并且前缀必须为动词。e.g.: `function getListData() {}`

   * 常用动词推荐：`can`， `is`, `has`, `get`, `set`, `load`, `open`, `close`, `jump`, `computed`

   * 触发为事件型动词推荐：`on`, `handle`

   

#### 02、注释规范

1. 建议文件顶部写入文件信息注释。具体注释和其他注释可参照【[注释规范](/code-guide/comment?id=_04、文件文档注释)】
2. 公共组件必须要注释使用说明
3. 复杂的业务逻辑处理必须注释说明



#### 03、语法规范

1. `template` 中组件标签渲染必须采用中划线形式

2. `template` 中模块之间建议注释处理

3. `template` 中建议不要写死数据，建议用变量替代，数据写在 `data` 中

4. `template` 中多个属性建议换行处理，增强可读性

5. `template` 中如果涉及复杂的逻辑表达式，必须放入 `computed` 或者 `methods` 中，以函数形式 `return` 给出

6. `template` 中涉及引号，必须全部优先使用双引号。e.g.: `<app-title :style="{ width: titleWidth + 'px' }"></app-title>`

7. `v-for` 和 `:key` 必须配合使用

8. `v-if`` 和 `v-for` 不能同时用在同一个元素上

9. ``props` 中数据必须采用详尽模式。

   ```javascript
   props: {
       status: {
           type: String | Number,
           required: true,
           default: 0
       }
   }
   ```

10. 必须使用字符串模块来进行字符串拼接

11. vuex中 `mutation` 和 `action` 的函数名称必须放在 `types`里面统一声明

12. 公共组件统一放在 components 文件夹下

13. 公共方法、全局常量、请求封装、分享封装放在 utils 文件夹下

14. 路由模块必须工程化处理，自动化导入，精简代码

15. 页面组件的样式/公众组件的样式/全局的样式，推荐单独放置到 styles 文件下内

16. 静态文件统一放在 assets 文件夹下，需要绝对路径的静态文件统一放到 public 文件夹下

17. 接口文件统一方法 api 文件夹下

18. 特殊常量（api地址、微信appID等）统一放在 .env 环境配置中



#### 04、组件选项顺序规范

1. `name: `
2. `components: {}`
3. `props: {}`
4. `data(){}`
5. `computed: {}`
6. `created() {}`
7. `mounted() {}`
8. `methods: {}`
9. `watch: {}`

