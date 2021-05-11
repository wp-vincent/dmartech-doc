# 表单问题列表

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/questionList" %}
{% api-method-summary %}
 表单问题列表
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="formSn" type="string" required=true %}
 表单sn
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{
  "code": 0,
  "data": [
    {
      "field": "string",
      "fieldName": "string",
      "fieldType": 0,
      "sn": "string"
    }
  ],
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

#### 响应参数

<table>
  <thead>
    <tr>
      <th style="text-align:left">&#x5B57;&#x6BB5;&#x540D;</th>
      <th style="text-align:left">&#x7C7B;&#x578B;</th>
      <th style="text-align:left">&#x63CF;&#x8FF0;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">field</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x5B57;&#x6BB5;</td>
    </tr>
    <tr>
      <td style="text-align:left">fieldName</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x5B57;&#x6BB5;&#x540D;&#x79F0;</td>
    </tr>
    <tr>
      <td style="text-align:left">fieldType</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">
        <p>&#x5B57;&#x6BB5;&#x7C7B;&#x578B;</p>
        <p>0:&#x5B57;&#x7B26;&#x4E32;</p>
        <p>1:&#x6574;&#x6570;</p>
        <p>2:&#x65F6;&#x95F4;</p>
        <p>3:&#x5C0F;&#x6570;</p>
        <p>4:&#x5E03;&#x5C14;&#x503C;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">sn</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x5B57;&#x6BB5;sn</td>
    </tr>
  </tbody>
</table>



