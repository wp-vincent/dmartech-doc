# 联系人打分评级

     

​

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/contactGradeScoreList" %}
{% api-method-summary %}
 联系人打分评级
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="name" type="string" required=false %}
查询主键子段名
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" required=false %}
查询值
{% endapi-method-parameter %}

{% api-method-parameter name="customerId" type="string" required=false %}
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
    "traceNumber": "ca2725f51d91467788b65b340feeb0d6",
    "data": {
      "resultList": [
        {
          "gradeRule": "string",
          "rank": "string",
          "score": "string"
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

### 注意事项

name  value为一组查询条件，customerI为一组查询条件，两者不能同时存在。

### 返回参数说明 <a id="fan-hui-can-shu-shuo-ming"></a>

| 字段名 | 描述 |
| :--- | :--- |
| gradeRule | 评级规则 |
| score | 实际得分 |
| rank | 分值等级 |



