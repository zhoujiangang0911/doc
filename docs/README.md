# **接口文档**





## **修改历史**

| 时间   | 修改人   | 修改说明   | 版本   | 
|:----|:----|:----|:----|
| 2018-08-16   | 朱子成   | 添加获取行政区的接口说明   | v0.4   | 
| 2018-08-17   | 姚秀才   | 1. /api/user/queryUserRole  有司机角色正在运输的订单，把对应信息返回了。订单号 orderId, 车辆Id  carId,订单状态 status。  2. 订单查询发车日期参数优化：发车日期(today-今天 tomorrow-明天 thisweek-本周 nextweek-下周)  3.订单查询结果优化：运输中的单子，订单列表里面需要加上一个当前位置的坐标返回的，就是取这个单子对应车辆的最后一条记录就好了。   | V0.5   | 
| 2018-08-19   | 姚秀才   | 一、订单查询 ：  1.取消订单不显示 2.返回保单信息，3.返回增加货主信息，4.返回增加userType  二、计算订单保费接口：/api/order/updategoodprice  三、支付接口增加字段onlinePay:是否线上支付标志。   | V0.6   | 
| 2018-08-19   | 朱子成   | 去掉微信登录接口关于openid的说明   | V0.6   | 
| 2018-08-25   | 姚秀才   | 更新支付接口，支持app支付   | V0.6   | 
| 2018-08-26   | 姚秀才   | 1.创建保单：返回增加3个保单相关的字段：policyNo policyUrl downloadUrl  2.订单详情：返回增加1个是否支付运费字段：hasFreight   | V0.7   | 
| 2018-08-27   | 姚秀才   | 1.获取用户最近的角色：增加订单起始、终点坐标。  2.增加查询订单轨迹的接口。   | V0.8   | 
| 2018-09-13   | 姚秀才   | 新增接口：1.10. 获取APP版本号   | V0.8   | 
| 2018-09-25   | 周建刚   | 1、银联手机控件接口  2、支付接口添加方式字段   | V0.9   | 
| 2018-10-10   | 周建刚   | 1、添加身份证、手机号、车牌号等字段校验   | V0.9。   | 
| 2018-10-15   | 周建刚   | 添加支付宝支付   | V0.9   | 
| 2018-10-16   | 周建刚   | 1、账户可用余额查询  2、账户流水查询   | V0.9   | 
| 2018-10-17   | 肖荣   | 1.邀请注册功能  2.订单搜索功能  3.新增货单/回单功能  ４.新增订单修改功能   | v0.9   | 
| 2018-10-22   | 周建刚   | 1、账户信息查询  2、支付密码设置  3、提现功能  4、提现信息查询  5、余额支付  6、查询订单状态（支付成功后）   | v0.9   | 
| 2018-10-23   | 邱林超   | 1.添加新的收款方式(增加微信收款)   | v0.9   | 
| 2018-10-25   | 邱林超   | 1.佣金明细和总额   | v0.9   | 
| 2018-11-04   | 周建刚   | 1、订单查询返回保费支付方式   | v0.9   | 
| 2018-11-19   | 周建刚   | 1、登录返回融云token  2、查询个人资料返回融云token   | v1.0   | 
| 2018-11-20   | 周建刚   | 1、文件上传添加类型4 logo 类型   2、修改个人资料添加头像字段  3、订单返回融云token  4、牛贝流水查询返回修改（9.8）  5、用户订单明细查询（9.11）  6、登录和查询个人资料返回头像绝对路径用于显示   | v1.0   | 
| 2018-11-23   | 邱林超   | 被保险人接口(1.18-1.22)   | v1.0   | 
| 2018-11-23   | 方浩   | 添加活动相关接口(11.1)   | v1.0   | 
| 2018-11-26   | 周建刚   | 1、用户行为上传（12.2）  2、事件类型 （12.1）   | v1.0   | 
| 2018-11-29   | 周建刚   | 1、查询个人资料添加 userId 查询别人资料（1.4）   | v1.0   | 
| 2018-12-03   | 周建刚   | 1、所有支付接口添加被保险人ID    | v1.0   | 
| 2018-12-06   | 周建刚   | 1、车辆类型添加货车导航车辆类型（4.9）  2、货车导航开关（4.12）  3、更新货车导航信息（4.13）  4、货车轴数类型（4.9）   | v1.0   | 
| 2018-12-07   | 周建刚   | 1、修改事件上传地址（12.2）   | v1.0   | 
| ~~2019-02-25~~   | ~~周建刚~~   | ~~1、华夏银行直销银行开户发送短信（1.24）~~  ~~2、华夏银行直销银行开户（1.25）~~  ~~3、文件上传新增华夏银行直销银行开户身份证图片上传类型（10.1）~~   | ~~v1.1~~   | 
| 2019-03-06   | 方浩   | 1、废弃旧新增收款方(6.3)  2、新增获取绑卡支持银行列表(6.9)  3、新增收款方式(7.0)  4、华夏银行子账户开户(9.12)  5、查询充值账户信息(9.13)   | v1.1   | 
| 2019-03-06   | 周建刚   | 1、订单查询新增红包金额字段（2.17）  2、牛贝页面修改（9.8）  3、牛贝收益修改（9.3）  4、牛贝详情修改（9.11）   | v1.1   | 
| 2019-03-07   | 方浩   | 1、账号详情查询新增是否可以企业支付、支付支付可用余额、用户类型字段 (9.3)  2、查询订单接口新增订单状态(支付审核中、申请被拒)、被拒原因(2.1)  3、新增查询是否已开华夏银行子账户接口(9.14)   | v1.1   | 
| 2019-03-08   | 方浩   | 1、华夏银行开户接口更换成实名认证接口(9.12)  2、账号详情查询新增开户状态字段(9.3)  3、查询个人资料新增开户状态字段(1.4)  4、余额支付新增企业支付方式(6.7)   | v1.1   | 
| 2019-03-09   | 方浩   | 1、司机手机联想增加姓名联想字段(1.6)  2、新增收款方式新增手机号字段(7.0)   | v1.1   | 
| 2019-03-11   | 方浩   | 1、更改账户详情查询companyPayPermission和type字段说明(9.3)   | v1.1   | 
| 2019-03-12   | 方浩   | 1、查询订单新增支付方式类型(请求数据)(2.1)   | v1.1   | 
| 2019-03-13   | 方浩   | 1、查询订单订单状态筛选条件新增类型(响应数据)(2.1)  2、活动列表新增上下架状态字段(11.1)   | v1.1   | 
| 2019-03-29   | 周建刚   | 请求头添加verison 字段用来判断api版本   | v1.1   | 
| 2019-04-29   | 邱林超   | 解绑银行卡(6.10),弃用6.8   | v1.1   | 
| 2019-05-17   | 方浩   | 1、创建订单新增字段(2.5)  2、余额支付新增字段(6.7)  3、微信支付新增字段(6.1)  4、支付宝支付新增字段(6.6)  5、银联支付新增字段(6.5)     | v1.2   | 
| 2019-05-20   | 方浩   | 1、修改订单新增字段(2.16)  2、查询订单新增字段(2.1)   | v1.2   | 
| 2019-05-21   | 邱林超   | 车货匹配(13.1-13.9)   | v1.2   | 
| 2019-05-23   | 方浩   | 1、查询订单、查看订单状态新增货款和运费支付状态字段(2.1 2.17)  2、查询订单新增用户类型字段(2.1)   | v1.2   | 




