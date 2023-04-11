---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetStatusMessagePostRequestBody()
statusMessage = PresenceStatusMessage()
statusMessageMessage = ItemBody()
statusMessageMessage.content = 'Hey I am available now'

statusMessageMessage.ContentType(BodyType('text'))


statusMessage.message = statusMessageMessage

request_body.statusMessage = statusMessage


request_configuration = SetStatusMessageRequestBuilderPostRequestConfiguration(
)


await client.users_by_id('user-id').presence.setStatusMessage.post(request_body = request_body)


```