# 标签分组列表/labelGroupList

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/labelGroupList" %}
{% api-method-summary %}
 标签分组列表
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="access-key " type="string" required=true %}
 访问凭证
{% endapi-method-parameter %}

{% api-method-parameter name="access-sign" type="string" required=true %}
 访问签名
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="sortField" type="string" required=false %}
 排序字段 createDate:创建时间,updateDate:更新时间,name:分组名称
{% endapi-method-parameter %}

{% api-method-parameter name="sortOrder" type="string" required=false %}
 排序类型 desc:倒序,asc:正序
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
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
    "resultList": [
      {
        "createDate": "2021-01-01 00:00:00",
        "name": "string",
        "parentSn": "string",
        "sn": "string"
      }
    ]
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
| sn | string | 分组sn |
| parentSn | string | 父级分组sn |
| name | string | 分组名称 |
| createDate | string | 创建时间 |

