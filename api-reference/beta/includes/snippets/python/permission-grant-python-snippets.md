---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GrantPostRequestBody();
recipientsDriveRecipient1 = DriveRecipient();
recipientsDriveRecipient1.setEmail('john@contoso.com');


recipientsArray []= recipientsDriveRecipient1;
recipientsDriveRecipient2 = DriveRecipient();
recipientsDriveRecipient2.setEmail('ryan@external.com');


recipientsArray []= recipientsDriveRecipient2;
requestBody.setRecipients(recipientsArray);


requestBody.setRoles(['read', ]);



result = awaitclient.sharesById('sharedDriveItem-id').permission().grant().post(requestBody);


```