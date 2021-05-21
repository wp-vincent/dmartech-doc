# 创建标签

{% api-method method="post" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/createLabel" %}
{% api-method-summary %}
 创建标签
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="access-key" type="string" required=true %}
 访问凭证
{% endapi-method-parameter %}

{% api-method-parameter name="access-sign" type="string" required=true %}
 访问签名
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="groupSn" type="string" required=true %}
 分组sn
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}
 标签名称
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{
  "code": 0,
  "data": {
    "id":"string"
    "name": "string",
    "sn": "string"
  },
  "message": "string",
  "traceNumber": "string"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

#### 响应参数

| 参数名 | 类型 | 描述 |
| :--- | :--- | :--- |
| sn | string | 标签sn |
| name | string | 标签名称 |
| id | string | 标签id |



