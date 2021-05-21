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
{% api-method-parameter name="formSn" type="string" required=true %}
 表单sn
{% endapi-method-parameter %}

{% api-method-parameter name="pageNo" type="string" required=true %}
 页码
{% endapi-method-parameter %}

{% api-method-parameter name="pageSize" type="string" required=true %}
 分页数量
{% endapi-method-parameter %}

{% api-method-parameter name="filterRelation" type="integer" required=false %}
 过滤关系 1:且 2:或 不传默认为1
{% endapi-method-parameter %}

{% api-method-parameter name="filters" type="array" required=false %}
 过滤器
{% endapi-method-parameter %}

{% api-method-parameter name="filterType" type="number" required=false %}
 过滤器类型    
表单问题为字符串类型时\(1:等于,2:不等于,3:包含,4:不包含,5:有值,6:没值,7:属于,8:不属于\)   
 表单问题为时间类型时\(9:绝对时间,10:相对当前时间点,11:有值,12:没值）
{% endapi-method-parameter %}

{% api-method-parameter name="filterValue" type="object" required=false %}
 过滤器值
{% endapi-method-parameter %}

{% api-method-parameter name="formQuestionSn" type="string" required=false %}
 表单问题sn ，目前支持字符串fieldType为0的表单问题
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

> formQuestionSn字段从表单问题列表接口响应参数的字段sn获取

#### 响应参数

     请参考表单问题列表返回参数含义

#### 过滤器请求示例

* 等于 filterType = 1 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":1,
            "filterValue":"test@email.com"
        }
    ]
}
```

* 不等于 filterType = 2 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":2,
            "filterValue":"test@email.com"
        }
    ]
}
```

* 包含 filterType = 3

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":3,
            "filterValue":"test@email.com"
        }
    ]
}
```

*  不包含 filterType = 4

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":4,
            "filterValue":"test@email.com"
        }
    ]
}
```

* 有值 filterType = 5

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":5
        }
    ]
}
```

* 没值 filterType = 6 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":6
        }
    ]
}
```

* 属于 filterType = 7 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":7,
            "filterValue":[
                "testone@email.com",
                "testtwo@email.com"
            ]
        }
    ]
}
```

* 不属于 filterType = 8 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":8,
            "filterValue":[
                "testone@email.com",
                "testtwo@email.com"
            ]
        }
    ]
}
```

* 绝对时间 filterType = 9 

> startTime:开始时间，endTime:结束时间，时间格式为yyyy-MM-dd HH:mm

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":9,
            "filterValue":{
                "startTime":"2021-05-20 00:00",
                "endTime":"2021-05-20 23:59"
            }
        }
    ]
}
```

* 相对当前时间点 filterType = 10 

> days:几天，type:0\(以内\)/1\(以前\)

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":10,
            "filterValue":{
                "days":1,
                "type":1
            }
        }
    ]
}
```

* 有值 filterType = 11 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":11
        }
    ]
}
```

* 没值 filterType = 12 

```text
{
    "formSn":"06ef766448e0a1eb",
    "pageNo":1,
    "pageSize":100,
    "filters":[
        {
            "formQuestionSn":"c9d4455d1b88e72f",
            "filterType":12
        }
    ]
}
```