# **一、接口说明**
## **1. Http请求概述**
请求方法：POST
请求数据类型：JSON
响应类型：JSON
~~测试域名(老项目)：~~[https://www.qdyunguan.com](https://www.qdyunguan.com)
测试域名：http://47.104.130.110:8080/hongniu/api/*
适应对象：微信小程序端、app, 不包括登陆接口

接口请求分为“请求header”和“请求body”（请求header只有在用户登陆以后调用的接口才使用，详见**全局请求header**）两部分，接口响应格式如**全局相应数据**

本文中提到的坐标都是采用gcj02坐标
### **1.1.全局请求he****ad****er**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 与codetype对应   | 
| codetype   | true   | string   | openid或token，openid对应微信端登陆，token对应app端登陆   | 
| hn_sign   | true   | string   | 参数签名   | 
| hn_app_key   | true   | string   | app key,每个app唯一。   | 
| timestamp   | true   | sring   | 时间戳YYYY-MM-dd hh:mm:ss:SSS   | 
| randomNumber   | true    | string   | 随机数(0-1000000)   | 
| appVersion   | true   | string   | 1.3.0   | 


注：用户在登陆之前使用的接口都不需要以上参数
本文只介绍自定义的参数，如使用json格式请求头里必须的"Content-Type":"application/json"参数就不再讲解

微信小程序请求示例
{
"usercode":"openid",
"codetype":"123456",
"hn_sign":"d54b2ea3730fa7c41430d6e0eb8b62b9",
"hn_app_key":"c33fbf23b76246bf8ee4a3d00b621e03"
}

**hn_app_key和hn_sign的说明**
App现在与后台接口对接前，需要向后台申请AppKey和AppSecret两个值。其中，AppKey是需要在Http请求的Header中传给后台的；AppSecret用于参数加密的。这两个值的具体使用方法如下：
* ~~如果是Get请求，将QueryString中的参数序列化成JSON对象，比如：传递的参数为“http://www.test.com/api/order/query?status=3&user_id=6721432”,将问号后面的查询字符串转换成这样的JSON字符串：{"status":"3", "user_id":"6721432"}; 如果是其他类型的请求(如POST，DELETE)，将请求体(request body)中的内容转为成JSON字符串。~~
* ~~然后用用后台申请的App Secret和序列化的字符串拼接，用MD5算法将相加后的字符串进行散列算出Sign值。~~
* 加密规则：AppSecret+timestamp+randomNumber 去掉空格进行MD5
* 在header中加上Key为"hn_sign"，value为上面得到的Sign的参数
* 在header中加上key为"hn_app_key",value为后台申请的App Key的参数。
* version用来判断请求的API版本。升级后必须有。
### **1.2.全局响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据，详见各个接口   | 


| **code值**   | **描述**   | 
|:----|:----:|:----|:----:|
| 200   | 成功   | 
| 400   | 警告，详细信息见msg   | 
| 401   | 用户不存在（openid或token不存在或错误）   | 
| 402   | 参数不能为空   | 
| 500   | 服务器繁忙   | 
| 300   | 业务逻辑提示，详细信息见msg   | 
| 301   | openid不存在   | 
| 302   | 手机号不存在   | 
| 303   | 用户冻结   | 
| 304   | 用户审核中   | 
| 305   | 用户审核失败   | 


### **1.3.请求示例**
这里举例讲解，具体接口里就不再一一举例

**无“请求header”请求示例**
例如1.2微信验证openid是否存在
请求header
{
"Content-Type":"application/json"
}
请求body
{
“openId”:”123456”
}
Postman请求示例
![图片](https://images-cdn.shimo.im/m6GxuHlkMVQtNwos/image.image/png!thumbnail)
![图片](https://images-cdn.shimo.im/DqIb3eqlGQMddU7O/image.image/png!thumbnail)
响应数据示例
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "id": 1,
        "mobile": "15098673645",
        "registerTime": 1526262315000,
        "openId": "123456",
        "token": null,
        "type": 2,
        "state": 0,
        "logo": "",
        "contact": "林先生",
        "nickname": null,
        "gender": null,
        "remarks": null
    }
}


**有“请求header”请求示例**
例如2.1车主端查询订单分页列表
请求header
{
"Content-Type":"application/json",
"usercode":"openid",
"codetype":"123456"
}
请求body
{
"pageNum": 1,
"pageSize": 20,
"queryStatus": 2
}
Postman请求示例
![图片](https://images-cdn.shimo.im/unnsGVt2lF4GavYQ/image.image/png!thumbnail)
![图片](https://images-cdn.shimo.im/MDeIXpXzwzcBEF2z/image.image/png!thumbnail)
响应数据示例
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "pageNum": 1,
        "pageSize": 20,
        "total": 5,
        "pages": 1,
        "list": [
            {
                "id": 15,
                "orderNum": "D20180615",
                "departNum": "9989654321",
                "startLongitude": 323,
                "destinationInfo": "青岛",
                "deliverydate": 1522598400000,
                "creationDate": 1528882215000,
                "startLatitude": 323,
                "stratPlaceInfo": "山东",
                "destinationX": 400,
                "destinationY": 250,
                "endTime": null,
                "userId": 1,
                "userName": "小张",
                "userPhone": "18562850851",
                "userIdSend": 2,
                "drivername": "小张",
                "drivermobile": "18562850851",
                "carId": 2,
                "carInfo": "1",
                "carnum": "鲁B123456",
                "payWay": 1,
                "money": 100,
                "goodName": "大白兔奶糖",
                "goodvolume": 12,
                "goodweight": 2,
                "goodPrice": null,
                "status": 2,
                "insurance": true,
                "hasFreight": false,
                "policyMoney": 0,
                "deliverydateStr": null
            },
            {
                "id": 14,
                "orderNum": "D20180614",
                "departNum": "9987654321",
                "startLongitude": 323,
                "destinationInfo": "青岛",
                "deliverydate": null,
                "creationDate": null,
                "startLatitude": 323,
                "stratPlaceInfo": "山东",
                "destinationX": 400,
                "destinationY": 250,
                "endTime": null,
                "userId": 1,
                "userName": "小张",
                "userPhone": "18562850851",
                "userIdSend": 2,
                "drivername": "小张",
                "drivermobile": "18562850851",
                "carId": 2,
                "carInfo": "1",
                "carnum": "鲁B123456",
                "payWay": 1,
                "money": 100,
                "goodName": "大白兔奶糖",
                "goodvolume": 12,
                "goodweight": 2,
                "goodPrice": null,
                "status": 2,
                "insurance": true,
                "hasFreight": false,
                "policyMoney": 0,
                "deliverydateStr": null
            }
        ]
    }
}


**二、接口定义**
## **1. 用户管理**
### **1.1. 获取短信验证码**
接口地址：/api/login/getcheckcode

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| code   | true   | string   | 校验码，（手机号+秘钥）进行MD5加密,秘钥： 85274113a1ce1c39   | 


** 响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | code=200时返回验证码   | 


### **1.2. 登录**
接口地址：/api/login/wxmilogin
此接口用于微信登录，其他登录请参考下面的登录接口。
**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| hn-user-os   | false   | string   | 用户所用设备的系统信息。   | 


**请求body**

| **参数名**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| checkcode   | true   | string   | 手机验证码   | 
| openId   | true   | string   | 微信的openId。   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | long   | 用户id   | 
| mobile   | true   | string   | 用户手机号   | 
| openid   | false   | string   | 微信的openid   | 
| token   | false   | string   | 本次登录的token，有有效期。   | 
| type   | false   | int   | 用户类型。无实际作用。   | 
| state   | false   | int   | 状态   | 
| logo   | false   | string   | 微信登录时用户图像的地址   | 
| contact   | false   | string   | 用户的联系方式   | 
| nickname   | false   | string   | 用户的微信昵称   | 
| gender   | false   | string   | 性别,1男,2女,0未知   | 
| remark   | false   | string   | 备注   | 


接口地址：/api/login/login
非微信登录调用此接口
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| hn-user-os   | false   | string   | 用户所用设备的系统信息。   | 


**请求body**

| **参数名**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| checkcode   | true   | string   | 手机验证码   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | long   | 用户id   | 
| mobile   | true   | string   | 用户手机号   | 
| openid   | false   | string   | 微信的openid   | 
| token   | false   | string   | 本次登录的token，有有效期。   | 
| type   | false   | int   | 用户类型。无实际作用。   | 
| state   | false   | int   | 状态   | 
| logo   | false   | string   | 微信登录时用户图像的地址   | 
| contact   | false   | string   | 用户的联系方式   | 
| nickname   | false   | string   | 用户的微信昵称   | 
| gender   | false   | string   | 性别,1男,2女,0未知   | 
| remark   | false   | string   | 备注   | 
| rongToken   | true   | string   | 融云token   | 
| logoPath   | true   | string   | 绝对路径用于显示   | 



### **1.3. 注销**
接口地址：/api/user/logout

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **1.4. 查询个人资料**
接口地址：/api/user/finduserinfo

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求参数**
| **参数名**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| userId   | false   | long   | 用户ID   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 主键   | 
| company   | true   | string   | 公司名称   | 
| contact   | true   | string   | 联系人   | 
| email   | true   | string   | 邮箱   | 
| phone   | true   | string   | 公司电话   | 
| province   | true   | string   | 省名称   | 
| city   | true   | string   | 市名称   | 
| district   | true   | string   | 区名称   | 
| address   | true   | string   | 详细地址   | 
| mobile   | true   | string   | 手机号   | 
| organization   | true   | string   | 公司组织机构代码   | 
| idnumber   | true   | string   | 联系人身份证   | 
| rongToken   | true | string | 融云token | 
| logo   | true   | string   | 相对路径   | 
| logoPath   | true   | string   | 绝对路径用于显示   | 
| subAccStatus   | true   | boolean   | 开户状态 true:已开子账户 false:未开   | 


### **1.5. 修改个人资料**
接口地址：/api/user/updateuserinfo

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| company   | true   | string   | 公司名称（用户身份为物流公司有此项）   | 
| contact   | true   | string   | 联系人名称   | 
| email   | true   | string   | 邮箱   | 
| phone   | true   | string   | 公司电话（用户身份为物流公司有此项）   | 
| provinceId   | true   | int   | 省份Id   | 
| province   | true   | string   | 省名称   | 
| cityId   | true   | int   | 市Id   | 
| city   | true   | string   | 市名称   | 
| districtId   | true   | int   | 区Id   | 
| district   | true   | string   | 区名称   | 
| address   | true   | string   | 详细地址   | 
| organization   | true   | string   | 公司组织机构代码（用户身份为物流公司有此项）   | 
| idnumber   | true   | string   | 联系人身份证   | 
| logo   | true   | string   | 头像（相对路径）   | 


响应数据

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 



### **1.6. 司机手机联想**
接口地址：/api/user/querydriver

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| driverMobile   | false(两个参数不能同时为空)   | string   | 手机号 （支持模糊查询）   | 
| driverName   | false(两个参数不能同时为空)   | string   | 姓名(支持模糊查询)   | 


响应数据

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| contact   | true   | string   | 姓名（用户自己维护了采有姓名，没有维护则null）   | 


### **1.7. 获取用户最近的角色**
接口地址：/api/user/queryUserRole

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| <无>   |    |    |    | 
|    |    |    |    | 


响应数据

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|
| roleId   | true   | string   | 用户的角色Id(1 车主；2司机；3货主)   | 
| roleName   | true   | string   | 用户的角色名称   | 
| orderId   | false   | string   | 订单id （有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| carId   | false   | string   | 车辆Id（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| orderNum   | false   | string   | 订单号（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| status   | false   | string   | 订单状态（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| startLongitude   | false   | string   | 出发地经度（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| startLatitude   | false   | string   | 出发地纬度（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| destinationLongitude   | false   | string   | 目的地经度（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 
| destinationLatitude   | false   | string   | 目的地纬度（有司机角色正在运输的订单  时返回数据，其他情况为空）   | 


### **1.8. 获取省市区行政信息**
接口地址：/api/address/getAreas

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| areaId   | true   | int   | 父级区域ID。如果是要获取省份和直辖市信息，请传-1。   | 


示例
| {      "areaId": -1  }   | 
|----|

响应数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| areaId   | true   | int   | 行政区的ID   | 
| areaCode   | false   | string   | 行政区的代码   | 
| areaName   | true   | string   | 行政区的名称   | 
| cityCode   | false   | string   | 行政区的市区代码。仅直辖市有。   | 
| center   | false   | string   | 行政区中心点的GPS位置。本项目不使用。   | 
| parentId   | true   | int   | 行政区所属的行政区ID。省份的行政区的parentId为-1。   | 


示例
| {     "code": 200,     "msg": "操作成功",     "data":    [              {           "areaId": 1,           "areaCode": "110000",           "areaName": "北京市",           "level": 1,           "cityCode": "010",           "center": "116.407394,39.904211",           "parentId": -1        },              {           "areaId": 792,           "areaCode": "310000",           "areaName": "上海市",           "level": 1,           "cityCode": "021",           "center": "121.473662,31.230372",           "parentId": -1        },              {           "areaId": 920,           "areaCode": "330000",           "areaName": "浙江省",           "level": 1,           "cityCode": "[]",           "center": "120.152585,30.266597",           "parentId": -1        },              {           "areaId": 1021,           "areaCode": "340000",           "areaName": "安徽省",           "level": 1,           "cityCode": "[]",           "center": "117.329949,31.733806",           "parentId": -1        },              {           "areaId": 1143,           "areaCode": "350000",           "areaName": "福建省",           "level": 1,           "cityCode": "[]",           "center": "119.295143,26.100779",           "parentId": -1        },              {           "areaId": 1238,           "areaCode": "360000",           "areaName": "江西省",           "level": 1,           "cityCode": "[]",           "center": "115.81635,28.63666",           "parentId": -1        },              {           "areaId": 1350,           "areaCode": "370000",           "areaName": "山东省",           "level": 1,           "cityCode": "[]",           "center": "117.019915,36.671156",           "parentId": -1        },              {           "areaId": 3229,           "areaCode": "810000",           "areaName": "香港特别行政区",           "level": 1,           "cityCode": "1852",           "center": "114.171203,22.277468",           "parentId": -1        }     ]  }   | 
|----|

### **1.9. 获取所有省市区行政信息**
接口地址：/api/address/getAllAreas

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----|:----|
| <无> |    |    |    | 

响应数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| areaId   | true   | int   | 行政区的ID   | 
| areaCode   | false   | string   | 行政区的代码   | 
| areaName   | true   | string   | 行政区的名称   | 
| cityCode   | false   | string   | 行政区的市区代码。仅直辖市有。   | 
| center   | false   | string   | 行政区中心点的GPS位置。本项目不使用。   | 
| parentId   | true   | int   | 行政区所属的行政区ID。省份的行政区的parentId为-1。   | 


示例
| {     "code": 200,     "msg": "操作成功",     "data":    [              {           "areaId": 1,           "areaCode": "110000",           "areaName": "北京市",           "level": 1,           "cityCode": "010",           "center": "116.407394,39.904211",           "parentId": -1        },              {           "areaId": 792,           "areaCode": "310000",           "areaName": "上海市",           "level": 1,           "cityCode": "021",           "center": "121.473662,31.230372",           "parentId": -1        },              {           "areaId": 920,           "areaCode": "330000",           "areaName": "浙江省",           "level": 1,           "cityCode": "[]",           "center": "120.152585,30.266597",           "parentId": -1        },              {           "areaId": 1021,           "areaCode": "340000",           "areaName": "安徽省",           "level": 1,           "cityCode": "[]",           "center": "117.329949,31.733806",           "parentId": -1        },              {           "areaId": 1143,           "areaCode": "350000",           "areaName": "福建省",           "level": 1,           "cityCode": "[]",           "center": "119.295143,26.100779",           "parentId": -1        },              {           "areaId": 1238,           "areaCode": "360000",           "areaName": "江西省",           "level": 1,           "cityCode": "[]",           "center": "115.81635,28.63666",           "parentId": -1        },              {           "areaId": 1350,           "areaCode": "370000",           "areaName": "山东省",           "level": 1,           "cityCode": "[]",           "center": "117.019915,36.671156",           "parentId": -1        },              {           "areaId": 3229,           "areaCode": "810000",           "areaName": "香港特别行政区",           "level": 1,           "cityCode": "1852",           "center": "114.171203,22.277468",           "parentId": -1        }     ]  }   | 
|----|

### **1.10. 获取APP版本号**
接口地址：/api/app/getVersion

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| type   | 是   | number   | APP类型，字典：1 苹果，2 安卓   | 

响应数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----|
| type   | true   | number   | APP类型，字典：1 苹果，2 安卓   | 
| versionCode   | false   | number   | 版本号   | 
| versionName   | true   | string   | 版本说明   | 

### 1.11.查询搜索记录
接口地址：/api/user/querySearchHistory

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| 无   |    |    |    | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----:|:----|
| id   | true   | number   | 记录ID   | 
| text   | true   | string   | 搜索内容   | 

### **1.12.删除搜索记录**
接口地址：/api/user/deleteSearchHistory

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 搜索记录ID   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

### 1.13.获取个人的邀请信息
接口地址：/api/user/queryInvitedInfo
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| 无   |    |    |    | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----|
| invitedCount | true   | number   | 邀请总人数   | 
| rebateTotalAmount   | true   | double   | 返佣总金额   | 
| invitedUrl   | true   | string   | 邀请链接, 例如:[http://47.104.224.80/invited.html?inviteid%3D337%26inviter%3D%E5%BE%90%E6%9D%B0](http://47.104.224.80/invited.html?inviterId%3D337%26inviterName%3D%E5%BE%90%E6%9D%B0)   | 
| invitedQrCodeUrl   | true   | string   | 邀请二维码图片地址   | 
| inviterName   | true   | string   | 邀请人姓名   | 
| title   | true   | string   | 分享标题   | 
| subtitle   | true   | string   | 分享副标题   | 
| shareIcoUrl   | true   | string   | 分享图片url   | 
| isContinue   | true   | string   | 分享活动是否继续 1是 2否   | 

### 1.14.获取邀请的用户列表
接口地址：/api/user/queryInvitedUsers
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | false   | number   | 页数，默认1   | 
| pageSize   | false   | number   | 每页条数，默认20   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----:|
| pageNum   | true   | number   | 当前页 | 
| pageSize   | true   | number   | 每页条数，默认20   | 
| total   | true   | number   | 总数量   | 
| pages   | true   | number   | 总页数   | 
| list   | true   | array   |    | 
| id   | true   | number   | 主键, 用户ID   | 
| contact | true   | string   | 用户名   | 
| mobile | true   | string   | 手机号码   | 

### 1.15.邀请注册
接口地址：/api/login/invited
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| checkCode   | true   | string   | 手机验证码   | 
| inviterId | true   | number   | 邀请人ID   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

### 1.16.验证码校验
```
接口地址：/api/login/ckeckcode
```
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| checkCode   | true   | string   | 手机验证码   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|
| code   | true   | number   | 200 成功   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

### **1.17. 获取邀请注册的短信验证码**
接口地址：/api/login/getInvitedCheckCode

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| mobile   | true   | string   | 手机号   | 
| code   | true   | string   | 校验码，（手机号+秘钥）进行MD5加密,秘钥： 85274113a1ce1c39   | 


** 响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | code=200时返回验证码   | 

### **1.18. 添加被保险人**
接口地址：/api/userinsured/add
说明:添加之前会通过身份证号查询是否添加了个人资料,没有添加则提示用户完善个人资料

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| username   | true   | string   | 个人姓名（身份为个人有此项）   | 
| idnumber   | true   | string   | 个人身份证（身份为个人有此项）   | 
| companyName   | true   | string   | 企业名称（身份为企业有此项）   | 
| companyCreditCode   | true   | string   | 企业社会信任码或纳税人识别号（身份为企业有此项）   | 
| imageUrl   | false   | string   | 证件照url相对路径(企业非必传)   | 
| email   | true   | string   | 邮箱   | 
| provinceId   | true   | int   | 省份Id   | 
| province   | true   | string   | 省名称   | 
| cityId   | true   | int   | 市Id   | 
| city   | true   | string   | 市名称   | 
| districtId   | true   | int   | 区Id   | 
| district   | true   | string   | 区名称   | 
| address   | true   | string   | 详细地址   | 
| insuredType   | true   | int   | 投保人类型 1个人 2公司   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

### **1.19. 被保险人详情**
接口地址：/api/userinsured/detail

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|
| id   | true   | long | 被保险人id   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| username   | true   | string   | 个人姓名（身份为个人有此项）   | 
| idnumber   | true   | string   | 个人身份证（身份为个人有此项）   | 
| companyName   | true   | string   | 企业名称（身份为企业有此项）   | 
| companyCreditCode   | true   | string   | 企业社会信任码或纳税人识别号（身份为企业有此项）   | 
| imageUrl   | false   | string   | 证件照url相对路径(企业非必需)   | 
| absoluteImageUrl   | false   | string   | 证件照url绝对路径(企业非必需)   | 
| email   | true   | string   | 邮箱   | 
| provinceId   | true   | int   | 省份Id   | 
| province   | true   | string   | 省名称   | 
| cityId   | true   | int   | 市Id   | 
| city   | true   | string   | 市名称   | 
| districtId   | true   | int   | 区Id   | 
| district   | true   | string   | 区名称   | 
| address   | true   | string   | 详细地址   | 
| insuredType   | true   | int   | 投保人类型 (1个人 2公司)   | 
| isDefault   | true   | boolean   | 是否为默认(0 不默认 1 默认)   | 
| isDel   | true   | boolean   | 是否删除(0 否 1 是)   | 
| isMe   | true   | boolean   | 是否为当前用户(0否 1 是)   | 
| createTime   | false   | string   | 创建时间   | 
| updateTime   | false   | string   | 更新时间   | 

### **1.20. 修改被保险人**
接口地址：/api/userinsured/update

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | long   | 被保险人id   | 
| username   | true   | string   | 个人姓名（身份为个人有此项）   | 
| idnumber   | true   | string   | 个人身份证（身份为个人有此项）   | 
| companyName   | true   | string   | 企业名称（身份为企业有此项）   | 
| companyCreditCode   | true   | string   | 企业社会信任码或纳税人识别号（身份为企业有此项）   | 
| imageUrl   | false   | string   | 证件照url相对路径(企业非必传)   | 
| email   | true   | string   | 邮箱   | 
| provinceId   | true   | int   | 省份Id   | 
| province   | true   | string   | 省名称   | 
| cityId   | true   | int   | 市Id   | 
| city   | true   | string   | 市名称   | 
| districtId   | true   | int   | 区Id   | 
| district   | true   | string   | 区名称   | 
| address   | true   | string   | 详细地址   | 
| insuredType   | true   | int   | 投保人类型 1个人 2公司   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 


### **1.21.设置默认被保险人**
接口地址：/api/userinsured/setDefault

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | long   | 被保险人id   | 
| isDefault   | true   | int   | 是否为默认(0 不默认 1 默认)   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

### **1.22. 被保险人列表**
接口地址：/api/userinsured/list

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
|    |    |    |    | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

### **1.23. 删除被保险人**
```
接口地址：/api/userinsured/delete
```

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | long   | 被保险人id   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

### **1.24.华夏银行直销银行开户发送短信**
```
接口地址：/api/hxbaccount/sendsms
```

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| userMobile   | true   | string   | 手机号   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

### **1.25.华夏银行直销银行开户**
```
接口地址：/api/hxbaccount/openaccount
```

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | c参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| bindCardNo   | true   | string   | 绑定银行卡卡号   | 
| idNo   | true   | string   | 身份证号码   | 
| userName   | true   | string   | 用户名称   | 
| userMobile   | true   | string   | 用户手机号   | 
| certimageface   | true   | string   | 身份证正面照150k-200k，jpg格式,BASE64处理（base64后不要有换行符）   | 
| certimageback   | true   | string   | 身份证背面照150k-200k，jpg格式,BASE64处理（base64后不要有换行符）   | 
| msgCode   | true   | string   | 1.24收到的验证码 | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据,200 代表成功   | 

## 
## 
## **2. 订单管理**
### **2.1. 查询订单**
接口地址：/api/order/queryPage

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | false   | number   | 页数，默认1   | 
| pageSize   | false   | number   | 每页条数，默认20   | 
| queryStatus   | false   | string   | 订单状态(0-待支付，2待发货，3配送中，4已到达, 5 已收货, 6支付审核中, 7审核被拒), 如果为空，则不限制订单状态   | 
| hasFreight   | false   | string   | 是否付运费(1是，0否)，如果为空，则不限制是否支付。   | 
| userType   | false   | string   | 我的身份（3-货主/1-车主/2-司机）   | 
| deliveryDateType   | false   | string   | 发车日期(today-今天 tomorrow-明天 thisweek-本周 nextweek-下周)   | 
| searchText   | false   | string   | 搜索内容   | 
| deliveryDateStart   | false   | string   | 起始发车时间,例如："2018-10-17"   | 
| deliveryDateEnd   | false   | string   | 结束发车时间,例如："2018-10-17"   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| 参数名称   | 是否必须   | 数据类型   | 描述   | 
|:----|:----|:----|:----|
| pageNum   | true   | number   | 当前页数   | 
| pageSize   | true   | number   | 每页条数   | 
| total   | true   | number   | 总数量   | 
| pages   | true   | number   | 总页数   | 
| userType   | false   | string   | 用户类型   | 
| list   | true   | array   |    | 

**list数据**
| id | true   | string   | 主键 | 
|:----|:----|:----|:----|
| orderNum   | true   | string   | 订单号   | 
| status | true   | string   | 订单状态 - 2待发货 3配送中 4到货 5已收货6支付审核中 7申请被拒 | 
| startLongitude | true   | string   | 出发地经度 | 
| startLatitude | true   | string   | 出发地纬度 | 
| startPlaceInfo | true   | string   | 出发地描述 | 
| destinationInfo   | true   | string   | 目的地描述   | 
| destinationLongitude | true   | string   | 目的地经度 | 
| destinationLatitude | true   | string   | 目的地纬度   | 
| creationDate   | true   | string   | 创建日期   | 
| deliverydate   | true   | string   | 发货日期   | 
| endTime   | true   | string   | 完成日期   | 
| userId   | true   | string   | 下单人id   | 
| userName   | true   | string   | 车主的姓名(非下单人)   | 
| userPhone   | true   | string   | 车主的电话(非下单人)   | 
| userIdSend   | true   | string   | 司机的id   | 
| drivername   | true   | string   | 司机的姓名   | 
| drivermobile   | true   | string   | 司机的手机号   | 
| carId   | true   | string   | 车辆id   | 
| carInfo   | true   | string   | 车辆类型   | 
| carnum   | true   | string   | 车牌号   | 
| money   | true   | number   | 运费，单位元   | 
| goodName   | true   | string   | 货物名称   | 
| goodvolume   | true   | number   | 货物体积，单位方   | 
| goodweight   | true   | number   | 货物质量，单位吨   | 
| goodPrice   | true   | number   | 货物价值，单位元   | 
| insurance   | true   | boolean   | 是否购买保险，true=是   | 
| hasFreight   | true   | boolean   | 是否付运费，true=是   | 
| departNum   | true   | string   | 发车编号   | 
| longitude | false   | string   | 订单最新GPS的经度数据（仅当运输中的订单才有值）。   | 
| latitude | false   | string   | 订单最新GPS的纬度数据（仅当运输中的订单才有值）。   | 
| ownerName   | false   | string   | 货主姓名   | 
| ownerPhone   | false   | string   | 货主电话   | 
| payWay   | false   | string   | 支付方式：0微信支付1银联支付2线下支付3支付宝支付4余额支付 5企业支付   | 
| policyNum   | false   | string   | 保单号   | 
| companyName   | false   | string   | 保险公司简称   | 
| policyMoney   | false   | number   | 保费   | 
| policyInfo   | false   | string   | 保单信息   | 
| hasGoodsImage   | false   | boolean   | 是否有货单图片   | 
| hasReceiptImage   | false   | boolean   | 是否有回单图片   | 
| policyPayWay   | false   | string   | 保单支付方式：0微信支付1银联支付2线下支付3支付宝支付4余额支付 5企业支付   | 
| ownerRongToken | false   | string   | 车主融云token   | 
| driveRongToken | false   | string   | 司机融云token   | 
| userRongToken | false   | string   | 货主融云token   | 
| verifyFailCause | false   | string   | 被拒原因 订单状态(status=7)时必须返回   | 
| replaceState   | true   | number   | 代收货款:0:否 1:是   | 
| paymentAmount   | false   | number   | 货款金额 replaceState=1 时必填   | 
| receiptName   | false   | string   | 收货人姓名 replaceState=1 时必填   | 
| receiptMobile   | false   | string   | 收货人手机 replaceState=1 时必填   | 
| freightStatus   | false   | number   | 运费支付状态: 0待支付 1支付成功 2支付失败   | 
| paymentStatus   | false   | number   | 货款状态: 0待支付 1支付成功 2支付失败   | 
| userType   | false   | string   | 用户类型（3-发货人/1-车主/2-司机 4收货人）   | 


### 
**2.2. 立即发车**
接口地址：/api/order/start

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 订单id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **2.3. 确认到达**
接口地址：/api/order/endSend

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 订单id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **2.4. 确认收货**
接口地址：/api/order/receive

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 订单id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **2.5. 创建订单**
接口地址：/api/order/add

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| departNum   | true   | string(128)   | 发车编号   | 
| startLongitude   | true   | string   | 开始地点经度   | 
| startLatitude   | true   | string   | 开始地点纬度   | 
| startPlaceInfo   | true   | string(128)   | 开始地点描述   | 
| destinationLongitude   | true   | string   | 目的地经度   | 
| destinationLatitude   | true   | string   | 目的地纬度   | 
| destinationInfo   | true   | string(128)   | 目的地描述   | 
| deliveryDate   | true   | string   | 发货日期（字符串，格式YYYY-MM-dd）   | 
| goodName   | true   | string(128)   | 货物名称   | 
| goodVolume   | true   | string   | 货物体积 (方)   | 
| goodWeight   | true   | string   | 货物质量(吨)   | 
| money   | true   | string   | 配送金额   | 
| carNum   | true   | string   | 车牌号 根据A附录车牌正则校验   | 
| ownerName   | true   | string   | 车主姓名   | 
| ownerMobile   | true   | string   | 车主手机号 根据A附录手机号正则校验   | 
| driverName   | true   | string   | 司机名称   | 
| driverMobile   | true   | string   | 司机手机号 根据A附录手机号正则校验   | 
| goodsImageUrls   | false   | array   | 货物图片列表   | 
| replaceState   | true   | number   | 代收货款:0:否 1:是   | 
| paymentAmount   | false   | number   | 货款金额 replaceState=1 时必填   | 
| receiptName   | false   | string   | 收货人姓名 replaceState=1 时必填   | 
| receiptMobile   | false   | string   | 收货人手机 replaceState=1 时必填   | 
| gsNum   | false   | string   | 货源单号(车货匹配货主下单时使用)   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----:|:----:|
| id   | true   | number   | 订单id | 
| orderNum   | true   | string   | 订单号 | 


**示例数据**

{
"departNum":"WL925868637",
"startLongitude":"120.98888",
"startLatitude":"30.760860",
"stratPlaceInfo":"青岛城阳",
"destinationLongitude":"120.344335",
"destinationLatitude":"30.805835",
"destinationInfo":"青岛市北",
"deliverydateStr":"2018-06-20",
"goodName":"红木家具",
"goodvolume":"1",
"goodweight":"1",
"money":"100",
"carnum":"鲁B56565",
"userName":"曹操",
"userPhone":"15190909090",
"drivername":"刘备",
"drivermobile":"15289898989"
}

### **2.6. 取消订单**
接口地址：/api/order/cancel

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 订单id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   | code=200时订单取消成功   | 




### **2.7 查看订单车辆轨迹**

接口地址：/api/order/positionList

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| orderId   | true   | string   | 订单id   | 
| timeOffSet   | false   | string   | 时间 (yyyy-MM-dd HH:mm:ss)   | 
| pageNum   | false   | number   | 页数，默认1   | 
| pageSize   | false   | number   | 每页条数，默认20；为空，则不限制条数   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | true   | number   | 当前页数   | 
| pageSize   | true   | number   | 每页条数   | 
| total   | true   | number   | 总数量   | 
| pages   | true   | number   | 总页数   | 
| carNum   | false   | string   | 车辆号码   | 
| startPlace   | fale   | string   | 订单开始地点描述   | 
| endPlace   | fale   | string   | 订单目的地描述   | 
| list   | true   | array   |    | 
|    carId   | true   | string   | 车辆id   | 
|    orderId   | true   | string   | 订单号   | 
|    movingTime   | true   | string   | 位移时发生的时间   | 
|    |    |    | <完整字段列表参考5.1 上传车辆位置的请求参数>   | 


### **2.8. 订单详情**
接口地址：/api/order/detail

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 订单id   | 
| orderNum   | true   | string   | 订单号   | 
| flowId   | false   | string   | 账户流水ID   | 

请求body说明:参数id和orderNum至少需要一个
**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | number   | 主键   | 
| orderNum   | true   | string   | 订单号   | 
| startLongitude   | true   | string   | 出发地经度   | 
| startLatitude   | true   | string   | 出发地纬度   | 
| startPlaceInfo   | true   | string   | 出发地描述   | 
| destinationInfo   | true   | string   | 目的地描述   | 
| destinationLongitude   | true   | string   | 目的地经度   | 
| destinationLatitude   | true   | string   | 目的地纬度   | 
| creationDate   | true   | string   | 创建日期   | 
| deliverydate   | true   | string   | 发货日期   | 
| endTime   | true   | string   | 完成日期   | 
| userId   | true   | string   | 下单人id   | 
| userName   | true   | string   | 车主的姓名(非下单人)   | 
| userPhone   | true   | string   | 车主的电话(非下单人)   | 
| userIdSend   | true   | string   | 司机的id   | 
| drivername   | true   | string   | 司机的姓名   | 
| drivermobile   | true   | string   | 司机的手机号   | 
| carId   | true   | string   | 车辆id   | 
| carInfo   | true   | string   | 车辆类型   | 
| carnum   | true   | string   | 车牌号   | 
| money   | true   | number   | 运费，单位元   | 
| goodName   | true   | string   | 货物名称   | 
| goodvolume   | true   | number   | 货物体积，单位方   | 
| goodweight   | true   | number   | 货物质量，单位吨   | 
| goodPrice   | true   | number   | 货物价值，单位元   | 
| status   | true   | number   | 订单状态 -1退款 2待发货 3配送中 4到货 5已收货   | 
| insurance   | true   | boolean   | 是否购买保险，true=是   | 
| hasFreight   | true   | boolean   | 是否付运费，true=是  是否付运费，true=是 | 
| goodsImages   | true   | arrary   | 货单图片列表   | 
| id   | true   | number   | 图片ID   | 
| imageUrl   | true   | string   | 图片绝对url   | 
| relativeImageUrl   | true   | string   | 图片相对url   | 
| role   | false   | string   | 1货主2车主3司机   | 
| policyPayWay | false   | string   | 支付方式：0微信支付1银联支付2线下支付3支付宝支付4余额支付   | 
| replaceState   | true   | number   | 代收货款:0:否 1:是   | 
| paymentAmount   | false   | number   | 货款金额 replaceState=1 时必填   | 
| receiptName   | false   | string   | 收货人姓名 replaceState=1 时必填   | 
| receiptMobile   | false   | string   | 收货人手机 replaceState=1 时必填   | 
| freightStatus   | false   | number   | 运费支付状态: 0待支付 1支付成功 2支付失败   | 
| paymentStatus   | false   | number   | 货款状态: 0待支付 1支付成功 2支付失败   | 


### **2.9 **计算订单保费
接口地址：/api/order/updategoodprice

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 订单id   | 
| goodPrice   | true   | number   | 货物价值，单位元，不能超过200万   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   | code=200时返回购买保险支付的金额，单位元   | 

### 2.10.查看回单信息
接口地址：/api/order/queryReceiptInfo
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| orderId | true   | number   | 订单ID   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| remark   | true   | string   | 备注   | 
| images   | true   | arrary   | 图片列表   | 
| id   | true   | number   | 图片ID   | 
| imageUrl   | true   | string   | 图片绝对url   | 
| relativeImageUrl   | true   | string   | 图片相对url   | 

### 2.11.保存回单信息
接口地址：/api/order/saveReceiptInfo
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| orderId | true   | number   | 订单ID   | 
| remark   | false   | string   | 备注   | 
| imageUrls   | false   | arrary   | 图片url列表(相对路径)   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

### ~~2.12.删除回单图片（废弃）~~
~~通过保存回单接口实现~~
请求地址：/api/order/deleteReceiptImage
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| orderId | true   | number   | 订单ID   | 
| imageId   | true   | number   | 图片ID   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

### 2.13.查看货单信息
接口地址：/api/order/queryGoodsImages
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| orderId | true   | number   | 订单ID   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 图片ID   | 
| imageUrl   | true   | string   | 图片绝对url   | 
| relativeImageUrl   | true   | string   | 图片相对url   | 

### ~~2.14.保存货单图片（废弃）~~
~~移到修改订单中~~
接口地址：/api/order/saveGoodsImage
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| orderId | true   | number   | 订单ID   | 
| imageUrls   | false   | arrary   | 图片url数组, 例：["url1", "url2"]   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

### ~~2.15.删除货单图片（废弃）~~
~~通过保存实现~~
请求地址：/api/order/deleteGoodsImage
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| orderId | true   | number   | 订单ID   | 
| imageId   | true   | number   | 图片ID   | 

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

### **2.16. 修改订单**
接口地址：/api/order/updateOrder

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 订单ID   | 
| departNum   | true   | string(128)   | 发车编号   | 
| startLongitude   | true   | string   | 开始地点经度   | 
| startLatitude   | true   | string   | 开始地点纬度   | 
| startPlaceInfo   | true   | string(128)   | 开始地点描述   | 
| destinationLongitude   | true   | string   | 目的地经度   | 
| destinationLatitude   | true   | string   | 目的地纬度   | 
| destinationInfo   | true   | string(128)   | 目的地描述   | 
| deliveryDate | true   | string   | 发货日期（字符串，格式YYYY-MM-dd）   | 
| goodName   | true   | string(128)   | 货物名称   | 
| goodVolume | true   | string   | 货物体积 (方)   | 
| goodWeight | true   | string   | 货物质量(吨)   | 
| money   | true   | string   | 配送金额   | 
| carNum | true   | string   | 车牌号 根据A附录车牌正则校验 | 
| ownerName | true   | string   | 车主姓名   | 
| ownerMobile | true   | string   | 车主手机号 根据A附录手机号正则校验 | 
| driverName | true   | string   | 司机名称   | 
| driverMobile | true   | string   | 司机手机号 根据A附录手机号正则校验 | 
| goodsImageUrls   | false   | string   | 货单图片url列表(相对路径)，例:["imges/1.jpg","imges/2.jpg"]   | 
| replaceState   | true   | number   | 代收货款:0:否 1:是   | 
| paymentAmount   | false   | number   | 货款金额 replaceState=1 时必填   | 
| receiptName   | false   | string   | 收货人姓名 replaceState=1 时必填   | 
| receiptMobile   | false   | string   | 收货人手机 replaceState=1 时必填   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
### **2.17. 订单状态查询**
```
接口地址：/api/order/queryOrder
```

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 订单ID   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----:|
| orderState | true   | number   | 订单状态0待支付2支付成功待发车3运输中 | 
| havePolicy | true   | string   | 是否生成保单 true /false   | 
| policyNo | fasle   | string   | 保单号码   | 
| downloadUrl   | false   | string   | 保单下载地址   | 
| policyUrl   | false   | string   | 保单查询链接   | 
| payPolicyState   | true   | string   | 0未支付1支付成功   | 
| errormsg   | false   | string   | 投保失败返回结果   | 
| redPacket   | false   | string   | 红包金额   | 
| freightStatus   | false   | number   | 运费支付状态: 0待支付 1支付成功 2支付失败   | 
| paymentStatus   | false   | number   | 货款状态: 0待支付 1支付成功 2支付失败   | 

响应示例：
```
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "policyUrl": "http://testing.mypicc.com.cn/t/cc/jEz2ee",
        "redPacket": "0.00",
        "freightStatus": "1",
        "downloadUrl": "http://partnertest.mypicc.com.cn/ecooperation/policydownload/downloadurl.do?platfromcodes=CPI000458&policyNo=94FE248CF9918240BD8852265D47F39DEC5EA03BF8D61F28B2322E838E8EC8EE&insuredID=57ACA30709A7B5C3DF453879FA18D745ECF13A6574946FF257E73E25C8C3D686&flag=Y",
        "policyNo": "PYDG20193713Q000E44102",
        "havePolicy": "true",
        "payPolicyState": "1",
        "paymentStatus": "1",
        "orderState": "5"
    }
```
1. }**保单管理**
### **3.1. 创建保单**
接口地址：/api/policy/create

**请求head****er**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| orderNum   | true   | string   | 订单编号   | 
| goodsValue   | true   | number   | 货物价值   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   |    | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| policyNo   | true   | string   | 保单号公司缩写加流水号对应序列号   | 
| policyUrl   | true   | string   | 保单查询链接   | 
| downloadUrl   | true   | number   | 电子保单下载地址   | 


### **3.2. 查询保单**
接口地址：/api/policy/queryPage

**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | false   | number   | 当前页数，默认1   | 
| pageSize   | false   | number   | 每页数量，默认20   | 
| recentMonth   | false   | number   | 近几月，比如近1个月，这里填1   | 
| carNum   | false   | string   | 车牌号   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | true   | number   | 当前页数   | 
| pageSize   | true   | number   | 每页数量   | 
| total   | true   | number   | 总记录数   | 
| pages   | true   | number   | 总页数   | 
| list   | true   | array   |    | 
| id   | true   | string   | 主键id   | 
| policyNo   | true   | string   | 保单号公司缩写加流水号对应序列号   | 
| orderNum   | true   | string   | 投保订单号   | 
| policyMoney   | true   | number   | 投保金额即保单总保险费   | 
| companyId   | true   | string   | 保险公司id   | 
| companyName   | true   | string   | 保险公司名称   | 
| createTime   | true   | number   | 创建时间   | 
| carNumber   | true   | string   | 车牌号   | 
| policyInfo   | true   | string   | 保单信息   | 



### **3.3. 查询保单总额**
接口地址：/api/policy/queryTotal

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| recentMonth   | false   | number   | 近几月，比如近1个月，这里填1   | 
| carNum   | false   | string   | 车牌号   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | string   | code=200时返回保单总金额，单位元   | 




1. **车辆模块**
### **4.1 添加车辆**
接口地址：/api/car/savecar

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|
| usercode   | true   | string   | 参考全局请s求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| carNumber   | true   | string   | 车牌号   | 
| carCode   | false   | string   | 车架号   | 
| carType   | true   | string   | 车辆类型id   | 
| carOwnerId     | true   | long   | 车主id   | 
| contactName   | true   | string   | 车辆联系人姓名   | 
| contactMobile   | true   | string   | 车辆联系人手机号   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **4.2 修改车辆**
接口地址：/api/car/updatecar

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 车辆id   | 
| carType   | true   | string   | 车辆类型id   | 
| carNumber   | true   | string   | 车牌号   | 
| carCode   | false   | string   | 车架号   | 
| contactName   | true   | string   | 车主姓名   | 
| contactMobile   | true   | string   | 车主手机号   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **4.3 删除车辆**
接口地址：/api/car/deletebyid

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 车辆id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### **4.4 根据车牌号查询**
接口地址：/api/car/querynumber

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| carNumber   | true   | string   | 车牌号(全名)   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 主键id   | 
| carType   | true   | string   | 车辆类型   | 
| status   | true   | int   | 0正常，1运输中   | 
| carNumber   | true   | string   | 车牌号   | 
| carOwnerId   | true   | long   | 车主Id   | 
| userId   | true   | long   | 添加车辆的人的用户Id（可忽略不用）   | 
| createTime   | true   | datetime   | 车辆添加时间   | 
| cartypename   | true   | string   | 车辆类型名称   | 
| contactName   | true   | string   | 车辆联系人姓名   | 
| contactMobile   | true   | string   | 车辆联系人手机号   | 
| userId   | true   | long   | 添加车辆的人的用户Id（可忽略不用）   | 
| createTime   | true   | datetime   | 车辆添加时间   | 
| cartypename   | true   | string   | 车辆类型名称   | 
| contactName   | true   | string   | 车辆联系人姓名   | 
| contactMobile   | true   | string   | 车辆联系人手机号   | 
| vehicleSize   | true   | string   | 1:微型货车; 2:轻型货车; 3:中型货车; 4:重型货车' | 
| vehicleLoad   | true   | string   | 货车的总重 ,单位：吨。 | 
| vehicleWeight   | true   | string   | 货车的载重 ,单位：吨。 | 
| vehicleLength | true   | string   | 货车的最大长度, 单位：米。 | 
| vehicleWidth | true   | string   | 货车的最大宽度,单位：米。 | 
| vehicleHeight | true   | string   | 货车的高度，单位：米。 | 
| vehicleAxis | true | string   | 货车的轴数 | 


### **4.5 查询车辆**
接口地址：/api/car/selectpagecar

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | false   | string   | 页数，默认1   | 
| pageSize   | false   | string   | 每页条数，默认20   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| pageNum   | true   | number   | 当前页数   | 
| pageSize   | true   | number   | 每页数量   | 
| total   | true   | number   | 总数量   | 
| pages   | true   | number   | 总页数   | 
| list   | true   | array   |    | 
| id   | true   | string   | 主键   | 
| carNumber   | true   | string   | 车牌号   | 
| carcode   | true   | string   | 车架号   | 
| carType   | true   | string   | 车辆类型id   | 
| carownerId   | true   | string   | 车主id   | 
| userId   | true   | string   | 创建人id   | 
| createTime   | true   | string   | 创建时间   | 
| state   | true   | string   | 0正常，1运输中   | 
| cartypename   | true   | string   | 类型名称   | 
| contactName   | true   | string   | 车辆联系人姓名   | 
| contactMobile   | true   | string   | 车辆联系人手机号   | 



### **~~4.7 查询车辆运输~~**
~~接口地址：~~~~/api/car/queryOrderPage~~

**~~请求header~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~usercode~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 
| ~~codetype~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 
| ~~hn_sign~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 
| ~~hn_app_key~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 


**~~请求body~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~pageNum~~   | ~~false~~   | ~~number~~   | ~~当前页数，默认1~~   | 
| ~~pageSize~~   | ~~false~~   | ~~number~~   | ~~每页数量，默认20~~   | 
| ~~recentMonth~~   | ~~false~~   | ~~number~~   | ~~近几月，比如近1个月，这里填1~~   | 
| ~~carNum~~   | ~~false~~   | ~~string~~   | ~~车牌号~~   | 


**~~响应数据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~code~~   | ~~true~~   | ~~number~~   | ~~错误码~~   | 
| ~~msg~~   | ~~true~~   | ~~string~~   | ~~提示信息~~   | 
| ~~data~~   | ~~true~~   | ~~object~~   | ~~响应数据~~   | 


**~~data数据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~pageNum~~   | ~~true~~   | ~~number~~   | ~~当前页数~~   | 
| ~~pageSize~~   | ~~true~~   | ~~number~~   | ~~每页数量~~   | 
| ~~total~~   | ~~true~~   | ~~number~~   | ~~总记录数~~   | 
| ~~pages~~   | ~~true~~   | ~~number~~   | ~~总页数~~   | 
| ~~list~~   | ~~true~~   | ~~array~~   |    | 
| ~~id~~   | ~~true~~   | ~~number~~   | ~~主键~~   | 
| ~~payMoney~~   | ~~true~~   | ~~number~~   | ~~支付金额，单位元~~   | 
| ~~createTime~~   | ~~true~~   | ~~string~~   | ~~支付时间~~   | 
| ~~orderNum~~   | ~~true~~   | ~~string~~   | ~~订单编号~~   | 
| ~~stratPlaceInfo~~   | ~~true~~   | ~~string~~   | ~~订单发货地~~   | 
| ~~destinationInfo~~   | ~~true~~   | ~~string~~   | ~~订单目的地~~   | 
| ~~carNum~~   | ~~true~~   | ~~string~~   | ~~车牌号~~   | 
| ~~createTimeStr~~   | ~~true~~   | ~~string~~   | ~~支付时间字符串~~   | 



### **~~4.8 查询车辆运费总额~~**
~~接口地址：~~~~/api/car/queryFreightTotal~~

**~~请求header~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~usercode~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 
| ~~codetype~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 
| ~~hn_sign~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 
| ~~hn_app_key~~   | ~~true~~   | ~~string~~   | ~~参考全局请求header~~   | 


**~~请求body~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~recentMonth~~   | ~~false~~   | ~~number~~   | ~~近几月，比如近1个月，这里填1~~   | 
| ~~carNum~~   | ~~false~~   | ~~string~~   | ~~车牌号~~   | 


**~~响应数据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| ~~code~~   | ~~true~~   | ~~number~~   | ~~错误码~~   | 
| ~~msg~~   | ~~true~~   | ~~string~~   | ~~提示信息~~   | 
| ~~data~~   | ~~true~~   | ~~string~~   | ~~code=200时返回总金额数，单位元~~   | 


### **4.****9**** 获取车辆类型**
接口地址：/api/car/vehicletype
查询所有可用的车辆类型
**请求header**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|:----:|
| type   | false   | string   | 1获取货车导航车辆类型  2获取车辆轴数类型   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | list   | 响应数据   | 


data数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 车辆类型id   | 
| carType   | true   | string   | 车辆类型名称   | 
| status   | true   | string   | 是否可用。1 代表可用 0 不可用   | 


### **4.10 车牌号联想**
接口地址: /api/car/querynumber

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| carNumber   | true   | string   | 车牌号   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| id   | true   | string   | 车辆id   | 
| carNumber   | true   | string   | 车牌号   | 
| carCode   | true   | string   | 车架号   | 
| ownerName   | true   | string   | 司机姓名   | 
| ownerPhone   | true   | string   | 司机手机号   | 
| userId   | true   | string   | 车主id   | 
| createTime   | true   | string   | 添加时间   | 
| del   | true   | true   | 是否删除   | 



### **4.11 **车辆订单明细
### 
```
接口地址: /api/account/cardetails
```


**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   |    | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----|:----:|:----|:----:|
| carNumber   | true   |    | string   | 车牌号   | 
| pageNum   | false   |    | number   | 页数，默认1   | 
| pageSize   | false   |    | number   | 每页条数，默认20   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| carDetails   | true   |    | 数字代表月份   | 
| 同订单   |    |    |    | 


**示例**
```
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "carDetails": {
            "9": [
                {
                    "id": 192,
                    "orderNum": "HN20180929151826116182",
                    "creationDate": "2018-09-29 15:18:26",
                    "deliveryDate": "2018-09-29 00:00:00",
                    "startLongitude": 121.350814,
                    "startLatitude": 31.31342,
                    "startPlaceInfo": "上海衷愿物流有限公司",
                    "destinationLongitude": 121.350814,
                    "destinationLatitude": 31.31342,
                    "destinationInfo": "上海衷愿物流有限公司",
                    "departNum": "从而",
                    "goodName": "百度",
                    "goodVolume": 1,
                    "goodWeight": 1,
                    "money": 111,
                    "carId": 39,
                    "carNum": "沪A12345",
                    "carInfo": "",
                    "ownerId": 449,
                    "ownerName": "车主姓名",
                    "ownerMobile": "15877412110",
                    "driverId": 449,
                    "driverName": "周林",
                    "driverMobile": "15877412110",
                    "userId": 449,
                    "userName": "周林",
                    "userMobile": "15877412110",
                    "status": 2,
                    "endTime": null,
                    "payTime": "2018-09-29 15:19:40",
                    "arrivedTime": null,
                    "hasFreight": true,
                    "payWay": 2,
                    "goodPrice": 1800,
                    "insurance": true,
                    "policyMoney": 0.27,
                    "orderInfo": null,
                    "receiptImageUrls": null,
                    "goodsImageUrls": null,
                    "receiptRemark": "",
                    "goodsImages": null,
                    "departUserCode": null,
                    "departCodetype": null,
                    "departTime": null,
                    "del": false
                },
                {
                    "id": 191,
                    "orderNum": "HN20180929151257713765",
                    "creationDate": "2018-09-29 15:12:57",
                    "deliveryDate": "2018-09-30 00:00:00",
                    "startLongitude": 121.350914,
                    "startLatitude": 31.313474,
                    "startPlaceInfo": "绿地领创国际",
                    "destinationLongitude": 121.350914,
                    "destinationLatitude": 31.313474,
                    "destinationInfo": "绿地领创国际",
                    "departNum": "大",
                    "goodName": "百度",
                    "goodVolume": 1,
                    "goodWeight": 1,
                    "money": 1,
                    "carId": 39,
                    "carNum": "沪A12345",
                    "carInfo": "",
                    "ownerId": 449,
                    "ownerName": "车主姓名",
                    "ownerMobile": "15877412110",
                    "driverId": 449,
                    "driverName": "周林",
                    "driverMobile": "15877412110",
                    "userId": 449,
                    "userName": "周林",
                    "userMobile": "15877412110",
                    "status": 2,
                    "endTime": null,
                    "payTime": "2018-09-29 15:13:20",
                    "arrivedTime": null,
                    "hasFreight": true,
                    "payWay": 2,
                    "goodPrice": 10000,
                    "insurance": true,
                    "policyMoney": 1.5,
                    "orderInfo": null,
                    "receiptImageUrls": null,
                    "goodsImageUrls": null,
                    "receiptRemark": "",
                    "goodsImages": null,
                    "departUserCode": null,
                    "departCodetype": null,
                    "departTime": null,
                    "del": false
                }
            ],
            "10": [
                {
                    "id": 266,
                    "orderNum": "HN20181026165837302442",
                    "creationDate": "2018-10-26 16:58:38",
                    "deliveryDate": "2018-10-26 00:00:00",
                    "startLongitude": 121.350814,
                    "startLatitude": 31.31342,
                    "startPlaceInfo": "上海衷愿物流有限公司",
                    "destinationLongitude": 106.713478,
                    "destinationLatitude": 26.578343,
                    "destinationInfo": "贵州省",
                    "departNum": "测试",
                    "goodName": "可",
                    "goodVolume": 69,
                    "goodWeight": 1,
                    "money": 1,
                    "carId": 39,
                    "carNum": "沪A12345",
                    "carInfo": "",
                    "ownerId": 449,
                    "ownerName": "车主姓名",
                    "ownerMobile": "15877412110",
                    "driverId": 449,
                    "driverName": "周林",
                    "driverMobile": "15877412110",
                    "userId": 449,
                    "userName": "周林",
                    "userMobile": "15877412110",
                    "status": 2,
                    "endTime": null,
                    "payTime": "2018-10-26 16:59:24",
                    "arrivedTime": null,
                    "hasFreight": true,
                    "payWay": 1,
                    "goodPrice": 20000,
                    "insurance": true,
                    "policyMoney": 6,
                    "orderInfo": null,
                    "receiptImageUrls": null,
                    "goodsImageUrls": null,
                    "receiptRemark": "",
                    "goodsImages": null,
                    "departUserCode": null,
                    "departCodetype": null,
                    "departTime": null,
                    "del": false
                },
                {
                    "id": 265,
                    "orderNum": "HN20181026165205416306",
                    "creationDate": "2018-10-26 16:52:06",
                    "deliveryDate": "2018-10-26 00:00:00",
                    "startLongitude": 102.70446,
                    "startLatitude": 25.051794,
                    "startPlaceInfo": "云南大学(翠湖东路)(公交站)",
                    "destinationLongitude": 121.350814,
                    "destinationLatitude": 31.31342,
                    "destinationInfo": "上海衷愿物流有限公司",
                    "departNum": "百度",
                    "goodName": "咯",
                    "goodVolume": 1,
                    "goodWeight": 1,
                    "money": 1,
                    "carId": 39,
                    "carNum": "沪A12345",
                    "carInfo": "",
                    "ownerId": 449,
                    "ownerName": "车主姓名",
                    "ownerMobile": "15877412110",
                    "driverId": 449,
                    "driverName": "周林",
                    "driverMobile": "15877412110",
                    "userId": 449,
                    "userName": "周林",
                    "userMobile": "15877412110",
                    "status": 2,
                    "endTime": null,
                    "payTime": "2018-10-26 16:57:34",
                    "arrivedTime": null,
                    "hasFreight": true,
                    "payWay": 1,
                    "goodPrice": 20000,
                    "insurance": true,
                    "policyMoney": 6,
                    "orderInfo": null,
                    "receiptImageUrls": null,
                    "goodsImageUrls": null,
                    "receiptRemark": "",
                    "goodsImages": null,
                    "departUserCode": null,
                    "departCodetype": null,
                    "departTime": null,
                    "del": false
                }
            
            ]
        }
    }
}

```
### **4.12 货车导航开关**
接口地址: /api/car/navigationSwitch

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

无
**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|
| switch | true   | boolean   | true 开启 false 关闭 | 

```
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "switch": true
    }
}
```
### **4.13 修改车辆货车导航信息**
接口地址：/api/car/updatenavigationcar


**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| carNumber   | true   | string   | 车牌号   | 
| vehicleSize   | true   | string   | 1:微型货车; 2:轻型货车; 3:中型货车; 4:重型货车'   | 
| vehicleLoad   | true   | string   | 货车的总重 ,单位：吨。   | 
| vehicleWeight   | true   | string   | 货车的载重 ,单位：吨。   | 
| vehicleLength   | true   | string   | 货车的最大长度, 单位：米。 | 
| vehicleWidth   | true   | string   | 货车的最大宽度,单位：米。 | 
| vehicleHeight   | true   | string   | 货车的高度，单位：米。 | 
| vehicleAxis   | true   | string   | 货车的轴数 | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


# 
# **5.地理位****置**
### **5.1 上传车辆位置坐标**
接口地址：/api/position/save

接口描述：上传位置坐标，坐标采用gcj02坐标

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| orderId   | true   | long   | 订单id   | 
| carId   | true   | string   | 车辆id   | 
| movingTime   | true   | datetime   | 位移时间   | 
| latitude   | true   | double   | 纬度，浮点数，范围为-90~90，负数表示南纬   | 
| longitude   | true   | double   | 经度，浮点数，范围为-180~180，负数表示西经   | 
| altitude   | false   | double   | 高度，单位 m   | 
| speed   | false   | double   | 速度，浮点数，单位m/s   | 
| direction   | false   | int   | 方向   | 
| accuracy   | false   | int   | 位置的精确度   | 
| verticalAccuracy   | false   | int   | 垂直精度，单位 m（Android 无法获取，返回 0）   | 
| horizontalAccuracy   | false   | int   | 水平精度，单位 m   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

### **5.2 获取指定订单的地理位置**
接口地址：/api/position/list
接口描述：上传位置坐标，坐标采用gcj02坐标

**请求header**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| usercode   | true   | string   | 参考全局请求header   | 
| codetype   | true   | string   | 参考全局请求header   | 
| hn_sign   | true   | string   | 参考全局请求header   | 
| hn_app_key   | true   | string   | 参考全局请求header   | 


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| orderId   | true   | long   | 订单id   | 
| carId   | true   | string   | 车辆id   | 

**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

data数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
|    |    |    |    | 
|    |    |    |    | 
|    |    |    |    | 


# **6.支付管理**
### **6.1. 微信支付**
接口地址：/wx/jsApiPay

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| orderNum   | true   | string   | 订单号   | 
| appid   | false   | string   | 应用ID (小程序不用传，app必传)   | 
| openid   | false   | string   | 微信用户openid（app不传，小程序要传）   | 
| hasFreight   | true   | boolean   | 是否付运费，true=是   | 
| hasPolicy   | true   | boolean   | 是否买保险，true=是   | 
| onlinePay   | true   | boolean   | 是否线上支付,false=线下支付(现付为true, 到付和回付为fase)   | 
| payType   | true   | string   | 0微信支付1银联支付2线下支付3支付宝支付4余额支付 5企业支付   | 
| payPassword | true   | strng   | 支付密码   | 
| insuranceUserId   | false   | long   | 被保险人ID   | 
| paybusiness | true   | string   | 1订单支付2代收货款和代收运费支付3意向金支付   | 
| matchingId   | true   | long   | 车货匹配抢单记录id   | 
| freightPayClass   | true   | number   | 运费支付类型1:现付 2:到付 3:回付   | 
| receiptName   | false   | string   | 收货人姓名 到付时必填   | 
| receiptMobile   | false   | string   | 收货人手机 到付时必填   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| timeStamp   | true   | string   | 时间   | 
| nonceStr   | true   | string   | 随机数   | 
| package   | true   | string   | prepay_id=XXXXXXX   | 
| signType   | true   | string   | 加签类型   | 
| paySign   | true   | string   | 签名   | 
| prePayId   | true   | string   | prepay_id (APP 支付时有值)   | 
| partnerId   | true   | string   | 商户号 (APP 支付时有值)   | 


参考微信jsapi

### **6.2. 获取我的收款方式**
接口地址：/api/refund/queryMyCards

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| <无>   |    |    | body传一个“{}”空json对象即可   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | long   | 收款方式ID   | 
| userId   | true   | long   |    | 
| bankName   | true   | String   | 银行名称   | 
| ~~depositBank~~   | ~~true~~   | ~~String~~   | ~~开户行名称~~   | 
| accountName   | true   | String   | 帐户名称/持卡人姓名   | 
| cardNo   | true   | String   | 银行卡号   | 
| isDefault   | true   | int   | 是否默认1默认。0非默认   | 
| type   | true   | int   | 收款/退款方式(微信0,银行卡1)   | 
| openId   | true   | String   | 微信openid   | 
| wxNickName   | true   | String   | 微信昵称   | 


### **~~6~~****~~.3.~~****~~ 新增收款方式~~****~~(废弃)~~**
~~接口地址：~~~~/api/refund/add~~

**~~请求body~~**
| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----|:----|:----|
| ~~bankName~~   | ~~true~~   | ~~String~~   |    | 
| ~~depositBank~~   | ~~true~~   | ~~String~~   | ~~开户行名称~~   | 
| ~~accountName~~   | ~~true~~   | ~~String~~   | ~~帐户名称/持卡人姓名~~   | 
| ~~cardNo~~   | ~~true~~   | ~~String~~   |    | 
| ~~code~~   | ~~true~~   | ~~String~~   | ~~小程序传过来的code~~   | 
| ~~encryptedData~~   | ~~true~~   | ~~String~~   | ~~用户敏感信息加密数据~~   | 
| ~~iv~~   | ~~true~~   | ~~String~~   | ~~加密算法的初始向量~~   | 
| ~~type~~   | ~~true~~   | ~~int~~   | ~~传0表示微信(code,encryptedData,iv四个字段必须)~~  ~~传1表示银行卡(bankName,depositBank,accountName,cardNo四个字段必须)~~   | 


**~~响应~~****~~数~~****~~据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----|:----|:----|
| ~~code~~   | ~~true~~   | ~~number~~   | ~~错误码~~   | 
| ~~msg~~   | ~~true~~   | ~~string~~   | ~~提示信息~~   | 
| ~~data~~   | ~~true~~   | ~~object~~   | ~~响应数据~~   | 


**~~data数据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----|:----|:----|
|    |    |    |    | 


### **6.4. 设置/取消默认收款方式**
```
接口地址：/api/refund/modifyDefault
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | long   |    | 
| isDefault   | true   | int   | 传0表示取消这个默认方式；传1表示将这个方式设置为默认。   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

### **6.****5. 银联支付****支付**
接口地址：/api/unionpay/unionpaytn

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| orderNum   | true   | string   | 订单号   | 
| appid   | false   | string   | 应用ID (小程序不用传，app必传)   | 
| openid   | false   | string   | 微信用户openid（app不传，小程序要传）   | 
| hasFreight   | true   | boolean   | 是否付运费，true=是   | 
| hasPolicy   | true   | boolean   | 是否买保险，true=是   | 
| onlinePay   | true   | boolean   | 是否线上支付,false=线下支付(现付为true, 到付和回付为fase)   | 
| payType   | true   | string   | 0微信支付1银联支付2线下支付3支付宝支付4余额支付 5企业支付   | 
| payPassword | true   | strng   | 支付密码   | 
| insuranceUserId   | false   | long   | 被保险人ID   | 
| paybusiness | true   | string   | 1订单支付2代收货款和代收运费支付3意向金支付   | 
| matchingId   | true   | long   | 车货匹配抢单记录id   | 
| freightPayClass   | true   | number   | 运费支付类型1:现付 2:到付 3:回付   | 
| receiptName   | false   | string   | 收货人姓名 到付时必填   | 
| receiptMobile   | false   | string   | 收货人手机 到付时必填   | 


**响应****数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**d****ata数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| code   | true   | string   | 银联返回code 00 成功 其他失败   | 
| msg   | true   | string   | 银联返回msg   | 
| tn   | true   | string   | 银行返回的tn号码   | 
| orderNum   | true   | string   | 订单号   | 

### **6.6. 支付宝支付**
```
接口地址：/api/alipay/getorderinfo
```


**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| orderNum   | true   | string   | 订单号   | 
| appid   | false   | string   | 应用ID (小程序不用传，app必传)   | 
| openid   | false   | string   | 微信用户openid（app不传，小程序要传）   | 
| hasFreight   | true   | boolean   | 是否付运费，true=是   | 
| hasPolicy   | true   | boolean   | 是否买保险，true=是   | 
| onlinePay   | true   | boolean   | 是否线上支付,false=线下支付(现付为true, 到付和回付为fase)   | 
| payType   | true   | string   | 0微信支付1银联支付2线下支付3支付宝支付4余额支付 5企业支付   | 
| payPassword | true   | strng   | 支付密码   | 
| insuranceUserId   | false   | long   | 被保险人ID   | 
| paybusiness | true   | string   | 1订单支付2代收货款和代收运费支付3意向金支付   | 
| matchingId   | true   | long   | 车货匹配抢单记录id   | 
| freightPayClass   | true   | number   | 运费支付类型1:现付 2:到付 3:回付   | 
| receiptName   | false   | string   | 收货人姓名 到付时必填   | 
| receiptMobile   | false   | string   | 收货人手机 到付时必填   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| code   | true   | string   | 支付宝返回code 00 成功 其他失败   | 
| msg   | true   | string   | 支付宝返回msg   | 
| orderInfo   | true   | string   | 支付宝返回的orderInfo   | 
| orderNum   | true   | string   | 订单号   | 

### **6.7. ****余额支付**
```
接口地址：/api/account/accountpay
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| orderNum   | true   | string   | 订单号   | 
| appid   | false   | string   | 应用ID (小程序不用传，app必传)   | 
| openid   | false   | string   | 微信用户openid（app不传，小程序要传）   | 
| hasFreight   | true   | boolean   | 是否付运费，true=是   | 
| hasPolicy   | true   | boolean   | 是否买保险，true=是   | 
| onlinePay   | true   | boolean   | 是否线上支付,false=线下支付(现付为true, 到付和回付为fase)   | 
| payType   | true   | string   | 0微信支付1银联支付2线下支付3支付宝支付4余额支付 5企业支付   | 
| payPassword   | true   | strng   | 支付密码   | 
| insuranceUserId   | false   | long   | 被保险人ID   | 
| paybusiness   | true   | string   | 1订单支付2代收货款和代收运费支付3意向金支付   | 
| matchingId   | true   | long   | 车货匹配抢单记录id   | 
| freightPayClass   | true   | number   | 运费支付类型1:现付 2:到付 3:回付   | 
| receiptName   | false   | string   | 收货人姓名 到付时必填   | 
| receiptMobile   | false   | string   | 收货人手机 到付时必填   | 


**响应****数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**dat****a数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| code   | true   | string   | 返回code 00 成功 其他失败   | 
| msg   | true   | string   | 返回msg   | 
| flowid   | true   | string   | 流水号flowid | 
| orderNum   | true   | string   | 订单号   | 

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 



### 6.9.获取绑卡支持银行列表
```
接口地址:/api/refund/bankList
```

**请求body**
无

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----:|:----:|
| id | true   | long | 银行id(新增收款方式时需传) | 
| description | true   | string   | 银行名称 | 


### **6.10. 解绑银行卡**
```
接口地址：/api/refund/remove
```

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | int   | 收款方式id   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 




### 7.0.新增收款方式
```
接口地址:/api/refund/add
```

**请求body**
| 参数名称   | 是否必须   | 数据类型   | 描述   | 
|:----|:----|:----|:----|:----:|
| type   | true   | int   | 收款方式  (微信0,银行卡1)   | 
| bankId   | type为1时必填   | long   | 选中银行id   | 
| linkAccountType   | type为1时必填   | string   | 0出入金   | 
| accountName   | type为1时必填   | string   | 开户名   | 
| idnumber   | type为1时必填   | string   | 身份证号   | 
| cardNo   | type为1时必填   | string   | 银行卡号   | 
| mobile   | type为1时必填   | string   | 手机号码   | 
| code   | type为0时必填   | String   | 小程序传过来的code   | 
| encryptedData   | type为0时必填   | String   | 用户敏感信息加密数据   | 
| iv   | type为0时必填   | String   | 加密算法的初始向量   | 



**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 



# **7.微信接口**
### **7.1.获取微信的openId**
接口地址：/wx/getid

**请****求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | string   | 授权码   | 


**响应****数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| openid   | true   | string   | 微信的openid   | 
| session_key   | true   | string   | 微信的session_key   | 
| code   | true   | string   | 状态码   | 
| msg   | true   | string   | 提示信息   | 

### **7.****2****. 保存微信的openId**
接口地址：/api/wxAuth/saveOpenId

**请求bo****dy**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----:|
| wxId | true   | string   | 微信的openId | 
| wxIdType   | true   | string   | 设备类型(iOS, Android, WeMini)   | 


**响****应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| openid   | true   | string   | 微信的openid   | 
| session_key   | true   | string   | 微信的session_key   | 
| code   | true   | string   | 状态码   | 
| msg   | true   | string   | 提示信息   | 

# 
# **8****.财务**
### **8.1. 获取运费支出**
接口地址：/api/finance/getExpressCost

**请求****body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|
| year | true   | int   | 年份 | 
| month   | true   | int   | 月份，从1开始，1代表1月，2代表2月以此类推。   | 

示例
| {  	"year":2018,  	"month":8  }   | 
|----|
**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| costDate   | true   | Strng   | 月份   | 
| costs   | true   | String   | 运费开支。含所输入日期之前12个月的数据。   | 

costs数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----:|:----:|:----|
| payWay | true | int | 1线上支付，2线下支付   | 
| money | true | money | 金额 | 

示例
| {     "code": 200,     "msg": "操作成功",     "data":    [{           "costDate": "2018-06",           "costs":          [                          {                 "payWay": 1,                 "money": 322.01              },                          {                 "payWay": 2,                 "money": 0              }           ]        },              {           "costDate": "2018-07",           "costs":          [                          {                 "payWay": 1,                 "money": 8440              },                          {                 "payWay": 2,                 "money": 0              }           ]        },              {           "costDate": "2018-08",           "costs":          [                          {                 "payWay": 1,                 "money": 0              },                          {                 "payWay": 2,                 "money": 0              }           ]        }     ]  }     | 
|----|
### **8.2. 获取保****费支出**
接口地址：/api/finance/getInsuranceCost

**请****求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|
| year | true   | int   | 年份 | 
| month   | true   | int   | 月份，从1开始，1代表1月，2代表2月以此类推。   | 


**响****应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| costDate   | true   | Strng   | 月份   | 
| costs   | true   | String   | 保费开支。含所输入日期之前12个月的数据。   | 

costs数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----:|:----:|:----:|
| payWay | true | int | 1线上支付，2线下支付 | 
| money | true | money | 金额 | 

### **8.3. 获取运费收入**
接口地址：/api/finance/getExpressIncome

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|
| year | true   | int   | 年份 | 
| month   | true   | int   | 月份，从1开始，1代表1月，2代表2月以此类推。   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| costDate   | true   | Strng   | 月份   | 
| costs   | true   | String   | 保费开支。含所输入日期之前12个月的数据。   | 

costs数据
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----:|:----:|:----|
| payWay | true | int | 1线上支付，2线下支付(暂无区分)   | 
| money | true | money | 金额 | 

### **8.4. 财****务搜索**
接口地址：/api/finance/search

**请****求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----|:----:|
| year |    | int   | 年份 | 
| month   | false   | int   | 月份，从1开始，1代表1月，2代表2月以此类推。   | 
| carNo   | false   | String   | 车牌号   | 
| financeType   | true   | int   | 财务类型，0支出和收入；1支出；2收入   | 
| pageNum   | false   | int   | 页面索引   | 
| pageSize   | false   | int   | 页面记录条数   | 
| feeType   | false   | int   | 1 运费，2保费。默认1运费。支出搜索时请传0或者1。   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| pageNum   | true   | int   | 月份   | 
| pageSize   | true   | int   |    | 
| total   | true   | int   | 总记录数/交易的总笔数   | 
| pages   | false   | int   | 无用   | 
| userType   | false   | int   | 无用   | 
| list   | true   | FinanceOrder   | 参见下订单的实体说明   | 
| totalMoney   | true   | decimal   | 总金额   | 

FinanceOrder数据

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   |    |    | 订单id   | 
| orderNum   |    |    | 订单编号 | 
| payTime   |    |    | 付款时间(yyyy-MM-dd HH:mm:ss)   | 
| money   |    |    | 金额。收入时为正数，支出时为负数   | 
| roleType   |    |    | 角色类型1车主2司机3货主   | 
| financeType   |    |    | 支出还是收入。0-支出和收入都算；1-支出；2-收入   | 

# **9.会员账户**
### **~~9~~****~~.1~~****~~. 设置支付密码(~~****~~废弃)~~**
```
接口地址：/api/account/setpass
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| passWord   | true   | string(32)   | MD5后的支付密码，必须32位   | 


**响应数****据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 




### **9.2. 更新支付密码**
```
接口地址：/api/account/updatepass
```

**请求b****ody**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----:|:----:|
| newPassWord   | true | string(32) | 新密码MD5后的支付密码，必须32位 | 
| checkCode   | true   | string   | 验证码   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 




### **9.3. 账****号详情查询 **
```
接口地址：/api/account/accountdetails
```

**请求body**


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**dat****a数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| accountCode   | true   | string   | 会员代码   | 
| userId   | true   | long   | 用户ID   | 
| userName   | false   | string   | 用户姓名   | 
| userMobile   | true   | string   | 用户手机号码   | 
| totalBalance   | true   | double   | 账户总余额=（可用余额+锁定金额+在途金额）   | 
| availableBalance   | true   | double   | 账户可用余额（实际可用余额）   | 
| lockAmount   | true   | double   | 账户锁定金额   | 
| transitAmount   | true   | double   | 账户在途金额   | 
| state   | true   | int   | 1正常2锁定   | 
| setPassWord   | true   | string   | 是否设置支付密码(true:设置过支付密码，false：未设置支付密码）   | 
| totalIntegral   | true   | double   | 总牛贝   | 
| availableIntegral   | true   | double   | 牛贝总收益   | 
| lockIntegral   | true   | double   | 牛贝昨日收益   | 
| tobeCreditedIntegral   | true   | double   |    | 
| tobeCreditedBalance   | true   | double   | 待入账金额   | 
| companyPayPermission   | true   | boolean   | 是否为企业用户(true:有  false:无)   | 
| companyAvailableBalance   | true   | double   | 企业支付可用余额   | 
| type   | true   | int   | 2:企业支付不需要输入企业支付密码  3:企业支付需要输入企业支付密码   | 
| subAccStatus | true   | boolean | 开户状态 true:已开子账户 false:未开 | 

响应数据示例:
```
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "accountCode": "HN000026",
        "userId": 26,
        "userName": "方浩",
        "userMobile": "15713954565",
        "totalBalance": 2999.2,
        "availableBalance": 2999.2,
        "lockAmount": 0,
        "transitAmount": 0,
        "accountType": "1",
        "state": 1,
        "stateStr": "正常",
        "setPassWord": "true",
        "totalIntegral": 0,
        "availableIntegral": 0,
        "lockIntegral": 0,
        "tobeCreditedIntegral": 0,
        "tobeCreditedBalance": 13,
        "companyPayPermission": true,
        "companyAvailableBalance": 28990,
        "type": 3
    }
}
```
### **9.****5****.**** ****提****现****流****水查询**
```
接口地址：/api/account/withdrawquery
```

**~~请求body~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----|:----|:----|
| ~~pageNum~~   | ~~false~~   | ~~int~~   | ~~页面索引~~   | 
| ~~pageSize~~   | ~~false~~   | ~~int~~   | ~~页面记录条数~~   | 
| ~~startDate~~   | ~~false~~   | ~~string~~   | ~~流水开始时间(yyyy-MM-dd)~~   | 
| ~~endDate~~   | ~~false~~   | ~~string~~   | ~~流水结束时间(yyyy-MM-dd)~~   | 


**~~响应数据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----|:----|:----|
| ~~code~~   | ~~true~~   | ~~number~~   | ~~错误码~~   | 
| ~~msg~~   | ~~true~~   | ~~string~~   | ~~提示信息~~   | 
| ~~data~~   | ~~true~~   | ~~object~~   | ~~响应数据~~   | 


**~~data数据~~**

| **~~参数名称~~**   | **~~是否必须~~**   | **~~数据类型~~**   | **~~描述~~**   | 
|:----|:----|:----|:----|
| ~~accountFlows~~   | ~~true~~   | ~~object~~   | ~~账号流水~~   | 
| ~~pageNum~~   | ~~true~~   | ~~int~~   | ~~当前页数~~   | 
| ~~pages~~   | ~~true~~   | ~~int~~   | ~~总页数~~   | 
| ~~total~~   | ~~true~~   | ~~int~~   | ~~总条数~~   | 
| ~~pageSize~~   | ~~true~~   | ~~int~~   | ~~每页显示的记录数~~   | 
| ~~rows~~   | ~~true~~   | ~~object~~   | ~~流水详细信息~~   | 
| ~~id~~   | ~~false~~   | ~~int~~   | ~~流水id~~   | 
| ~~accountCode~~   | ~~fasle~~   | ~~string~~   | ~~会员代码~~   | 
| ~~accountName~~   | ~~fasle~~   | ~~string~~   | ~~会员名称~~   | 
| ~~amount~~   | ~~false~~   | ~~double~~   | ~~体现金额~~   | 
| ~~reviewState~~   | ~~false~~   | ~~int~~   | ~~审核状态0未审核1审核通过2审核不通过~~   | 
| ~~state~~   | ~~false~~   | ~~int~~   | ~~状态0生成记录1已发送2提现成功3提现失败~~   | 
| ~~review_remark~~   | ~~false~~   | ~~string~~   | ~~审核备注~~   | 

响应数据示例:
```
{
    "code":200,
    "data":{
        "pageNum":1,
        "pageSize":10,
        "pages":1,
        "rows":[
            {
                "accountCode":"HN000449",
                "accountName":"名字",
                "amount":300,
                "createTime":"2018-10-19 13:19:26",
                "id":3,
                "receiptBankCode":"测试银行开户行",
                "receiptBankName":"测试银行名字",
                "receiptBankNumber":"56666666553265665",
                "receiptBankOpenName":"测试银行开户行",
                "relPayBillno":"1231231",
                "reviewState":1,
                "sourcesType":1,
                "state":1
            },
            {
                "accountCode":"HN000449",
                "accountName":"名字",
                "amount":10,
                "createTime":"2018-10-19 13:14:44",
                "id":2,
                "receiptBankCode":"测试银行开户行",
                "receiptBankName":"测试银行名字",
                "receiptBankNumber":"56666666553265665",
                "receiptBankOpenName":"测试银行开户行",
                "relPayBillno":"1231231",
                "reviewState":1,
                "sourcesType":1,
                "state":1
            },
            {
                "accountCode":"HN000449",
                "accountName":"名字",
                "amount":123.23,
                "createTime":"2018-10-18 16:10:01",
                "id":1,
                "receiptBankCode":"测试银行开户行",
                "receiptBankName":"测试银行名字",
                "receiptBankNumber":"56666666553265665",
                "receiptBankOpenName":"测试银行开户行",
                "reviewState":1,
                "sourcesType":1,
                "state":1
            }
        ],
        "total":3
    },
    "msg":"操作成功"
}
```
### **9.6. 账户提现**
```
接口地址：/api/account/withdraw
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----|:----|
| amount | true   | double   | 提现金额   | 
| payPassword | true   | string   | 支付密码   | 
| refundId | true   | long   | 提现方式id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----:|:----:|
| code   | true | string | 00成功其他失败 | 
| msg   | true | string | 消息   | 

