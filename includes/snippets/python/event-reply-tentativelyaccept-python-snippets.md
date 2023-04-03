---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TentativelyAcceptPostRequestBody();
requestBody.setComment('I will probably be able to make it.');

requestBody.setSendResponse(true);



graphServiceClient.me().eventsById('event-id').tentativelyAccept().post(requestBody);


```