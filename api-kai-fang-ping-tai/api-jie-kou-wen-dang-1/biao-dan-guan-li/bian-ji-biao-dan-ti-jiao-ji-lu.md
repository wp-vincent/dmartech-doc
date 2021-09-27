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
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
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

  参数获取实例：**（截图url为测试环境，实际以上方信息为准。）**

  formSn:   通过/form/formPageList 获取

![](blob:https://app.gitbook.com/f07fd4e5-4811-496f-ae33-0b689c77a7f4)

\_id  :  通过/form/submitRecordPageList 获取

![](blob:https://app.gitbook.com/7134f2dd-51ce-490a-839d-2297d616a9e2)

HTML名称 为要修改记录的 HTML名称 例：

![](blob:https://app.gitbook.com/a9c981a3-c266-48c9-ae92-3dd48f67d84a)

测试实例：

![](blob:https://app.gitbook.com/339c5f4c-6a52-421f-b2ff-3d22c0a4973a)

![](blob:https://app.gitbook.com/25e0e6eb-4b96-45a4-8128-99c7d330b31d)

