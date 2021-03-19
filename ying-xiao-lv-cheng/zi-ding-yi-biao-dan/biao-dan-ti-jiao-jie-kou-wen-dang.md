# 表单提交接口文档

### 1、Action提交方式

POST: /questionnaire/api/web-api/questionnaire/v1/submit/{formId}

_备注：{formId}可以通过导出的html中检索”paperId”_

Header：

             Content-Type：application/x-www-form-urlencoded 

Request： 

             __PathParameters： 

                         formIdInteger表单id 

Response： 

             BodyParameters： 

                        Key-Value表单提交数据，见示例

请求示例：

![](../../.gitbook/assets/image%20%28590%29.png)

返回码说明：

            页面后台重定向自动跳转，无返回值。 

备注： 无

### 2、ajax提交方式

/questionnaire/api/web-api/questionnaire/v1/submitByForm/{formId} 

Header： 

            Content-Type：multipart/form-data 

            注意：不要使用RequestPayload方式 

Request： 

            PathParameters： 

                       formIdInteger表单id 

Response： 

Success200

![](../../.gitbook/assets/image%20%28581%29.png)

请求示例：

![](../../.gitbook/assets/image%20%28585%29.png)

![](../../.gitbook/assets/image%20%28587%29.png)

备注: 

       设置隐藏字段【GOTOURL】时，type返回3，content会返回设置的跳转路径

