### ?i=1&c=entry&storeid=3&a=api&do=voucher_qrcode&m=weisrc_dish

---

获取扫优惠券二维码。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=voucher_qrcode&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=voucher_qrcode&m=weisrc_dish)

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
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;flag | string | 二维码唯一标识 |

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "flag": "1508828223EReH33"
    }
}
```