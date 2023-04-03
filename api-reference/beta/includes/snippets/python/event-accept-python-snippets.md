---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AcceptPostRequestBody();
requestBody.setComment('comment-value');

requestBody.setSendResponse(true);



graphServiceClient.me().eventsById('event-id').accept().post(requestBody);


```