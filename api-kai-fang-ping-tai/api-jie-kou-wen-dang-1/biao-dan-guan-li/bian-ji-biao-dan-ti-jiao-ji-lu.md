---
description: editRecord
---

# 编辑表单提交记录/editRecord

{% swagger baseUrl="https://api.dmartech.cn/openapi" path="/open-api/v1/form/editRecord" method="put" summary=" 编辑表单提交记录" %}
{% swagger-description %}
 调用此接口注意事项：

\



{% endswagger-description %}

{% swagger-parameter in="header" name="access-key" type="string" %}
 访问凭证
{% endswagger-parameter %}

{% swagger-parameter in="header" name="access-sign" type="string" %}
 访问签名
{% endswagger-parameter %}

{% swagger-parameter in="body" name="formSn" type="string" %}
必填，通过/form/formPageList 获取。
{% endswagger-parameter %}

{% swagger-parameter in="body" name="_Id" type="string" %}
表单提交记录ID，必填，不能使用cutomerid或其他主键，因为可能重复提交且未加密。通过/form/submitRecordPageList 获取。
{% endswagger-parameter %}

{% swagger-parameter in="body" name="htmlName" type="string" %}
必填，表单项的HTML名称，而非字段名称以及对应的值。例如：formItem1
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{
    "code": 0,
    "message": "Successful.",
    "traceNumber": "9fb45ada62024164ace92dd1542a081d",
    "data": null
}
```
{% endswagger-response %}
{% endswagger %}

  参数获取实例：**（截图url为测试环境，实际以上方信息为准。）**

  formSn:   通过/form/formPageList 获取

![](<../../../.gitbook/assets/tu-pian-1 (3).png>)

\_id  :  通过/form/submitRecordPageList 获取

![](<../../../.gitbook/assets/tu-pian-2 (2).png>)

HTML名称 为要修改记录的 HTML名称 例：

![](<../../../.gitbook/assets/tu-pian-3 (2).png>)

测试实例：

![](<../../../.gitbook/assets/tu-pian-4 (2).png>)

![](<../../../.gitbook/assets/tu-pian-5 (2).png>)
