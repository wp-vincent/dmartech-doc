# 标签分页列表/labelPageList

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/labelPageList" %}
{% api-method-summary %}
 标签分页列表
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
{% api-method-parameter name="pageNo" type="string" required=true %}
 页码
{% endapi-method-parameter %}

{% api-method-parameter name="pageSize" type="string" required=true %}
 分页数量
{% endapi-method-parameter %}

{% api-method-parameter name="groupSn" type="string" required=false %}
 分组sn
{% endapi-method-parameter %}

{% api-method-parameter name="keywords" type="string" required=false %}
 关键字\(名称\)
{% endapi-method-parameter %}

{% api-method-parameter name="sortField" type="string" required=false %}
 排序字段 createDate:创建时间,updateDate:更新时间
{% endapi-method-parameter %}

{% api-method-parameter name="sortOrder" type="string" required=false %}
 排序类型 desc:倒序,asc:正序
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
  "data": {
    "resultList": [
      {
        "contactCount": 0,
        "id":"number"
        "isConceal": 0,
        "labelName": "string",
        "sn": "string",
        "updateDate": "2021-01-01 00:00:00"
      }
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

#### 响应参数

<table>
  <thead>
    <tr>
      <th style="text-align:left">&#x53C2;&#x6570;&#x540D;</th>
      <th style="text-align:left">&#x7C7B;&#x578B;</th>
      <th style="text-align:left">&#x63CF;&#x8FF0;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">sn</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x6807;&#x7B7E;sn</td>
    </tr>
    <tr>
      <td style="text-align:left">labelName</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x6807;&#x7B7E;&#x540D;&#x79F0;</td>
    </tr>
    <tr>
      <td style="text-align:left">isConceal</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">
        <p>&#x9690;&#x85CF;&#x72B6;&#x6001;</p>
        <p>0:&#x4E0D;&#x9690;&#x85CF;</p>
        <p>1:&#x9690;&#x85CF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">contactCount</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">&#x8054;&#x7CFB;&#x4EBA;&#x6570;&#x91CF;</td>
    </tr>
    <tr>
      <td style="text-align:left">updateDate</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x66F4;&#x65B0;&#x65F6;&#x95F4;</td>
    </tr>
    <tr>
      <td style="text-align:left">id</td>
      <td style="text-align:left">number</td>
      <td style="text-align:left">&#x6807;&#x7B7E;id</td>
    </tr>
  </tbody>
</table>

