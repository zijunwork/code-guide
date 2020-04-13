#### 01、开发文档

用于项目项目开发过程中，记录重要的开发信息。其必要性的意义个人总结如下：

1. 提高软件开发的能见度
2. 提高开发效率
3. 利于软化后期迭代的开发和维护，增强可读性和可维护性
4. 提供对软件的运行，维护的有关信息，便于管理人员、开发人员、运维同事、用户之间的协作，交流和了解
5. 也有利于项目的交接、培训等工作



#### 02、开发文档文件规范

1. 项目开发的总文档必须写在项目的根目录 `README.md` 文件中
2. 建议每个超过3个文件或文件夹的目录下，需要有文档说明。命名为：`~README.md`



#### 03、开发文档内容规范

1. 项目名称
2. 项目的技术栈清单
3. 项目的环境配置中每个配置项的注解说明
4. 如果是Hybrid开发，需要有联调地址清单
5. 项目版本迭代信息
6. 项目的运行说明
7. 项目的所有文件或目录的说明



#### 04、版本更新日志书写规范

1. `A`: 新增 xxx
2. `U`: 优化 xxx
3. `F`: 修复 xxx



#### 05、开发文档举例说明

```markdown
# xxx项目开发文档

**技术栈: Vue2.5.2 + Vue-router + VueX + axios + mint-ui**

## 项目测试/生产配置文件参数（test/prod.env.js）:
​```
  NODE_ENV: '"production"', // 环境名称：development/production(测试/生产）
  WX_APPID: '"XXX"', // 微信公众号APPID
  BASE_URL: '"XXX"' // 接口地址
​```

## Hybrid联调地址列表:
+ 开发环境：
  - 展示列表页： http://172.16.55.29:8086/xxx
+ 测试环境：
  - 展示列表页： xxx

## 项目迭代日志:
> ### v1.0.x更新内容？
> 1. `A` 新增 xxx
> 2. `U` 优化 xxx
> 3. `F` 修复 xxx

## 项目运行说明:
​``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
​```

## 项目根项目文件说明:
+ public : 静态资源文件夹（图片、json）
+ src : 资源文件夹,项目主文件夹
+ .env.developent : 环境配置
+ .babel.config.js : ES6语法编译配置
+ .editorconfig : 编辑器的一些配置（编码格式、缩进风格、换行格式）
+ .eslintignore : eslint忽略文件配置
+ .eslintrc.js : eslint配置文件
+ .gitignore : git仓库上传忽略文件配置
+ favicon.ico : logo图标
+ README.md : 开发文档
+ vue.config.js : vue项目配置
+ package.json : 项目基本信息（模块、项目名称、版本）
```



