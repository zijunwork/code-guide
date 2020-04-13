#### 01、命名规范

1. css/scss/sass/less文件必须使用中划线命名法。e.g.: `meida-item.css`
2. 选择器必须使用中划线命名法。e.g.: `.part1-title`
3. 使用语义化、通用化的方式命名



#### 02、文档规范

1. 建议文件顶部写入文件信息注释。具体注释可参照【[注释规范](/code-guide/comment?id=_04、文件文档注释)】
2. 区块之间建议加入区块注释（注意不要使用行注释）和空格，增强代码的可读性



#### 03、常规语法规范

1. 样式层级嵌套不能太深，不要超过3层
2. `class` 和 `id` 避免叠加使用
3. 每个声明都应该用分号结束，保证一致性和可扩展性
4. 需要用到引号，必须优先使用双引号
5. 样式属性 `：` 后面必须要有一个空格。e.g.: `background-color: rgba(0, 0, 0, .5);`
6. 颜色属性如果是16进制，全部采用小写，且能简写就简写。e.g.: `color: #33c;`
7. 小于1的小数，必须去掉点前面的0。e.g.: `opcity: .5;`
8. 避免为0值指定单位。e.g.: `margin: 0;`
9. 多个属性共用一个通用属性（即以 `,` 分割的属性值），必须换行对齐
10. 无前缀的属性必须写在有前缀的属性前面
11. 直接子选择器优先后代选择器。e.g.: `.content > .title{}`



#### 04、属性顺序规范

必须遵循： 结构性属性 > 表现性属性 > 其他属性

1. 结构性属性
   1. 定位。`position`, `top`, `right`, `left`, `z-index`
   2. 盒模型。`display`, `box-sizing`, `width`, `height`, `padding`, `marigin`, `border`, `overflow`
2. 表现性属性
   1. 字体。`font-size`, `line-height`, `test-align`
   2. 颜色。`color`, `background-color`, `opacity`
3. 其他属性
   1. e.g.: `user-select`, `cursor`