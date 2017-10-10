### ?i=1&c=entry&storeid=3&a=api&do=order&m=weisrc_dish

---

获取订单列表数据。
- 这里storeid=3暂时固定，为以后多门店预留

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order&m=weisrc_dish]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order&m=weisrc_dish)

### 例子
- 全部订单:<br />
{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order&m=weisrc_dish
- 查询状态:<br />
{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order&m=weisrc_dish&status=-1
- 关键字查询:<br />
{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=order&m=weisrc_dish&keywords=13800138000

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
| status | int | N | 订单状态值：<br />-1：已取消<br />0: 待处理<br />1: 已处理<br />3：已完成<br />11：已配送<br /><br />若全部订单则不传该值 |
| keywords | string | N | 关键字搜索 |


### 返回值

---

| 字段 | 类型 | 说明 |
| :--- | :---: | :--- |
| code | int | 请求返回状态码 |
| message | string | 请求返回状态信息 |
| data | array | 订单列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 订单ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ordersn | string | 订单号 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;totalprice | float | 订单总金额 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dateline | string | 下单时间 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;status | int | 订单状态 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;status_title | string | 状态名称 |

### 返回结果示例

---

``` js
{
    'code': 0,
    'message': '请求成功',
    'data': [
        {
            'id': 1,
            'ordersn': '2017...5027',
            'totalprice': '586.00',
            'dateline': '17-08-14 15:41',
            'status': 0,
            'status_title': '待处理'
        }
    ]
}
```