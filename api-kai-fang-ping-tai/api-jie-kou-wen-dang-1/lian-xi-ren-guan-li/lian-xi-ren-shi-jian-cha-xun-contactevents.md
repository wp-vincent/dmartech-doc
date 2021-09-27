# 联系人事件查询/contactEvents

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/contactEvents" %}
{% api-method-summary %}
联系人事件查询
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

{% api-method-query-parameters %}
{% api-method-parameter name="customerId " type="string" required=true %}
联系人ID，可通过/contact/contactPageList 获取
{% endapi-method-parameter %}

{% api-method-parameter name="pageNo " type="string" required=true %}
页码
{% endapi-method-parameter %}

{% api-method-parameter name="pageSize " type="string" required=true %}
每页多少条，上限20
{% endapi-method-parameter %}

{% api-method-parameter name="fromDate" type="string" %}
起始时间，非必填，例如2021-09-17
{% endapi-method-parameter %}

{% api-method-parameter name="toDate" type="string" %}
4结束时间，非必填，例如2021-09-30
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
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

参数获取：**（截图url为测试环境，实际以上方信息为准。）**

customerId \* 联系人ID，可通过/contact/contactPageList 获取

![](blob:https://app.gitbook.com/f33b8e21-a0c9-47f6-8a56-a1dccd81a06e)

![](blob:https://app.gitbook.com/617f1f9a-0d62-4d85-beb1-c949eec70f47)