### **9.7****. 账号****流水查询**
```
接口地址：/api/account/accountflows
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| flowtype   | true   | string   | 1余额明细2待入账明细   | 
| pageNum | false | int | 页面索引 | 
| pageSize | false | int | 页面记录条数 | 
| startDate | false   | string   | 流水开始时间(yyyy-MM-dd)   | 
| endDate | false   | string   | 流水结束时间(yyyy-MM-dd)   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| pageNum   | true   | int   | 当前页数   | 
| pages   | true   | int   | 总页数   | 
| total   | true   | int   | 总条数   | 
| pageSize   | true   | int   | 每页显示的记录数   | 
| list   | true   | object   | 流水详细信息   | 
| id   | false   | int   | 流水id   | 
| accountCode   | fasle   | string   | 会员代码   | 
| userName   | fasle   | string   | 会员名称   | 
| amount   | false   | double   | 流水发生金额   | 
| fundtype | false | int | 流水来源，1支付2提现3转账4退款5充值 | 
| inorexptype | false | int | 1收入2支出 | 
| createTime | false | string | 流水发生时间 | 
| carteUserName | false | string | 流水创建人 | 
| relAccountCode | false | string | 流水关联会员代码  微信提现openid  银行卡提现银行号码   | 
| relAccountName | false | string | 流水关联会员名称  微信提现昵称  银行卡提现银行名称   | 
| remark | false | string | 备注 | 
| ordernumber   | false   | string   | 关联订单号   | 
| fundsources   | false   | string   | 支付来源，1保费2运费3保费加运费4返现5积分兑换6邀请返现   | 
| accountCode   | true   | string   | 会员代码   | 
| flowType   | true   | string   | 流水类型1余额流水 2 提现流水   | 
| reviewState   | true   | string   | 提现审核状态 0待审核 1 审核通过 2 审核不通过   | 
| reviewRemark | true   | string   | 审核不通过的原因 | 
| state   | true   | int   |  提现状态 0生成记录、1已发送、2提现成功、3提现失败   | 
| ref1   | true   | string   | 提现方式0微信 1银行卡   | 
| title   | true   | string   | 显示标题   | 
| subtitle   | true   | string   | 副标题   | 
| subheading   | true   | string   | 时间标题   | 
| amtStr   | true   | string   | 金额   | 
| isMe   | true   | string   | 是否可以显示订单 1是 2否 3不可点击   | 
| reviewTime   | true   | string   | 审核时间   | 
| successTime   | true   | string   | 到账时间   | 

响应数据示例:
```
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "pageNum": 1,
        "pages": 3,
        "total": 51,
        "pageSize": 20,
        "list": [
            {
                "id": null,
                "accountCode": "HN000449",
                "userName": null,
                "amount": 1,
                "fundtype": 1,
                "inorexptype": 1,
                "createTime": "2018-10-27 13:40:41",
                "carteUserName": null,
                "relPayBillno": null,
                "relAccountCode": null,
                "relAccountName": null,
                "remark": null,
                "ref1": null,
                "ref2": null,
                "ref3": null,
                "ref4": null,
                "inorexptypeStr": null,
                "income": null,
                "expend": null,
                "flowType": "1",
                "reviewState": null,
                "reviewRemark": null,
                "state": null,
                "successTime": null,
                "reviewTime": null,
                "subtitle": "HN20181027134040802646",
                "title": "订单运费收入",
                "amtStr": "+1.00",
                "isMe": "1",
                "surplus": null,
                "fundtypeStr": null,
                "fundsources": null,
                "ordernumber": "HN20181027134040802646"
            }
        ]
    }
}
```

### 9.8. 积分流水查询
```
接口地址：/api/account/accountintegralflows
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| flowtype   | true   | string   | 1牛贝列表   | 
| pageNum | false | int | 页面索引 | 
| pageSize | false | int | 页面记录条数 | 
| startDate | false   | string   | 流水开始时间(yyyy-MM-dd)   | 
| endDate | false   | string   | 流水结束时间(yyyy-MM-dd)   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数****据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| pageNum   | true   | int   | 当前页数   | 
| pages   | true   | int   | 总页数   | 
| total   | true   | int   | 总条数   | 
| pageSize   | true   | int   | 每页显示的记录数   | 
| list   | true   | object   | 流水详细信息   | 
| id   | false   | int   | 用户ID   | 
| name   | false   | string   | 姓名   | 
| mobile   | false   | string   | 电话   | 
| rongToken   | false   | string   | 融云token   | 
| integralStr   | false   | string   | 牛贝显示字符   | 
| totalAmt   | false   | string   | 总收益   | 
| yesterdayAmt   | false   | string   | 昨日收益   | 

