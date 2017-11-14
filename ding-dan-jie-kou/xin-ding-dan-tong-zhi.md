### 未处理订单推送通知

---

新

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_refresh&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_refresh&m=weisrc_dish)


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
| data | int | 是否有新订单：1有，0无 |
| total | int | 待处理订单总数 |

- 有新订单，提示语音。

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "data": 1,
    "total": 999
}
```