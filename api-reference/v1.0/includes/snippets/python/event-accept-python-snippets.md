---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AcceptPostRequestBody();
requestBody.setComment('comment-value');

requestBody.setSendResponse(true);



await client.me().eventsById('event-id').accept().post(requestBody);


```