# 联系人字段详情



{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/contactFieldDetails" %}
{% api-method-summary %}
联系人字段详情
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
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

{% endapi-method-response-example-description %}

```
{
    "code": 0,
    "message": "Successful.",
    "traceNumber": "47ac0ae36f0c4a58a4289c1252832231",
    "data": {
        "resultList": [
            {
                "fieldName": "weChat",
                "sn": "4c140f5832429eb1",
                "name": "微信",
                "searchType": false,
                "sortType": false
            },
            {
                "fieldName": "update_date",
                "sn": "390f451bcf04dcf1",
                "name": "更新时间",
                "searchType": false,
                "sortType": true
            }
                   ]
    }
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=403 %}
{% api-method-response-example-description %}

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

### 返回参数说明

| 字段名 | 描述 |
| :--- | :--- |
| fieldName | 联系人字段名 |
| sn | 联系人标识  |
| name | 联系人字段中文名 |
| searchType | 是否可以作为查询字段查询 true / false （联系人分页列表接口使用） |
| sortType | 是否可以作为排序字段排序 true / false （联系人分页列表接口使用） |



