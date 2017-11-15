### ?i=1&c=entry&storeid=3&a=api&do=cart&m=weisrc_dish

---

门店选择商品接口。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=cart&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=cart&m=weisrc_dish)


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
| is_out | bool | Y | 是否外卖，外卖订单不在副屏展示所购商品 |
| goods | string | Y | 商品数据 |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功'
}
```