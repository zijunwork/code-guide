#### 01、多单词常用命名方式

1. 驼峰（camel）命名法。e.g.: `thisIsAnApple`
2. 帕斯卡（pascal）命名法。e.g.: `ThisIsAnApple`
3. 下划线命名法。e.g.: `this_is_an_apple`
4. 中划线命名法。e.g.: `this-is-an-apple`（参照Github众多前端开源项目，本规范将推荐此命名法）



#### 02、项目命名

全部采用中划线方式，多单词以下划线命名。

e.g.: `my-blog`



#### 03、目录命名

1. 有复数结构时，采用复数命名法。

   e.g.: `utils`, `styles`, `images`, `views`, `components`, `assets`

2. 全部采用中划线命名法。

   比如，在vue项目中，不管是public静态目录下还是webpack打包文件目录。

   e.g.: `static-images`, `static-json`，`global-styles`

   

#### 04、html文件命名

如果有多个单词，全部采用中划线命名法。

e.g.: `login-home.html`



#### 05、css文件命名

如果有多个单词，全部采用中划线命名法。

e.g.: `element-ui.scss`, `global-variables.scss`



#### 06、javascript文件命名

如果有多个单词，全部采用中划线命名法。

e.g.: `global-methods.js`, `global-const.js`



#### 07、vue文件命名

vue文件，如果有多个单词，全部采用pascal命名法。

e.g.: `MyComponent.vue`, `BaseButton.vue`

**需要注意的是：**

+ 基础组件文件。也就是样式类的，无逻辑，或无状态的组件。全部以一个特定的前缀开头。

  e.g.：`Base`, `App`, `V`, `C `等。

+ 单例组件文件。无数据交互的，每个页面只可能使用一次的，单例组件不接受任何 `prop`。组件名必须以 `The` 前缀命名。

  e.g.: `TheHeading.vue`, `TheSidebar.vue` 等。

+ 紧密耦合组件文件。子组件命名必须以父组件名作为前缀命名。

  e.g.: `TodoList.vue`, `TodoListItem.vue`, `TodoListItemButton.vue`

  

#### 08、markdow文件命名

如果有多个单词，全部采用中划线命名法。

e.g.: `code-guide.md`, `dev-document.md`



#### 09、图片命名

如果有多个单词，全部采用下划线命名法。

e.g.: `icon_avatar.jpg`, `defalut_bg.png`

