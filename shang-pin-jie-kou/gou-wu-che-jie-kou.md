### ?i=1&c=entry&storeid=3&a=api&do=cart&m=weisrc_dish

---

选择商品接口。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=cart&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=cart&m=weisrc_dish)


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
| -- | -- | -- | -- |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| data | array | 商品分类列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 分类ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name | string | 分类名称 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功',
    'data': [
        {
            'id': 1,
            'name': '特色小龙虾'
        },
        {
            'id': 2,
            'name': '凉拌类'
        }
    ]
}
```