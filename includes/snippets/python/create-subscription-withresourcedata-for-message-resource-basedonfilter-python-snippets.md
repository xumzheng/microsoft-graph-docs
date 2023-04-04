---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Subscription();
request_body.setChangeType('created');

request_body.setNotificationUrl('https://webhook.azurewebsites.net/api/send/myNotifyClient');

request_body.setResource('me/mailfolders(\'Drafts\')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq \'High\'');

request_body.setExpirationDateTime(DateTime('2022-01-01T21:42:18.2257768+00:00'));

request_body.setClientState('secretClientValue');

request_body.setIncludeResourceData(true);

request_body.setEncryptionCertificate('MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==');

request_body.setEncryptionCertificateId('testCertificateId');



result = await client.subscriptions.post(request_body);


```