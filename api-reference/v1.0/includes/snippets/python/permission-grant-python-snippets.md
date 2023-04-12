---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GrantPostRequestBody()
recipientsDriveRecipient1 = DriveRecipient()
recipientsDriveRecipient1.email = 'john@contoso.com'


recipientsArray []= recipientsDriveRecipient1;
recipientsDriveRecipient2 = DriveRecipient()
recipientsDriveRecipient2.email = 'ryan@external.com'


recipientsArray []= recipientsDriveRecipient2;
request_body.recipients(recipientsArray)


request_body.Roles(['read', ])




result = await client.shares_by_id('sharedDriveItem-id').permission.grant.post(request_body = request_body)


```