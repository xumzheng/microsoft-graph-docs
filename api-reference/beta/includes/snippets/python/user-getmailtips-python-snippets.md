---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GetMailTipsPostRequestBody();
$requestBody->setEmailAddresses(['danas@contoso.onmicrosoft.com', 'fannyd@contoso.onmicrosoft.com', ]);

$requestBody->setMailTipsOptions(new MailTipsType('automaticreplies, mailboxfullstatus'));



$requestResult = $graphServiceClient->me()->getMailTips()->post($requestBody);


```