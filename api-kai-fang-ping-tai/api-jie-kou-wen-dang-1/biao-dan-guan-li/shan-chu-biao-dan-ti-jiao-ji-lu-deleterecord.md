# 删除表单提交记录/deleteRecord

{% api-method method="post" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/deleteRecord" %}
{% api-method-summary %}
Get Cakes
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
{% api-method-parameter name="\_id" type="string" required=true %}
表单提交记录ID，通过/form/submitRecordPageList 获取，可一次性提交多个\_ids。
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
    "message": "Successful.",
    "traceNumber": "7920def7752a40399b607eb2827b2625",
    "data": null
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

请求实例：**（截图url为测试环境，实际以上方信息为准。）**

![](../../../.gitbook/assets/tu-pian-11%20%282%29.png)

![](../../../.gitbook/assets/tu-pian-22%20%282%29.png)