响应数据示例:
```
{
    "code": 200,
    "msg": "操作成功",
    "data": {
        "pageNum": 1,
        "pages": 1,
        "total": 1,
        "pageSize": 20,
        "list": [
            {
                "id": 133,
                "name": "周建刚",
                "company": null,
                "contact": "周建刚",
                "mobile": "17602153410",
                "rongToken": "v4cd2cNipxwX9FJPVMDE7CQnPbxE0G8DcEDeVienvtIPSf4geBUhyeS6N8UKRKaX1lfjyJlo93gvl/VehQF+sw==",
                "totalAmt": "65.06",
                "yesterdayAmt": "0.00",
                "integralStr": "（+1个）"
            }
        ]
    }
```
### }

**9****.****9. 佣金明细**
```
接口地址：/api/account/rebateFlows
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----:|
| pageNum | true   | int | 页面索引 | 
| pageSize | ture   | int | 页面记录条数 | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| pageNum   | true   | int   | 当前页数   | 
| pages   | true   | int   | 总页数   | 
| total   | true   | int   | 总条数   | 
| pageSize   | true   | int   | 每页显示的记录数   | 
| list   | true   | array   | amount:交易金额  createTime: 交易时间  rebateName:返佣人姓名  rebateMobile: 返佣人手机号,  orderNum:订单号       | 

### **9.10. 赚取的佣金总额**
```
接口地址：/api/account/rebateTotalMoney
```

**请求body(不传)**

**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据为佣金总额   | 


### **9.11. 用户订单详情**
```
接口地址：/api/account/userOrderdetails
```

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----|
| userId   | true   | long   | 用户ID   | 
| pageNum   | false   | number   | 页数，默认1   | 
| pageSize   | false   | number   | 每页条数，默认20   | 



**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   |    | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| amount   | false   | stringstring   | 金额   | 
| datestr   | false   |    | 日期   | 


**示例**
```
{
    "code": 200,
    "msg": "操作成功",
    "data": [
        {
            "amount": 55.12,
            "createTime": "2019-03-07 00:00:00",
            "datestr": "2019-03-07"
        },
        {
            "amount": 0.2,
            "createTime": "2018-12-06 00:00:00",
            "datestr": "2018-12-06"
        },
        {
            "amount": 0.09,
            "createTime": "2018-12-05 00:00:00",
            "datestr": "2018-12-05"
        },
        {
            "amount": 0.04,
            "createTime": "2018-11-07 00:00:00",
            "datestr": "2018-11-07"
        },
        {
            "amount": 0.04,
            "createTime": "2018-11-05 00:00:00",
            "datestr": "2018-11-05"
        },
        {
            "amount": 8.7,
            "createTime": "2018-11-01 00:00:00",
            "datestr": "2018-11-01"
        },
        {
            "amount": 0.87,
            "createTime": "2018-10-30 00:00:00",
            "datestr": "2018-10-30"
        }
    ]
}
```



### 9.12.实名认证
```
接口地址:/api/hxbaccount/certification
```

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| contact   | false   | string   | 姓名(未实名认证前必填)   | 
| email   | false   | string   | 邮箱(未实名认证前必填)   | 
| provinceId   | true   | int   | 省份Id   | 
| province   | true   | string   | 省名称   | 
| cityId   | true   | int   | 市Id   | 
| city   | true   | string   | 市名称   | 
| districtId   | true   | int   | 区Id   | 
| district   | true   | string   | 区名称   | 
| address   | true   | string   | 详细地址   | 
| idnumber   | false   | string   | 身份证(未实名认证前必填)   | 
| logo   | true   | string   | 头像（相对路径）   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


### 9.13.查询充值账户信息
```
接口地址:/api/hxbaccount/rechargeInfo
```

**请****求body**
无

**响应数****据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|
| othBankPayeeSubAccName | true   | string   | 收款账号户名 | 
| othBankPayeeSubAccSetteName | true   | string   | 收款账号清算行 | 
| othBankPayeeSubAcc | true   | string   | 收款账号 | 
| bankCardNum   | true   | string   | 用户绑定的银行卡号   | 

# 
### 9.14.查看是否已开华夏银行子账户

```
接口地址:/api/hxbaccount/querySubAcc
```

**请求body**
无

**响应****数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----:|:----|
| subAccStatus | true   | boolean | 开户状态 true:已开子账户 false:未开   | 

### 
# 10.文件相关
### 10.1. 文件上传
接口地址：/api/file/upload

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----|
| file   | true   | form-data   | 文件数据   | 
| classify   | true   | number   | 文件分类：1-货单, 2-回单,4 -logo 7企业营业执照，8-身份证图片    | 


**响****应****数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数****据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----:|:----|
| path   | true   | string   | 图片相对路径,保存时使用   | 
| absolutePath   | true   | string   | 图片绝对路径,显示时使用   | 
| originalName   | true   | string   | 原文件名称   | 

### 10.2. 多张图片上传
```
接口地址：/api/file/uploadFiles
```


**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----|
| file   | true   | form-data   | 文件数据   | 
| classify   | true   | number   | 文件分类：1-货单, 2-回单   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----:|:----|
| path   | true   | string   | 图片相对路径,保存时使用   | 
| absolutePath   | true   | string   | 图片绝对路径,显示时使用   | 
| originalName   | true   | string   | 原文件名称   | 

响应示例：
```
{
    "code": 200,
    "msg": "操作成功",
    "data": [
        {
            "path": "images/goods/2018/10/01154080067304821.jpg",
            "absolutePath": "https://dev.static.hongniudai.cn/images/goods/2018/10/01154080067304821.jpg",
            "originalName": "a.jpg"
        },
        {
            "path": "images/goods/2018/10/01154080067324261.jpg",
            "absolutePath": "https://dev.static.hongniudai.cn/images/goods/2018/10/01154080067324261.jpg",
            "originalName": "b.jpg"
        },
        {
            "path": "images/goods/2018/10/01154080067346538.jpg",
            "absolutePath": "https://dev.static.hongniudai.cn/images/goods/2018/10/01154080067346538.jpg",
            "originalName": "c.jpg"
        },
        {
            "path": "images/goods/2018/10/01154080067372694.jpg",
            "absolutePath": "https://dev.static.hongniudai.cn/images/goods/2018/10/01154080067372694.jpg",
            "originalName": "d.jpg"
        }
    ]
}
```


# 11.活动管理
## 11.1.获取活动列表
**接****口地****址**
```
/api/activity/list
```
**请****求****b****ody**
```
无
```

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **参数类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | 是   | Long   | 活动id   | 
| picture   | 是   | String   | 活动图片访问地址   | 
| title   | 是   | String   | 标题   | 
| subtitle   | 否   | String   | 副标题   | 
| link   | 是   | String   | 链接地址   | 
| status   | 是   | int   | 状态 0:上架 1:下架   | 

# 12.事件统计
## 12.1.事件类型查询
**接口地址**
```
/api/login/eventtpye
```
**请求body**
```
无
```

**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----:|:----|:----:|
| explanation | true | string   | 事件描述 | 
| key | true   | string   | 事件值 | 

示例：
```
{
    "code": 200,
    "msg": "操作成功",
    "data": [
        {
            "key": "home_carowner",
            "explanation": "首页-车主"
        },
        {
            "key": "home_owner",
            "explanation": "首页-货主"
        },
        {
            "key": "home_search",
            "explanation": "首页-搜索"
        },
        {
            "key": "menu_me",
            "explanation": "菜单栏-我"
        },
        {
            "key": "menu_tochat",
            "explanation": "菜单栏-聊天"
        },
        {
            "key": "menu_create_order",
            "explanation": "菜单栏-下单"
        },
        {
            "key": "menu_order",
            "explanation": "菜单栏-订单"
        },
        {
            "key": "menu_home",
            "explanation": "菜单栏-首页"
        }
    ]
}


