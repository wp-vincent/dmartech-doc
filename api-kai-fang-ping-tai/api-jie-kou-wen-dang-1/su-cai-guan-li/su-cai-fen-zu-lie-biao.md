# 素材分组列表



{% api-method method="get" host="https://api.dmartech.cn" path="/open-api/v1/material/groupList" %}
{% api-method-summary %}
 素材分组列表
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="keywords" type="string" required=false %}
 关键字 素材分组名称
{% endapi-method-parameter %}

{% api-method-parameter name="sortField" type="string" required=false %}
排序字段 groupName/createDate/updateDate
{% endapi-method-parameter %}

{% api-method-parameter name="sortOrder" type="string" required=false %}
 排序类型 desc\(倒序\)/asc\(正序\)
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="access-sign" type="string" required=true %}
访问签名
{% endapi-method-parameter %}

{% api-method-parameter name="access-key" type="string" required=true %}
访问凭证
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
 成功事例
{% endapi-method-response-example-description %}

```
{
  "code": 0,
  "data": {
    "resultList": [
      {
        "keywords": "string",
        "sortField": "string",
        "sortOrder": "string"
      }
    ]
  },
  "message": "string",
  "traceNumber": "string"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=403 %}
{% api-method-response-example-description %}
失败案例
{% endapi-method-response-example-description %}

```
{
    "code": 40003,
    "message": "Forbidden",
    "traceNumber": "dcfd0c46b9e64d5a8a20b852388f6310",
    "data": null
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

### 

