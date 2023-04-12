---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetStatusMessagePostRequestBody()
statusMessage = PresenceStatusMessage()
statusMessageMessage = ItemBody()
statusMessageMessage.content = 'Hey I\'m currently in a meeting.'

statusMessageMessage.ContentType(BodyType('text'))


statusMessage.message = statusMessageMessage
statusMessageExpiryDateTime = DateTimeTimeZone()
statusMessageExpiryDateTime.dateTime = '2022-10-18T17:05:33.2079781'

statusMessageExpiryDateTime.timeZone = 'Pacific Standard Time'


statusMessage.expiryDateTime = statusMessageExpiryDateTime

request_body.statusMessage = statusMessage



await client.users_by_id('user-id').presence.setStatusMessage.post(request_body = request_body)


```