#### 01、Git提交规范作用

1. 修改文档、调整代码结构、性能优化，代码重构等信息一目了然
2. 提高合作开发的效率
3. 便于codereview及后续查阅、版本发布
4. 便于对自己的开发工作快速总结



#### 02、提交消息格式规范

Commit message 一般包括三部分：标题(Header) + 正文(body) + 页脚(Footer)

```bash
[修改类型][(影响范围)]: [标题]

[正文]

[页脚]
```

!> 修改类型和标题是强制性的，但是标题的范围是可选的

1. **标题(Header):** `type(scope): subject`

   * `type`: 用于说明commit的类型，规定如下几种：
     * `feat`: 新增功能(feature)
     * `fix`: 修复bug
     * `docs`: 修改文档(documentation)
     * `refactor`: 代码重构，没有添加新功能，也不是修复bug
     * `style`: 调整代码格式，未修改代码逻辑（e.g.: 修改空格、格式化、缩进、分号、样式等）
     * `perf`: 性能优化，提高性能的代码更改
     * `chore`: 对构建流程或辅助工具和依赖库（如文档生成，vconsole工具等）的更改
     * `revert`: 回滚版本

   * `scope`: 可选。用于说明commit影响的范围，内容不固定，例如：
     * `route`: 路由模块
     * `view`: 页面模块
     * `api`: api模块
     * `component`: 组件模块
     * `utils`: 工具模块
     * `README`: 开发文档模块
     *  `*`: 多个模块
   * `subject`： 用于简短说明更新，结尾不要使用句号

2. **正文(Body)**

   正文是对标题的补充。是commit的详细描述。如代码修改的动机，于修改前的代码对比等。

3. **页脚(Footer)**

   页脚常用备注信息。比如

   1. 版本兼容性变动（需要相关描述）
   2. 关闭指定的Issue号（也适用于关闭的bug号）



#### 03、插件推荐

commitlint: commitlint校验commit是否符合规范

husky: husky能够防止不规范代码被commit、push、merge等等