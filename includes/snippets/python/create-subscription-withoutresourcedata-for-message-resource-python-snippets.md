---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Subscription()
request_body.setChangeType('created')

request_body.setNotificationUrl('https://webhook.azurewebsites.net/api/send/myNotifyClient')

request_body.setResource('users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages')

request_body.setExpirationDateTime(DateTime('2021-07-07T21:42:18.2257768+00:00'))

request_body.setClientState('secretClientState')



result = await client.subscriptions.post(request_body)


```