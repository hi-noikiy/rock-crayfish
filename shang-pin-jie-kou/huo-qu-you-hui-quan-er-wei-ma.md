### ?i=1&c=entry&storeid=3&a=api&do=voucher_qrcode&m=weisrc_dish&flag=1

---

获取扫优惠券二维码。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=voucher_qrcode&m=weisrc_dish&flag=1]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=voucher_qrcode&m=weisrc_dish&flag=1)

### 传输方式

---

GET

### 是否需要登录

---

否


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
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;qrcode | string | 二维码URL |

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "data": {
        "qrcode": "http://xia.1234x.com/xxxx.png"
    }
}
```