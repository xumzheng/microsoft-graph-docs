---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetMailTipsPostRequestBody()
request_body.setEmailAddresses(['danas@contoso.onmicrosoft.com', 'fannyd@contoso.onmicrosoft.com', ])

request_body.setMailTipsOptions(MailTipsType('automaticreplies, mailboxfullstatus'))



result = await client.me_getMailTips.post(request_body)


```