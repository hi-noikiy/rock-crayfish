### ?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish

---

验证优惠券码是否有效。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish)

### 传输方式

---

POST

### 是否需要登录

---

是


### 请求参数

---

| 参数名 | 类型 | 非空 | 说明 |
| :---: | :---: | :---: | :--- |
| voucher | string | Y | 用户优惠券码 |
| goods | string | Y | 订单商品列表 |

- goods: JSON化订单商品数据: [{"id":"商品ID", "total": "购买数量"}, {...}]。


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求码 |
| message | string | 请求返回信息 |
| data  | object | 优惠券信息 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;coupon | string | 优惠券名称 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sncode | string | 优惠券码 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;discount | float | 优惠券减扣金额 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;number | int | 当前使用数量 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;limit | int | 最大使用数量 |


### 返回结果示例

---

``` js
// 以下示例说明该优惠券折扣为666元，最多使用3张
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "discount": 666.00,
        "limit": 3,
        "sncode": "SN94289887901"
    }
}
```