---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Subscription()
request_body.changeType = 'created'

request_body.notificationUrl = 'https://webhook.azurewebsites.net/api/send/myNotifyClient'

request_body.resource = 'me/mailFolders(\'Inbox\')/messages'

request_body.expirationDateTime = DateTime('2016-11-20T18:23:45.9356913Z')

request_body.clientState = 'secretClientValue'

request_body.latestSupportedTlsVersion = 'v1_2'




result = await client.subscriptions.post(request_body = request_body)


```