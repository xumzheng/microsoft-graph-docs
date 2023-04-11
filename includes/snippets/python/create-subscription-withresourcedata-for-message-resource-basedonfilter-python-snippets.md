---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Subscription()
request_body.changeType = 'created'

request_body.notificationUrl = 'https://webhook.azurewebsites.net/api/send/myNotifyClient'

request_body.resource = 'me/mailfolders(\'Drafts\')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq \'High\''

request_body.expirationDateTime = DateTime('2022-01-01T21:42:18.2257768+00:00')

request_body.clientState = 'secretClientValue'

request_body.includeResourceData = true

request_body.encryptionCertificate = 'MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA=='

request_body.encryptionCertificateId = 'testCertificateId'



request_configuration = SubscriptionsRequestBuilderPostRequestConfiguration(
)


result = await client.subscriptions.post(request_body = request_body)


```