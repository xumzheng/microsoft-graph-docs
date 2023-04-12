---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetMailTipsPostRequestBody()
request_body.EmailAddresses(['danas@contoso.onmicrosoft.com', 'fannyd@contoso.onmicrosoft.com', ])

request_body.MailTipsOptions(MailTipsType('automaticreplies, mailboxfullstatus'))




result = await client.me.getMailTips.post(request_body = request_body)


```