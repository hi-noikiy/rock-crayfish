### ?i=1&c=entry&storeid=3&a=api&do=settings&m=weisrc_dish

---

验证门店配置信息。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=settings&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=settings&m=weisrc_dish)


### 传输方式

---

POST

### 是否需要登录

---

否


### 请求参数

---

| 参数名 | 类型 | 非空 | 说明 |
| :---: | :---: | :---: | :---: |
| device | string | Y | 设备号 |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| data | object | 返回数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 门店ID     |


### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功',
    'data': {
        'id': 3
    }
}
```