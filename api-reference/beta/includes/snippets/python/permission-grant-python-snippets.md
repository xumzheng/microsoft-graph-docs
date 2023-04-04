---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GrantPostRequestBody();
recipientsDriveRecipient1 = DriveRecipient();
recipientsDriveRecipient1.setEmail('john@contoso.com');


recipientsArray []= recipientsDriveRecipient1;
recipientsDriveRecipient2 = DriveRecipient();
recipientsDriveRecipient2.setEmail('ryan@external.com');


recipientsArray []= recipientsDriveRecipient2;
request_body.setRecipients(recipientsArray);


request_body.setRoles(['read', ]);



result = await client.sharesById('sharedDriveItem-id').permission.grant.post(request_body);


```