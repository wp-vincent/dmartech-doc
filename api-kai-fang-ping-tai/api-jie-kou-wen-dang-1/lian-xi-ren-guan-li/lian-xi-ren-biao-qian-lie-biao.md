# 联系人标签列表





{% api-method method="get" host="https://api.dmartech.cn/openapi" path="/open-api/v1/contact/contactLabelList" %}
{% api-method-summary %}
 联系人标签列表
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="customerId" type="string" required=true %}
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
    "traceNumber": "c1e89108db6e4f7e8e79cc902a7a2386",
    "data": {
        "customerLabelList": [
            {
                "name": "哈哈哈的标签",
                "sn": "0f8e94d9965e8c67"
            },
            {
                "name": "9-10-标签不属于条件测试",
                "sn": "7873ad641d292e48"
            }
        ],
        "fansLabelList": [
            {
                "appid": "wxef09590e7de97fd0",
                "fansLabelInfoList": []
            },
            {
                "appid": "wx7a137c6c7eaa3f70",
                "fansLabelInfoList": [
                    {
                        "name": "1029034",
                        "sn": "1dfae073b2a4b46a"
                    },
                    {
                        "name": "再次更改09-5",
                        "sn": "fedd1f9af403845b"
                    }
                ]
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



### 返回参数说明 <a id="fan-hui-can-shu-shuo-ming"></a>

| 字段名 | 描述 |
| :--- | :--- |
| customerLabelList | 联系人标签列表 |
| fansLabelList | 微信粉丝标签列表 |
| appid | 公众号id |

