# 表单分页列表/formPageList

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/formPageList" %}
{% api-method-summary %}
 表单分页列表
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
 关键字\(表单名称\)
{% endapi-method-parameter %}

{% api-method-parameter name="sortField" type="string" required=false %}
 排序字段 createDate:创建时间,updateDate:更新时间
{% endapi-method-parameter %}

{% api-method-parameter name="sortOrder" type="string" required=false %}
 排序类型 desc:倒序,asc:正序
{% endapi-method-parameter %}

{% api-method-parameter name="type" type="string" required=false %}
 表单类型 JSJ:金数据表单,DMT:标准表单
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
        "commitDataCount": 0,
        "commitPersonCount": 0,
        "createDate": "2021-01-01 00:00:00",
        "createName": "string",
        "formName": "string",
        "sn": "string",
        "status": "已发布",
        "type": "DMT",
        "updateDate": "2021-01-01 00:00:00",
        "updateName": "string"
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

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/groupList" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
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

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/groupList" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
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

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/form/groupList" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
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
      <td style="text-align:left">sn</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x8868;&#x5355;sn</td>
    </tr>
    <tr>
      <td style="text-align:left">formName</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x8868;&#x5355;&#x540D;&#x79F0;</td>
    </tr>
    <tr>
      <td style="text-align:left">type</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">
        <p>&#x8868;&#x5355;&#x7C7B;&#x578B;</p>
        <p>JSJ:&#x91D1;&#x6570;&#x636E;&#x8868;&#x5355;</p>
        <p>DMT:&#x6807;&#x51C6;&#x8868;&#x5355;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">status</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">
        <p>&#x91D1;&#x6570;&#x636E;&#x8868;&#x5355;&#x72B6;&#x6001;:&#x672A;&#x6D4B;&#x8BD5;/&#x5DF2;&#x6D4B;&#x8BD5;/&#x5DF2;&#x53D1;&#x5E03;</p>
        <p>&#x6807;&#x51C6;&#x8868;&#x5355;&#x72B6;&#x6001;:&#x6B63;&#x5E38;/&#x6682;&#x505C;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">commitDataCount</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">&#x63D0;&#x4EA4;&#x6570;&#x636E;&#x91CF;</td>
    </tr>
    <tr>
      <td style="text-align:left">commitPersonCount</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">&#x63D0;&#x4EA4;&#x4EBA;&#x6570;</td>
    </tr>
    <tr>
      <td style="text-align:left">createName</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x521B;&#x5EFA;&#x8005;</td>
    </tr>
    <tr>
      <td style="text-align:left">createDate</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x521B;&#x5EFA;&#x65F6;&#x95F4;</td>
    </tr>
    <tr>
      <td style="text-align:left">updateName</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x66F4;&#x65B0;&#x8005;</td>
    </tr>
    <tr>
      <td style="text-align:left">updateDate</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">&#x66F4;&#x65B0;&#x65F6;&#x95F4;</td>
    </tr>
  </tbody>
</table>



