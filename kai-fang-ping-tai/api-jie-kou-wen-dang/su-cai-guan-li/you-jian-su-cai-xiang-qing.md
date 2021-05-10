# 邮件素材详情



{% api-method method="get" host="https://api.dmartech.cn" path="/open-api/v1/material/emailMaterialDetails" %}
{% api-method-summary %}
 邮件素材详情
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="materialSn" type="string" required=true %}
素材sn
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
    "createDate": "string",
    "createName": "string",
    "materialContent": "string",
    "materialName": "string",
    "previewUrl": "string",
    "sn": "string",
    "testSubject": "string",
    "updateDate": "string",
    "updateName": "string"
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

