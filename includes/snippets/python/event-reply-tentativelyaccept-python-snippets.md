---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TentativelyAcceptPostRequestBody();
requestBody.setComment('I will probably be able to make it.');

requestBody.setSendResponse(true);



await client.me().eventsById('event-id').tentativelyAccept().post(requestBody);


```