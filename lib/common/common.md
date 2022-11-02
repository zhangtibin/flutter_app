## 文件目录说明：
存放绝大多数可与业务逻辑抽离的抽象接口，公共 widget，公共构造方法，const值等

* entities：存放 jsonToModel 转出的 model,该层实际与 pages 耦合。
* extension：存放对系统Foundation 类的拖展。
* impl：对系统的抽象代理类,进行抽象,封装成 widget 回调。
* langs：国际化。
* middlewares：中间件，
* routes：业务中最核心的路由模块，使用命名路由的好处是,业务中页面与页面的跳转解耦,并且,直接就完美实现了远程路由路由的 pages 页面，
```ruby
scheme://host/path?userId=123&personId=123
```
* service：存储一些全局服务,或者三方功能模块封装
* store：存储一些单例,比如当前登录用户 User.loginer,全局单例 AppManager 等
* utils：封装一些工厂方法,http 请求等等
* value：存储一写 const 值,比如全局 horizontal 的 padding 等等,全局的本地缓存 key 键等等。
* widget：封装了一些本 APP 风格输入框,按钮,吐丝,图片加载等。