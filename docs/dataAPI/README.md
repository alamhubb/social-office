# 社交软件联盟
### 关键词
Open Social Data Interoperability API
开放的社交数据互通接口

## [官网](https://shejiao.qingchiapp.com/)

## 社交数据互通互联开放接口文档

### 如无特殊说明，以下接口均需要在header中携带开发者密钥和用户授权后的token访问
* header.secretKey = 开发者密钥
* header.token = 用户授权后的token
### 项目根目录  https://social.qdaas.cn

### 错误码
* 601 未登录
* 602 具体业务错误
* 603 自定义错误，需要前端特殊处理的接口
* 604 系统内部错误
* 605 用户被封禁

### 用户信息 

* #### 获取登陆用户信息

 介绍：获取用户登陆后所需要的大部分信息，头像，昵称，年龄，头像，是否绑定手机号等等
  
 uri：[/user/getMineUser](https://social.qdaas.cn/user/getMineUser)

 请求类型：get

 请求header参数：
  * header.secretKey = 开发者密钥
  * header.token = 用户授权后的token

 请求参数：无

 返回response参数类型：ResultVO<[UserDetailVO](https://gitee.com/类的代码地址)>
      
### 动态信息

* #### 获取动态信息

 介绍：根据筛选条件获取动态信息，可根据条件筛选获取指定人群的动态信息，筛选条件包括（性别、年龄、城市编码、动态标签），还有动态的限制条件（仅哪个性别可见，仅哪个年龄可见）

 举例：以集美小世界，女生社区举例，请求数据时，筛选条件设置为，获取仅女生可见的动态，且动态发布人为女生

 uri：[/user/getMineUser](https://social.qdaas.cn/user/getMineUser)

 请求类型：get

 请求header参数：
  * header.secretKey = 开发者密钥
  * header.token = 用户授权后的token

 请求参数：无

 返回response参数类型：ResultVO<[UserDetailVO](https://gitee.com/类的代码地址)>
