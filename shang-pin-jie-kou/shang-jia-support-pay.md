### ?i=1&c=entry&storeid=3&a=api&do=get_pay&m=weisrc_dish

---

获取商家所支持的支付方式

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=get_pay&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=category&m=weisrc_dish)

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
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 支付名称ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name | string | 支付名称 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功',
    'data': [
        {
            'id': 1,
            'pay_name': '微信支付'
        },
        {
            'id': 2,
            'pay_name': '支付宝支付'
        }
    ]
}
```
