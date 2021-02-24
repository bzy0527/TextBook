# 微信支付退款 WxPayRefund

作用：发起微信退款，服务器需要配置微信商户号-API安全证书；

### 设计属性

#### 1、微信支付退款：

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：微信支付退款；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；
* ##### App Id

  * 类型：字符串；

  * 说明：微信开放平台审核通过的移动应用APPID；
* ##### Saller

  * 类型：字符串；

  * 示例：12**\*\***\*\*02;

  * 说明：商户号，需与APPID签约绑定关系。

* ##### SubAppId

  * 类型：字符串；

  * 说明：子应用APPID，可不填；
* ##### SubMchId

  * 类型：字符串；

  * 说明：子商户号，可不填；
* ##### 签名密钥

  * 类型：字符串；

  * 值：

  * 说明：签名密钥；
* ##### 交易编号

  * 类型：字符串；

  * 值：示例：42000002592……

  * 说明：支付成功后微信账单详情里的“交易单号”；
* ##### 订单号

  * 类型：字符串；

  * 说明：支付的商户订单号；

* ##### 退单号

  * 类型：字符串；

  * 说明：支付的商户退单号。

* ##### 支付金额

  * 类型：数值；

  * 示例:@0.01；

  * 说明：本订单的支付金额；
* ##### 退款金额

  * 类型：数值；

  * 示例：@0.01；

  * 说明：本次退款的退款金额；
* ##### 操作员

  * 类型：字符串；

  * 示例：收银员；

  * 说明：填写操作员信息；

#### 2、调用成功：调用成功时需要执行的操作

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：调用成功；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；

#### 3、调用失败：调用失败时需要执行的操作

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：调用失败；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；

##### 回调函数参数：

* ##### payinfo-获取退款信息对象

  * 类型：对象；

  * 说明：在“调用成功”和“调用失败”中可以获取退款信息对象payinfo。支付信息对象属性JSonData对象包含“交易编号”、“退单号”属性。

  * 结构：

  * ```js
    //payinfo	退款信息对象结构：
    //Transaction_Id:退款交易编号；
    //Refund_Id：退单号；
    {"JSonData":{"Transaction_id":
    "50000500222019……",
    "Refund_Id":"12334453"},
    "Exception":"","State":0};
    ```


