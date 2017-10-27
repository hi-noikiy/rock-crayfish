### ?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish&flag=:flag

---

根据二维码唯一标识（flag）获取用户选择优惠券的折扣信息。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish&flag=111111]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish&flag=11111)

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
| 无 | - | - | - |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求码 |
| message | string | 请求返回信息 |
| data  | object | 优惠券信息 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;coupon | string | 优惠券名称 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sncode | string | 优惠券码 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;discount | float | 优惠金额 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;number | int | 使用数量 |

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "coupon": "满100减10",
        "discount": 10.00,
        "number": 1
    }
}
```