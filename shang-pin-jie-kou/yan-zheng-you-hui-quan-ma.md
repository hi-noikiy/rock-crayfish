### ?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish&voucher=:voucher

---

验证优惠券码是否有效。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish&voucher=:voucher]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=check_voucher&m=weisrc_dish&voucher=:voucher)

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
| - | - | - | - |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求码 |
| message | string | 请求返回信息 |
| data  | object | 优惠券信息 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 优惠券ID |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gmoney | float | 优惠券满减 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dmoney | float | 优惠券减扣金额 |
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;multiple | int | 是否允许使用多份：0表示不允许，1表示允许 |
- 优惠券ID：


### 返回结果示例

---

``` js
// 以下示例说明该优惠券满100减10，订单总额满100才可用
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "id": 11,
        "gmoney": 100.00,
        "dmoney": 10.00
    }
}
```