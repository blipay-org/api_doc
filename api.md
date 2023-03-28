# Blipay API 

## 1.支付

请求地址：```url: http://127.0.0.1:8890/blipay_api_service/order/pay```

调用方式：```post```

请求参数：

|  参数名   | 类型  | 描述 |
|  ----  | ----  | ----  |
| amount  | double | 请求支付金额 |
| outTradeOrder  | string | 外部订单号 |
| notifyUrl  | string | 订单状态通知回调url |
| merchantId  | string | 接入者ID，可以用接入者写死 |


返回参数:

|  参数名   | 类型  | 描述 |
|  ----  | ----  | ----  |
| amount  | double | 请求支付金额 |
| outTradeOrder  | string | 外部订单号 |
| tradeOrder  | string | 当前支付订单号 |
| address  | string | 收款地址，用于二维码展示 |
| expireTime  | long | 订单过期时间戳 |
| createTime  | long | 订单创建时间戳 |
| updateTime  | long | 订单更新时间戳 |
| status  | int | 状态.  0:初始化，2:成功，3：关闭，4，失败，5，超时|
| type  | int | 订单类型. 1:支付，2：下发|

通知回调参数:
|  参数名   | 类型  | 描述 |
|  ----  | ----  | ----  |
| amount  | double | 请求支付金额 |
| outTradeOrder  | string | 外部订单号 |
| tradeOrder  | string | 当前支付订单号 |
| address  | string | 收款地址，用于二维码展示 |
| expireTime  | long | 订单过期时间戳 |
| createTime  | long | 订单创建时间戳 |
| updateTime  | long | 订单更新时间戳 |
| status  | int | 状态.  0:初始化，2:成功，3：关闭，4，失败，5，超时|
| type  | int | 订单类型. 1:支付，2：下发|

