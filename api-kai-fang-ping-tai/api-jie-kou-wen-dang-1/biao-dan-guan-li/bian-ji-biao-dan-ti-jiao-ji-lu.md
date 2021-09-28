---
description: editRecord
---

# 编辑表单提交记录/editRecord

{% api-method method="put" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/editRecord" %}
{% api-method-summary %}
 编辑表单提交记录
{% endapi-method-summary %}

{% api-method-description %}
 调用此接口注意事项：  
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
{% api-method-parameter name="formSn" type="string" required=true %}
必填，通过/form/formPageList 获取。
{% endapi-method-parameter %}

{% api-method-parameter name="\_Id" type="string" required=true %}
表单提交记录ID，必填，不能使用cutomerid或其他主键，因为可能重复提交且未加密。通过/form/submitRecordPageList 获取。
{% endapi-method-parameter %}

{% api-method-parameter name="formSn" type="string" required=true %}
必填，表单项的HTML名称，而非字段名称以及对应的值。
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
    "traceNumber": "9fb45ada62024164ace92dd1542a081d",
    "data": null
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

  参数获取实例：**（截图url为测试环境，实际以上方信息为准。）**

  formSn:   通过/form/formPageList 获取

![](../../../.gitbook/assets/tu-pian-1%20%283%29.png)

\_id  :  通过/form/submitRecordPageList 获取

![](../../../.gitbook/assets/tu-pian-2%20%282%29.png)

HTML名称 为要修改记录的 HTML名称 例：

![](../../../.gitbook/assets/tu-pian-3%20%282%29.png)

测试实例：

![](../../../.gitbook/assets/tu-pian-4%20%282%29.png)

![](../../../.gitbook/assets/tu-pian-5%20%282%29.png)

