---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TentativelyAcceptPostRequestBody();
requestBody.setComment('I will probably be able to make it.');

requestBody.setSendResponse(true);



awaitclient.me().eventsById('event-id').tentativelyAccept().post(requestBody);


```