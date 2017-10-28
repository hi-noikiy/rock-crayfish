### ?i=1&c=entry&storeid=3&a=api&do=order_detail&m=weisrc_dish&id=:id

---

获取订单列表数据。
- 这里storeid=3暂时固定，为以后多门店预留

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_detail&m=weisrc_dish&id=:id]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_detail&m=weisrc_dish&id=:id)

- :id - 订单ID，非ordersn

### 传输方式

---

GET

### 是否需要登录

---

是


### 请求参数

---

| 参数名 | 类型 | 非空 | 说明 |
| :---: | :---: | :---: | :--- |
| 无 | 无 | 无 | 无 |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| is_self_take | bool | 是否门店自取<br />true=是<br />false=否<br /> |
| show_dispatch_corp | bool | APP可不理会此字段，WEB端需要 |
| data | array | 订单列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 订单ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ordersn | string | 订单号 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;username | string | 收货人姓名 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tel | string | 收货人手机号码 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;address | string | 收货地址 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dispatchprice | int | 配送费 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;totalprice | string | 订单总金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dateline | string | 下单时间 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;totalnum | string | 商品总数量 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;discount_money | string | 折扣 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pay_type | string | 付款方式 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;status | string | 订单状态 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;remark | string | 订单备注 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dispatch_id | int | 选择的跑腿公司ID |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods | array | 商品列表 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title | string | 商品名称 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;total | int | 商品数量 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;price | float | 商品总价 |

- 订单正常操作流程为：接单、配送、完成。
- 配送时需选择跑腿公司，若is_self_take值为true，则不显示跑腿公司，跳过配送这一流程，直接完成订单。


### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "is_self_take": 0,
    "show_dispatch_corp": 1,
    "data": {
        "id": "70",
        "ordersn": "20170814965100875027",
        "username": "林不懂",
        "tel": "15812425072",
        "address": "sjdf kf",
        "dispatchprice": "0.00",
        "totalprice": "586.00",
        "dateline": "2017-08-14 15:41:49",
        "totalnum": "7",
        "discount": 0,
        "pay_type": "现金支付",
        "status": "0",
        "remark": "多辣，少油",
        "dispatch_id": 1,
        "goods": [{
            "title": "爆炒小龙虾",
            "total": "2",
            "price": "78.00"
        }, {
            "title": "蒜香小龙虾",
            "total": "1",
            "price": "78.00"
        }, {
            "title": "口味小龙虾",
            "total": "1",
            "price": "78.00"
        }, {
            "title": "麻辣小龙虾",
            "total": "1",
            "price": "78.00"
        }, {
            "title": "干锅香辣蟹",
            "total": "1",
            "price": "98.00"
        }, {
            "title": "膏蟹煲",
            "total": "1",
            "price": "98.00"
        }]
    }
}
```