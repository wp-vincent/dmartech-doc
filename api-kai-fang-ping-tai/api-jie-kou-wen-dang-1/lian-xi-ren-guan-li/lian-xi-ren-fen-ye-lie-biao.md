# 联系人分页列表

{% api-method method="get" host="https://api.dmartech.cn" path="/open-api/v1/contact/contactPageList" %}
{% api-method-summary %}
 联系人分页列表
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="appIds" type="array" required=false %}
公众号appId数组（当查询customerType为3，微信粉丝客户的时候必传。）
{% endapi-method-parameter %}

{% api-method-parameter name="customerType" type="number" required=true %}
联系人列表类型 1.实名客户 2.匿名客户 3.微信粉丝客户 4.全部客户
{% endapi-method-parameter %}

{% api-method-parameter name="pageNo" type="number" required=true %}
页码
{% endapi-method-parameter %}

{% api-method-parameter name="pageSize" type="number" required=true %}
分页数量
{% endapi-method-parameter %}

{% api-method-parameter name="searchField" type="string" required=false %}
搜索字段 （搜索字段为联系人字段详情接口的sn字段，字段能否搜索请参考联系人字段详情接口的searchType字段）
{% endapi-method-parameter %}

{% api-method-parameter name="searchValue" type="string" required=false %}
 搜索值
{% endapi-method-parameter %}

{% api-method-parameter name="sortField" type="string" required=false %}
 排序字段 联系人字段详情接口的fieldName字段，字段能否排序请参考联系人字段详情接口的sortType字段
{% endapi-method-parameter %}

{% api-method-parameter name="sortOrder" type="string" required=false %}
 排序类型 desc\(倒序\)/asc\(正序\)
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
    "traceNumber": "95cb7914841740e8896316702c322518",
    "data": {
        "totalPage": 86,
        "totalRow": 852,
        "resultList": [
            {
                "联系人名称": "yi",
                "手机号": "15865591190",
                "customerId": "7e2375a3-6f48-4ffe-bbc8-3352e09f194f",
                "微信": "是",
                "导入时间": "2019-12-19 13:56",
                "更新时间": "2021-04-08 06:06"
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