```
## 12.2.用户行为上传
**接口地址**
```
/api/login/eventupload
```
**请求参数**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----|
| systemType | true   | string   | 系统类型必须是： ios、android 、miniprogram的一种   | 
| systemVersion | false   | string   | 系统版本号   | 
| systemOsVersion   | false   | string   | 系统版本号   | 
| systemModel   | false   | string   | 手机型号   | 
| systemName | false   | string | 系统名称   | 
| appVersion   | false   | string   | app版本号   | 
| crashlog   | false   | string   | 错误日志   | 
| events   | false   | array   |    | 
| eventkey | false   | string | 事件12.1返回的key   | 
| time   | false   | string   | 事件发生时间：yyyy-MM-dd HH:mm:ss   | 
| eventParameter   | false   | string   | 事件参数   | 

请求**示例：**
```
{
    "systemType": "android", 
    "systemVersion":"8.0.0",
    "systemOsVersion":"HOS1.1",
    "systemModel":"ONEPLUS A3000",
    "systemName":"oneplus3",
    "appVersion":"1.1.1",
    "events": [
        {
            "eventkey": "me_logout", 
            "time": "2018-10-30 18:41:58"
        }, 
        {
            "eventkey": "me_logout", 
            "time": "2018-10-30 18:41:58", 
            "eventParameter": "21"
        }
    ]
}


