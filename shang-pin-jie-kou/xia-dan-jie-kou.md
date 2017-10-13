### ?i=1&c=entry&storeid=3&a=api&do=add_order&m=weisrc_dish

---

店内下单、电话下单。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=add_order&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=add_order&m=weisrc_dish)

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
| username | string | N | 收货人姓名 |
| tel | string | N | 收货人电话 |
| address | string | N | 收货地址 |
| remark | string | N | 订单备注 |
| voucher | string | N | 优惠券码 |
| voucher_number | int | N | 优惠券数量 |
| goods | string | Y | 订单商品列表 |

- goods: JSON化订单商品数据: [{"id":"商品ID", "total": "购买数量"}, {...}]。


### 请求示例

---
``` js
{
    "username": "张三丰",
    "tel": "13800138000",
    "address": "广东省梅州市天河区车陂高地大街121号",
    "remark": "微辣",
    "voucher": "SN87788787",
    "goods": "[{"id":"69","total":1},{"id":"70","total":1}]"
}
```


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| - | - | - |

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功"
}
```