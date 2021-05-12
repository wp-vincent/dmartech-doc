# 联系人客户属性



{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/contactCustomerDetails" %}
{% api-method-summary %}
 联系人客户属性
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="customerId" type="string" required=true %}
联系人customerId（联系人分页列表接口提供） 
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

{% endapi-method-response-example-description %}

```
{
    "code": 0,
    "message": "Successful.",
    "traceNumber": "345eddf50ecf45c79a3ef328061513db",
    "data": {
        "resultList": [

            {
                "fieldName": "health_dbp",
                "value": "",
                "name": "舒张压"
            },
            {
                "fieldName": "health_sbp",
                "value": "",
                "name": "收缩压"
            },
            {
                "fieldName": "health_age",
                "value": "",
                "name": "体检年龄"
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

###  <a id="fan-hui-can-shu-shuo-ming"></a>

### 返回参数说明 <a id="fan-hui-can-shu-shuo-ming"></a>

| 字段名 | 描述 |
| :--- | :--- |
| fieldName | 联系人字段名 |
| value | 属性值 |
| name | 字段中文名 |

