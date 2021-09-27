# 标签下联系人列表/contactByLabelPageList



{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/contactByLabelPageList" %}
{% api-method-summary %}
 标签下联系人列表
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="sn" type="string" required=true %}
标签sn \(联系人标签列表接口提供\)
{% endapi-method-parameter %}

{% api-method-parameter name="pageNo" type="number" required=true %}
页码
{% endapi-method-parameter %}

{% api-method-parameter name="pageSize" type="number" required=true %}
分页数量
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
    "message": "Successful.",
    "traceNumber": "7aceb14f2e944ff1a5d5ceb35781ea40",
    "data": {
        "totalPage": 1447,
        "totalRow": 14468,
        "resultList": [
            {
                "sex_WeChat": null,
                "ageage": null,
                "邮箱": "******",
                "country": null,
                "nickname_WeChat": null,
                "customerId": "fffa2f8a-30c1-4153-875d-4ab9d79666f5",
                "微信": "******",
                "name": null,
                "mobile": null,
                "导入时间": "******",
                "更新时间": "******",
                "city_WeChat": null
            }
 
        ]
    }
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

### 注意事项

字段是否脱敏在后台配置

