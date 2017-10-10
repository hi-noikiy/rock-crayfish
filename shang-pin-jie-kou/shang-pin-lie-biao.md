### ?i=1&c=entry&storeid=3&a=api&do=goods&m=weisrc_dish&category_id=:category_id

---

获取指定分类下的商品

### URL

---

[{{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=goods&m=weisrc_dish&category_id=1]({{ book.app_host }}?i=1&c=entry&storeid=3&a=api&do=goods&m=weisrc_dish&category_id=1)


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
| data | array | 商品列表数据 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;id | int | 分类ID     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title | string | 商品名称 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;thumb | string | 商品缩略图 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unitname | string | 商品单位 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;marketprice | float | 商品价格 |

### 返回结果示例

---

``` js
{
    "code": 0,
    "message": "请求成功",
    "data": [{
        "id": "69",
        "title": "口味小龙虾",
        "thumb": "http://rock.xia/attachment/images/1/2017/06/Mee5NQw5IzNPnnwpjn6n2PwxzXuppT.jpg",
        "unitname": "份",
        "marketprice": "78"
    }, {
        "id": "70",
        "title": "膏蟹煲",
        "thumb": "http://rock.xia/attachment/images/1/2017/06/wy35YCiYy4ByjphqHQ43Q9I445bCCB.jpg",
        "unitname": "份",
        "marketprice": "98"
    }]
}
```