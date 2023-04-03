---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SetStatusMessagePostRequestBody();
statusMessage = PresenceStatusMessage();
statusMessageMessage = ItemBody();
statusMessageMessage.setContent('Hey I am available now');

statusMessageMessage.setContentType(BodyType('text'));


statusMessage.setMessage($statusMessageMessage);

requestBody.setStatusMessage($statusMessage);


awaitclient.usersById('user-id').presence().setStatusMessage().post(requestBody);


```