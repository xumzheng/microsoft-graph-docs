---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GetMailTipsPostRequestBody();
requestBody.setEmailAddresses(['danas@contoso.onmicrosoft.com', 'fannyd@contoso.onmicrosoft.com', ]);

requestBody.setMailTipsOptions(MailTipsType('automaticreplies, mailboxfullstatus'));



result = await client.me().getMailTips().post(requestBody);


```