```
**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

# 13.车货匹配
## 13.1.发布货源信息
**接口地址**
```
/api/goodsSource/add
```

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| startTime   | true   | string   | 发货日期（字符串，格式YYYY-MM-dd）   | 
| startPlaceInfo   | true   | string(128)   | 开始地点描述   | 
| startPlaceX   | true   | string   | 开始地点经度   | 
| startPlaceY   | true   | string   | 开始地点纬度   | 
| destinationInfo   | true   | string(128)   | 目的地描述   | 
| destinationX   | true   | string   | 目的地经度   | 
| destinationY   | true   | string   | 目的地纬度   | 
| departNum   | true   | string(128)   | 发车编号   | 
| goodName   | true   | string(128)   | 货物名称   | 
| goodVolume   | true   | string   | 货物体积 (方)   | 
| goodWeight   | true   | string   | 货物质量(吨)   | 
| freightAmount   | true   | string   | 运费   | 
| carTypeId   | false   | string   | 车辆类型(默认id为1,小货车) 车辆类型接口见文档4.9)   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----:|:----|:----:|:----|
| id   | true   | number   | 货源id   | 
| gsNum   | true   | string   | 货源单号   | 

## 13.2.车货匹配列表 / 我的发布列表
**接口地址**
```
/api/goodsSource/queryPage
```
**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| queryType   | true   | string   | 1.车货匹配列表(只包含可已抢单) 2.我的发布列表   | 
| pageNum   | false   | int   | 页面索引   | 
| pageSize   | false   | int   | 页面记录条数   | 
| carTypeId   | false   | int   | 车辆类型id   | 
| deliveryDateType   | false   | string   | 发车日期(today-今天 tomorrow-明天 thisweek-本周 nextweek-下周)   | 

**响应数据**


| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 


**data数据**
| 参数名称   | 是否必须   | 数据类型   | 描述   | 
|:----|:----|:----|:----|
| id   | true   | string   | 货源id   | 
| gsNum   | true   | string   | 货源单号   | 
| startTime   | true   | string   | 发货日期（字符串，格式YYYY-MM-dd）   | 
| creationTime   | true   | string   | 创建时间   | 
| startPlaceInfo   | true   | string(128)   | 开始地点描述   | 
| startPlaceX   | true   | string   | 开始地点经度   | 
| startPlaceY   | true   | string   | 开始地点纬度   | 
| destinationInfo   | true   | string(128)   | 目的地描述   | 
| destinationX   | true   | string   | 目的地经度   | 
| destinationY   | true   | string   | 目的地纬度   | 
| departNum   | true   | string(128)   | 发车编号   | 
| goodName   | true   | string(128)   | 货物名称   | 
| goodVolume   | true   | string   | 货物体积 (方)   | 
| goodWeight   | true   | string   | 货物质量(吨)   | 
| freightAmount   | true   | string   | 运费   | 
| carTypeId   | false   | string   | 车辆类型id   | 
| carType   | true   | string   | 车辆类型名称   | 
| userId   | true   | string   | 创建用户id   | 
| userName   | true   | string   | 创建用户名   | 
| userMobile   | true   | string   | 创建用户手机号   | 
| status   | true   | string   | 货源状态(0生成1已预定2已失效 3完成)   | 


## 13.3.点击支付抢单意向金(生成抢单记录)
**接口地址**
```
/api/robOrder/add
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----|
| carId | true   | string   | 车辆id(查询我的车辆接口见4.5)   | 
| goodsSourceId | true   | string   | 货源id   | 
| robAmount | true   | string   | 意向金金额   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 抢单id   | 
| goodsSourceId   | true   | string   | 货源id   | 

