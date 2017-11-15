### ?i=1&c=entry&storeid=3&a=api&do=settings&m=weisrc_dish

---

获取门店配置信息。

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=settings&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=settings&m=weisrc_dish)


### 传输方式

---

GET

### 是否需要登录

---

否


### 请求参数

---

| 参数名 | 类型 | 非空 | 说明 |
| :---: | :---: | :---: | :---: |
| -- | -- | -- | -- |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| data | array | 列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 门店ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title | string | 门店名称 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;address | string | 门店地址 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;devices | array | 门店设备列表 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功',
    'data': [
        {
            'id': 3,
            'title': '洛克的虾',
            'address': '兴宁市和平路5号(行政服务中心对面)',
            'devices': [
                {
                    'id': 1,
                    'device': 'RX171108001A'
                },
                {
                    'id': 2,
                    'device': 'RX171108002A'
                }
            ]
        }
    ]
}
```