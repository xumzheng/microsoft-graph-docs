---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SetStatusMessagePostRequestBody();
statusMessage = PresenceStatusMessage();
statusMessageMessage = ItemBody();
statusMessageMessage.setContent('Hey I\'m currently in a meeting.');

statusMessageMessage.setContentType(BodyType('text'));


statusMessage.setMessage($statusMessageMessage);
statusMessageExpiryDateTime = DateTimeTimeZone();
statusMessageExpiryDateTime.setDateTime('2022-10-18T17:05:33.2079781');

statusMessageExpiryDateTime.setTimeZone('Pacific Standard Time');


statusMessage.setExpiryDateTime($statusMessageExpiryDateTime);

requestBody.setStatusMessage($statusMessage);


awaitclient.usersById('user-id').presence().setStatusMessage().post(requestBody);


```