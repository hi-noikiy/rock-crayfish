### ?i=1&c=entry&storeid=3&a=api&do=order_op&m=weisrc_dish

---

订单操作
- 取消
- 接单
- 配送
- 完成

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_op&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order_op&m=weisrc_dish)

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
| action | string | Y | 操作：<br />cancel: 取消订单<br />confirm: 接单<br />dispatching: 配送<br />finish: 完成 |
| id    | int   | Y   | 订单ID  |
|dispatching_corp_id | int | N | 跑腿公司ID，操作配送的时候传该值 |

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