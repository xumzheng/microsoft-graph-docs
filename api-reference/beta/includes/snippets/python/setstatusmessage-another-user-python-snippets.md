---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SetStatusMessagePostRequestBody()
statusMessage = PresenceStatusMessage()
statusMessageMessage = ItemBody()
statusMessageMessage.setContent('Hey I am available now')

statusMessageMessage.setContentType(BodyType('text'))


statusMessage.setMessage($statusMessageMessage)

request_body.setStatusMessage($statusMessage)


await client.usersById('user-id').presence.setStatusMessage.post(request_body)


```