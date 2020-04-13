#### 01、命名规范

1. html文件必须使用中划线命名法。e.g.: `login-store.html`
2. 标签名必须使用中划线命名法。e.g.: `<base-loading></base-loading>`
3. 属性名必须使用中划线命名法。e.g.: `<p style="max-width: 100px"></p>`



#### 02、文档规范

1. 建议文件顶部写入文件信息注释。具体注释可参照【[注释规范](/code-guide/comment?id=_04、文件文档注释)】
2. HTML5文档必须声明，避免浏览器开启怪异模式 `<!DOCTYPE html>`



#### 03、常规语法规范

1. 在属性中，必须全部使用双引号
2. 自动闭合标签，不要使用斜线
3. 引入资源使用相对路径，不要指定资源所带的具体协议（`http:` / `https`）
4. 尽量结构、表现、行为分离，HTML只做展示内容
5. 区块之间需要有注释和空行
6. 标签节点能少则少，避免多余的父节点



#### 04、属性顺序规范

此为建议项，不过有些编辑器的风格插件，e.g.: pritter 会自动优化属性顺序。为了就是保证代码的易读性。

1. `class`
2. `id`
3. `name`
4. `data-*`
5. `src`, `for`, `type`, `href`, `value`, `max-length`, `max`, `min`, `pattern`
6. `placeholder`, `title`, `alt`
7. `aria-*`, `role`
8. `reuqired`, `readonly`, `disabled` 

 