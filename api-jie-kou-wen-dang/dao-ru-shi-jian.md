---
description: 用于单独事件导入，适用于添加增量数据。
---

# 导入事件

{% api-method method="post" host=" http://data-api.dmartech.cn/api/v1/api/import?secret=" path="your\_secret\_key" %}
{% api-method-summary %}
导入事件 event
{% endapi-method-summary %}

{% api-method-description %}
secret key 在数据中心-API数据源详情中找到。  
  
在导入客户数据的时候请务必确认至少导入一个主键，否则会失败。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="secret" type="string" required=true %}
请求认证密钥，在 **数据中心-API数据源** 中的找到SECRET
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="type" type="string" required=true %}
导入事件数据时该值为**event**, 标识这是一条事件数据导入请求
{% endapi-method-parameter %}

{% api-method-parameter name="event" type="string" required=true %}
事件名称, 标识该次请求是为哪个事件导入或更新数据
{% endapi-method-parameter %}

{% api-method-parameter name="properties" type="string" required=true %}
事件属性, 取值来自 "数据中心-元数据-事件属性" 和 "带主键标识的用户属性"
{% endapi-method-parameter %}

{% api-method-parameter name="event\_id" type="string" required=true %}
是事件的主键, 事件的唯一标识。
{% endapi-method-parameter %}

{% api-method-parameter name="create\_time" type="string" required=true %}
事件发生时间。格式为DATETIME
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
请求成功
{% endapi-method-response-example-description %}

```javascript
{
  "errcode": 0,
  "errmsg": "success"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
 请求错误（具体错误码说明见下方）
{% endapi-method-response-example-description %}

```javascript
{
   "errcode":10001,
   "errmsg":"json数据格式化失败"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

#### 请求示例

```text
{
    "type": "event",
    "event": "order_detail",
    "properties": {
        "mobile": "18366668888",
        "email": "zhangsan@sample.com",
        "event_id": "2018071216423310001",
        "create_time": "2018-07-12 16:42:33",
        "shop_name": "<门店名称>",
        "amount": "<订单金额>",
        "item_num": "<商品数量>",
        ...
    }
}
```

### 特殊参数说明

properties中都需要"带主键标识的用户属性"且至少一个有值.

#### 特别说明: 

1. "带主键标识的用户属性": 在"**数据中心-元数据-用户属性**"中可以将某些属性设置为主键标识, 默认为手机号和邮箱设为主键标识, 在导入数据时会根据这两个属性查询用户并更新数据。 （与任意主键一致即会合并更新数据）。

2. 事件数据中需要两个**必要**的属性,"**event\_id**"和"**create\_time**"。event\_id为该事件数据的唯一标识，create\_time为该事件发生的时间.

#### 返回码说明

| 返回码 | 说明 |
| :--- | :--- |
| 0 | 请求成功 |
| 10000 | 系统错误 |
| 10001 | json数据格式化失败 |
| 10002 | type取值不合法 |
| 10003 | 缺少secret参数 |
| 10004 | 属性列表为空 |
| 20000 | 身份验证失败 |
| 20001 | 缺少主键标识的用户属性 |
| 20002 | 至少需要一个主键标识的用户属性存在值 |
| 20003 | 数据校验失败 |

#### 备注

**该结果只是标识请求结果, 数据导入结果请查看系统中相关数据源的导入详情**

