#### 01、编码风格意义

* Editorconfig可以帮助开发人员定义和维护编码的一致性
* 不同编辑器和IDE之间的编码风格共享



#### 02、编码风格规范

文件位于项目根目录下，`.editorconfig` 文件：

```bash
# http://editorconfig.org

# 是否为顶级配置文件，设置为true时才会停止搜索.editorconfig文件
root = true

[*]
charset = utf-8
end_of_line = lf
indent_size = 2
indent_style = space
trim_trailing_whitespace = true
insert_final_newline = true
curly_bracket_next_line = false
spaces_around_operators = true
tab_width = 2

[*.{js,ts,vue}]
quote_type = single

[*.{html,less,css,scss,sass,json}]
quote_type = double

[*.md]
trim_trailing_whitespace = false

[package.json]
indent_size = 2
```

