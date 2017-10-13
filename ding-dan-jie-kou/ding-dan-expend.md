### ?i=1&c=entry&storeid=3&a=api&do=order_expend&m=weisrc_dish&start_time=2017-05-29&end_time=2017-10-29&page=1

---

获取某个时间段的订单数据

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_expend&m=weisrc_dish&start_time=2017-05-29&end_time=2017-10-29&page=1]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_expend&m=weisrc_dish&start_time=2017-05-29&end_time=2017-10-29&page=1)

### 传输方式

---

GET

### 是否需要登录

---

是

### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| data | array | 商品分类列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;total_price | float | 总成交金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;total_online_price | float | 线上付款总金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;total_cash_price | float | 现金付款总金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;total_discount_price | float |优惠券总减金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;list | &nbsp; | &nbsp; |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ordersn | string | 订单号 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dateline | int | 下单时间 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;order_total_price | float | 订单总金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;discount_money | float | 订单优惠券减免金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;totalprice | float | 订单实付金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;paytype | int | 0(未付款),1(余额),2(微信支付),3(到付) |

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "total_price": "24812.34",
        "total_online_price": 0,
        "total_cash_price": 0,
        "total_discount_price": 0,
        "list": [
            {
                "ordersn": "20171006536195525530",
                "dateline": "2017-10-06 09:33:39",
                "order_total_price": "252",
                "discount_money": "0.00",
                "totalprice": "252.00",
                "paytype": "未付款"
            },
			{
                "ordersn": "20170930438944510402",
                "dateline": "2017-09-30 11:48:13",
                "order_total_price": "58",
                "discount_money": "0.00",
                "totalprice": "58.00",
                "paytype": "未付款"
            }
		]
    }
}
// 空数据返回格式
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "total_price": 0,
        "total_online_price": 0,
        "total_cash_price": 0,
        "total_discount_price": 0,
        "list": []
    }
}
```
