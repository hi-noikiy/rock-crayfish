### ?c=user&a=api&do=logout

---

用户退出。

### URL

---

[{{ book.host }}?c=user&a=api&do=logout]({{ book.host }}?c=user&a=api&do=logout)

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
| 无 | 无 | 无 | 无       |


### 返回值

---

| 字段 | 类型 | 说明 |
| :---: | :---: | :--- |
| code | int | 0-退出成功 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '退出成功'
}
```