## 13.4.抢单明细
**接口地址**
```
/api/robOrder/queryPage
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| goodsSourceId   | true   | string   | 货源id   | 
| pageNum   | false   | int   | 页面索引   | 
| pageSize   | false   | int   | 页面记录条数   | 


**响应数据**


| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**


| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 抢单id   | 
| goodsSourceId   | true   | string   | 货源id   | 
| creationTime   | true   | string   | 创建时间   | 
| carId   | true   | string   | 车辆id   | 
| carNum   | true   | string   | 车牌号   | 
| carType   | true   | string   | 车辆类型   | 
| carTypeName   | true   | string   | 车辆类型名称   | 
| driverId   | true   | string   | 司机id   | 
| driverName   | true   | string   | 司机名   | 
| driverMobile   | true   | string   | 司机手机号   | 
| robAmount   | true   | string   | 意向金金额   | 
| payWay   | true   | string   | 意向金支付方式   | 
| payTime   | true   | string   | 意向金支付时间   | 
| status   | true   | string   | 抢单状态(0生成1已支付2确认3失效4已完成)   | 
| cancel   | true   | string   | 取消抢单(0可以取消 1不能取消,2已取消)   | 
| cancelTime   | true   | string   | 取消抢单时间   | 
| robNum   | true   | string   | 抢单单号   | 
| payNum   | true   | string   | 支付单号   | 

## 13.5.选择下单
**接口地址**
```
/api/robOrder/choose
```

**请求body**


| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| goodsSourceId   | true   | string   | 货源id   | 
| robId   | false   | int   | 抢单id   | 


**响应数据**



| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**



| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 货源id   | 
| gsNum   | true   | string   | 货源单号   | 
| startTime   | true   | string   | 发车时间   | 
| startPlaceInfo   | true   | string(128)   | 开始地点描述   | 
| startPlaceX   | true   | string   | 开始地点经度   | 
| startPlaceY   | true   | string   | 开始地点纬度   | 
| destinationInfo   | true   | string(128)   | 目的地描述   | 
| destinationX   | true   | string   | 目的地经度   | 
| destinationY   | true   | string   | 目的地纬度   | 
| departNum   | true   | string(128)   | 发车编号   | 
| goodName   | true   | string(128)   | 货物名称   | 
| goodVolume   | true   | string   | 货物体积 (方)   | 
| goodWeight   | true   | string   | 货物质量(吨)   | 
| freightAmount   | true   | string   | 运费   | 
| carTypeId   | false   | string   | 车辆类型id   | 
| carType   | true   | string   | 车辆类型名称   | 
| userId   | true   | string   | 创建用户id   | 
| userName   | true   | string   | 创建用户名   | 
| userMobile   | true   | string   | 创建用户手机号   | 
| status   | true   | string   | 货源状态(0生成1已预定2已失效 3完成)   | 
| goodsDetail   | true   | string   | 货物详细信息   | 

## 
## 
## 13.6.我的参与
**接口地址**
```
/api/robOrder/myJoin
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| pageNum   | false   | int   | 页面索引   | 
| pageSize   | false   | int   | 页面记录条数   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 抢单id   | 
| goodsSourceId   | true   | string   | 货源id   | 
| carId   | true   | string   | 车辆id   | 
| carNum   | true   | string   | 车牌号   | 
| carType   | true   | string   | 车辆类型   | 
| carTypeName   | true   | string   | 车辆类型名称   | 
| robAmount   | true   | string   | 意向金金额   | 
| creationTime   | true   | string   | 创建时间   | 
| payTime   | true   | string   | 意向金支付时间   | 
| goodsUserId   | true   | string   | 货源下单人id   | 
| goodsUserName   | true   | string   | 货源下单人名字   | 
| goodsUserMobile   | true   | string   | 货源下单人手机号   | 
| startTime   | true   | string   | 货源发货时间   | 
| startPlaceInfo   | true   | string   | 货源发货地址   | 
| destinationInfo   | true   | string   | 货源收货地址   | 
| goodsSourceDetail   | true   | string   | 货物名称   | 
| status   | true   | string   | 抢单状态(0生成1已支付2确认3失效4已完成)   | 
| cancel   | true   | string   | 取消抢单(0可以取消 1不能取消,2已取消)   | 


