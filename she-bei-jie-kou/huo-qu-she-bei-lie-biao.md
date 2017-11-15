### ?i=1&c=entry&storeid=3&a=api&do=device&m=weisrc_dish

---

获取设备列表。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=device&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=device&m=weisrc_dish)


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
| sub | int | N | 是否操作副屏，值：1或0 |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| data | array | 列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 设备ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;device | string | 设备号 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功',
    'data': [
        {
            'id': 1,
            'device': '特色小龙虾'
        },
        {
            'id': 2,
            'device': '凉拌类'
        }
    ]
}
```