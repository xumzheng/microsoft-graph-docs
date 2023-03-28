---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GrantPostRequestBody();
$recipientsDriveRecipient1 = new DriveRecipient();
$recipientsDriveRecipient1.setEmail('john@contoso.com');


$recipientsArray []= $recipientsDriveRecipient1;
$recipientsDriveRecipient2 = new DriveRecipient();
$recipientsDriveRecipient2.setEmail('ryan@external.com');


$recipientsArray []= $recipientsDriveRecipient2;
$requestBody.setRecipients($recipientsArray);


$requestBody.setRoles(['read', ]);



$requestResult = $graphServiceClient.sharesById('sharedDriveItem-id').permission().grant().post($requestBody);


```