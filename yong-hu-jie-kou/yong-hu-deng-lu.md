### ?i=1&c=entry&storeid=3&a=api&do=user_op&act=login&m=weisrc_dish

---

用户登录。

### URL

---

[{{ book.host }}?i=1&c=entry&storeid=3&a=api&do=user_op&act=login&m=weisrc_dish
]({{ book.host }}?i=1&c=entry&storeid=3&a=api&do=user_op&act=login&m=weisrc_dish
)

### 传输方式

---

POST

### 是否需要登录

---

否

### 加密数据

---

- password: 密码采用AES加密算法传输给服务端


### 请求参数

---

| 参数名 | 类型 | 非空 | 说明 |
| :---: | :---: | :---: | :--- |
| username | string | Y | 登录账号       |
| password | string | Y | 登录密码       |


### 返回值

---

| 字段 | 类型 | 说明 |
| :---: | :---: | :--- |
| access_token | string | 登录加密串 |

### 返回结果示例

---

``` js
{
    'access_token': 'eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VyX2lkIjoyOSwiZW1haWwiOiIiLCJ1c2VybmFtZSI6IjE1ODEyNDI1MDcyIiwiZXhwIjoxNDk3NTEyOTg1fQ.W5MbWPD02GANnJfrEEOkfXYrc2qp4ujy8giybPH2ahM'
}
```