---
description: About drag and drop editor compatibility instructions
---

# 关于拖拽编辑器兼容性说明

邮件的本质是HTML&CSS代码，而可惜的是，邮件编码至今**没有统一的标准**，各家邮件服务商e及开发者都可以制定自己的邮件编码渲染标准。

Email is based on HTML & CSS code,  unfortunately, there is **no standard for email coding**, and various email service providers have developed their own mail coding rendering standards.

这意味着不同的邮件服务商和客户端会对HTML&CSS代码进行不同方式的渲染，比如Chrome浏览器，它采取的是webkit引擎渲染；比如outlook客户端，它采取的是word HTML引擎渲染，同一封邮件，**在不同的渲染方式下会得出不同的结果**。

This means that different email providers and clients will render HTML & CSS code differently, such as Chrome browser, which takes webkit engine rendering; Outlook client, which takes word HTML engine rendering, **the same email will return different results due to different rendering engine.**

为了保证能被大多数用户正确查看邮件样式，拖拽式编辑器采取的是&lt;table&gt;的布局方式，而非&lt;div&gt;。然而，**我们仍无法保证能够100%完好的展示在每一个邮件客户端中，尤其是以word HTML引擎渲染的各种outlook客户端**。

To ensure that most users can view the message  correctly, the drag-and-drop editor takes the layout of  &lt;table&gt; instead of &lt;div&gt;. However, **we still can't guarantee 100% correct display in every email client, especially the various versions of Outlook clients which rendered by the word HTML engine.**

我们建议忽略邮件在不同客户端下的细微差别，因为几乎不可能做到100%一模一样。如果你特别追求完美，或特别强调在outlook下的完美展现，我们建议：

1. 单独进行邮件coding，然后通过上传zip或粘贴代码的形式制作邮件。
2. 尽可能的使用简单风格的邮件，避免使用过多风格。

We recommend ignoring the nuances of email's display under different clients, as it is almost impossible to do 100% exactly the same as you view in drag-and-drop editor. If you are particularly striving for perfection, or special emphasis on the perfect presentation under outlook client, we recommend:

1. Code you email by your own, then upload to Dmartech via zip file or copy code mode.
2. Use the styles as simply as possible, don't put too much css code.



Reference 参考：

> CSS support guide：[https://www.campaignmonitor.com/css/email-client/outlook-2007-16/](https://www.campaignmonitor.com/css/email-client/outlook-2007-16/)
>
> Word 2007 HTML and CSS Rendering Capabilities in Outlook 2007：[https://docs.microsoft.com/en-us/previous-versions/office/developer/office-2007/aa338201\(v=office.12\)](https://docs.microsoft.com/en-us/previous-versions/office/developer/office-2007/aa338201%28v=office.12%29)
>
> HTML邮件兼容性问题：[https://blog.csdn.net/Young\_Gao/article/details/83658454](https://blog.csdn.net/Young_Gao/article/details/83658454)



