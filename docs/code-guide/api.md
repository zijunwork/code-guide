#### 01、命名规范

1. 接口命名：统一使用中划线命名法，e.g. `user-get`
2. 接口参数命名：统一使用下划线命名法，e.g. `user_id`

```javascript
/api/user/list?page=1&page_size=10
```





#### 02、返回格式

```json
{
  "code": 200,
  "message": "success",
  "data": {}
}
```

```json
{
  "code": 404,
  "message": "Page not found",
  "data": {}
}
```



#### 03、返回状态码

1. 协议级：`200`、`301`、`302`、`401`、`403`、`502`
2. 系统级：`10001`、`10002`
3. 业务级：`20001`、`30001`、 `50001`
4. 异常级：`40001`



#### 04、请求标准

+ `GET(SELECT)` 从服务器取出资源（一项或多项）
+ `POST(CREATE)` 在服务器新建一个资源
+ `PUT(UPDATE)` 在服务器更新资源（客户端提供完整资源数据）
+ `PATCH(UPDATE)` 在服务器更新资源（客户端提供需要修改的资源数据）
+ `DELETE(DELETE)` 从服务器删除资源



#### 05、代码实现

+ `GET` 请求：公开的查询接口（无需鉴权）
+ `POST` 请求：增删改接口，私密的查询接口（需要鉴权）



#### 06、API URL规则

+ api/名词/名词 e.g. `/api/news/list`
+ api/名词/动词 e.g. `/api/news/update`



#### 07、API动词规则

+ `create` 添加、新增
+ `delete` 删除
+ `update` 更新、修改
+ `get` 获取
+ `list` 列表
+ `count` 统计
+ `batch` 批量
+ `search` 搜索
+ `query` 查询
+ `apply` 申请
+ `confirm` 确认
+ `check` 检查
+ `verify` 验证
+ `change` 更改
+ `fetch` 拉取
+ `push` 推送
+ `send` 发送
+ `notify` 通知
+ `sync` 同步
+ `bind` 绑定
+ `unbind` 解绑
+ `open` 开启
+ `close` 关闭
+ `cancel` 取消
+ `done` 结束
+ `upload` 上传
+ `accept` 同意
+ `reply` 回复
+ `refresh` 刷新 e.g. token



#### 08、HTTP状态码

+ `200` SUCCESS - GET 获取资源成功
+ `201` CREATED - POST 创建数据成功
+ `204` No Content - 对不会返回响应体的成功请求进行响应（比如DELETE请求）
+ `301` Moved Permanently - 请求的资源已永久移动到新位置
+ `302` Move Temporarily - 临时重定向
+ `304` Not Modified - 文档的内容并未改变，禁止包含消息体
+ `400` Bad Request - 请求异常，比如请求中的body无法解析
+ `401` Unauthorized - 没有进行认证或者认证非法
+ `403` Forbidden - 当认证成功，但是认证过的用户没有访问资源的权限
+ `404` Not Found - 当一个不存在的资源被请求
+ `405` Method Not Allowed - 所请求的HTTP方法不允许当前认证用户访问
+ `410` Gone - 表示当前请求的资源不再可用，当调用老版本API的时候很有用
+ `415` Unsupported Media Type - 请求中的内容类型是错误的
+ `422` Unprocessable Entity - 校验错误
+ `429` Too Many Requests - 由于请求频次达到上限而被拒绝访问
+ `500` Internal Server Error - 服务器遇到了一个未曾预料的状况
+ `502` Bad Gateway - 网关或者代理出错
+ `503` Service Unabailable - 服务器临时维护或者过载，服务器当前无法处理请求
+ `504` Gateway Timeout - 请求超时