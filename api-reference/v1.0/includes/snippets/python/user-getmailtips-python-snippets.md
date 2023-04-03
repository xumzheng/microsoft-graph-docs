---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GetMailTipsPostRequestBody();
requestBody.setEmailAddresses(['danas@contoso.onmicrosoft.com', 'fannyd@contoso.onmicrosoft.com', ]);

requestBody.setMailTipsOptions(MailTipsType('automaticreplies, mailboxfullstatus'));



result = awaitclient.me().getMailTips().post(requestBody);


```