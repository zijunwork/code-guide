#### 01、命名规范

1. 除特殊文件名外，文件名必须全部采用中划线命名法。e.g.: `global-methods.js`， `README.md`

2. 变量名全部采用驼峰命名法。e.g.: `isLogin`, `tableTitle`

3. 常量名全部采用大写字母下划线命名法。e.g.: `MAX_COUNT`, `BASE_URL`

4. 函数名全部采用驼峰命名法，并且前缀必须为动词。e.g.: `function getListData() {}`

   * 常用动词推荐：`can`， `is`, `has`, `get`, `set`, `load`, `open`, `close`, `jump`, `computed`

   * 触发为事件型动词推荐：`on`, `handle`

5. 类名全部采用pascal命名法。e.g.: `class Student{}`

6. 类中公共属性名全部采用驼峰命名法，私有属性全部采用下划线命名法。e.g.: `getName(){}`, `_name() {}`



#### 02、文档规范

1. 建议文件顶部写入文件信息注释。具体注释和其他注释可参照【[注释规范](/code-guide/comment?id=_04、文件文档注释)】



#### 03、常规语法规范

1. **推荐使用ES6+语法。**e.g.: `str.includes(“hello”)`

2. 变量声明，使用 `let` 代替 `var`

3. 字符串推荐使用单引号

4. 判断是否相等，使用 `===` / `!==` 代替 `==` / `!=`

5. 推荐短路运算替代 `if/else`

6. 推荐使用三元条件判断替代 `if/else` 逻辑处理（某些情况下）

7. 推荐使用 `switch/case`  替代 `if/else` 逻辑处理

8. 推荐使用 `for` 循环替换其他的循环语法

9. 推荐使用字符串模块替代字符串拼接

10. 推荐使用箭头函数替代老式函数语法

11. 函数的参数建议每个都有默认参数

12. 在只有单个导出的模块中，使用 `export defalult` 替代 `export`

13. jquery对象必须以 `$`开头命名

    