## 13.7.删除发布
**接口地址**
```
/api/goodsSource/delete
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----|
| id | true   | string   | 货源id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
## 13.8.取消参与
**接口地址**
```
/api/robOrder/cancel
```

**请求body**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----|
| robId | true   | string   | 抢单id   | 


**响应数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
## 13.9.抢单状态
**接口地址**
```
/api/robOrder/queryRob
```

**请求body**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----:|:----|:----:|:----|:----:|:----|
| robId | true   | string   | 抢单id   | 


**响应数据**

| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| code   | true   | number   | 错误码   | 
| msg   | true   | string   | 提示信息   | 
| data   | true   | object   | 响应数据   | 

**data数据**
| **参数名称**   | **是否必须**   | **数据类型**   | **描述**   | 
|:----|:----|:----|:----|
| id   | true   | number   | 抢单id   | 
| goodsSourceId   | true   | string   | 货源id   | 
| carId   | true   | string   | 车辆id   | 
| carNum   | true   | string   | 车牌号   | 
| carType   | true   | string   | 车辆类型   | 
| carTypeName   | true   | string   | 车辆类型名称   | 
| robAmount   | true   | string   | 意向金金额   | 
| creationTime   | true   | string   | 创建时间   | 
| payTime   | true   | string   | 意向金支付时间   | 
| driverId   | true   | string   | 抢单人id   | 
| driverName   | true   | string   | 抢单人名字   | 
| driverMobile   | true   | string   | 抢单人手机号   | 
| payWay   | true   | string   | 支付方式(0微信,1银联,2线下支付,3支付宝支付,4余额支付)   | 
| payTime   | true   | string   | 付款时间   | 
| robNum   | true   | string   | 抢单单号   | 
| payNum   | true   | string   | 支付单号   | 
| status   | true   | string   | 抢单状态(0生成1已支付2确认3失效4已完成)   | 
| cancel   | true   | string   | 取消抢单(0可以取消 1不能取消,2已取消)   | 




**A附录**
车牌正则 ：
```
public static final String PATTERN_LICENSE_PLATE = "([京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽贵粤青藏川宁琼]{1}(([A-HJ-Z]{1}[A-HJ-NP-Z0-9]{5})|([A-HJ-Z]{1}(([DF]{1}[A-HJ-NP-Z0-9]{1}[0-9]{4})|([0-9]{5}[DF]{1})))|([A-HJ-Z]{1}[A-D0-9]{1}[0-9]{3}警)))|([0-9]{6}使)|((([沪粤川云桂鄂陕蒙藏黑辽渝]{1}A)|鲁B|闽D|蒙E|蒙H)[0-9]{4}领)|(WJ[京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽贵粤青藏川宁琼·•]{1}[0-9]{4}[TDSHBXJ0-9]{1})|([VKHBSLJNGCE]{1}[A-DJ-PR-TVY]{1}[0-9]{5})";

```
[https:](https://my.oschina.net/chenyoca/blog/1571062)[//my.osc](https://my.oschina.net/chenyoca/blog/1571062)[hina.net/chenyoca/blog/1571062](https://my.oschina.net/chenyoca/blog/1571062) 客户端 
手机号正则：
```
public static final String REGEX_MOBILES = "^((13|14|15|16|18|17|19)\\d{9})(,(13|14|15|16|18|17|19)\\d{9})*$";
