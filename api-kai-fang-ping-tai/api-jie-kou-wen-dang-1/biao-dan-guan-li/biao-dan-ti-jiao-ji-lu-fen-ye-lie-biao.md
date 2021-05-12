# 表单提交记录分页列表

{% api-method method="post" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/submitRecordPageList" %}
{% api-method-summary %}
 表单提交记录分页列表
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
{% api-method-parameter name="formSn" type="string" required=false %}
 表单sn
{% endapi-method-parameter %}

{% api-method-parameter name="pageNo" type="string" required=true %}
 页码
{% endapi-method-parameter %}

{% api-method-parameter name="pageSize" type="string" required=true %}
 分页数量
{% endapi-method-parameter %}

{% api-method-parameter name="filters" type="array" required=false %}
 过滤器
{% endapi-method-parameter %}

{% api-method-parameter name="filterType" type="number" required=false %}
 过滤器类型 1:等于,2:不等于,3:包含
{% endapi-method-parameter %}

{% api-method-parameter name="filterValue" type="string" required=false %}
 过滤器值
{% endapi-method-parameter %}

{% api-method-parameter name="formQuestionSn" type="string" required=false %}
 表单问题sn
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
  "data": {
    "resultList": [
      {}
    ],
    "totalPage": 0,
    "totalRow": 0
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

响应参数

     请参考表单问题列表返回参数含义

