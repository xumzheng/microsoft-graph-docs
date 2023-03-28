---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Subscription();
$requestBody.setChangeType('created');

$requestBody.setNotificationUrl('https://webhook.azurewebsites.net/api/send/myNotifyClient');

$requestBody.setResource('me/mailfolders(\'Drafts\')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq \'High\'');

$requestBody.setExpirationDateTime(new DateTime('2022-01-01T21:42:18.2257768+00:00'));

$requestBody.setClientState('secretClientValue');

$requestBody.setIncludeResourceData(true);

$requestBody.setEncryptionCertificate('MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==');

$requestBody.setEncryptionCertificateId('testCertificateId');



$requestResult = $graphServiceClient.subscriptions().post($requestBody);


```