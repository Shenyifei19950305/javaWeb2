
​    
**简要描述：** 

- 获取支付参数

**请求URL：** 
- ` https://api-ugo-web.itheima.net/api/public/v1/my/orders/req_unifiedorder `

**请求方式：**

- POST 

**请求头参数：** 

| 参数名        | 必选 | 类型   | 说明                      |
| ------------- | ---- | ------ | ------------------------- |
| Authorization | 是   | string | 用户登录成功获取的token值 |

**请求体参数：**

| 参数名       | 必选 | 类型   | 说明     |
| ------------ | ---- | ------ | -------- |
| order_number | 是   | string | 订单编号 |

 **返回示例**

``` json
{
  "message": {
    "pay": {
      "timeStamp": "1564730510",
      "nonceStr": "SReWbt3nEmpJo3tr",
      "package": "prepay_id=wx02152148991420a3b39a90811023326800",
      "signType": "MD5",
      "paySign": "3A6943C3B865FA2B2C825CDCB33C5304"
    },
    "order_number": "HMDD20190802000000000422"
  },
  "meta": {
    "msg": "预付订单生成成功",
    "status": 200
  }
}
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|pay |object   |该对象内的参数，为调用微信支付所必须  |


